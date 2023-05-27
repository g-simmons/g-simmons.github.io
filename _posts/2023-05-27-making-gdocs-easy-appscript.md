---
layout: post
title: Making Google Docs slightly better with App Scripts
date: 2023-05-27
description: Apparently indentation settings are for power users only
---

I prefer not to write in Google Docs. I use Obsidian for personal note-taking and even most stages of solo manuscript writing. But now I'm working on a collaborative project. I decided against Overleaf, since I feel like writing LaTeX is mostly a distraction until the stage of the project where typesetting is actually important. Collaborative markdown editors with quick setup times leave a lot to be desired, so we ended up in Google Docs.

Start working on the document? Check.
Make an outline to keep things organized? Of course.
Indent the outline to make it easier to read? Uhhh, how many levels?

The default indentation for nested lists in Google Docs is big. Much too big. That would be fine if it were editable, but unfortunately it's not.

What would I have done before the ChatGPT era? I would have just dealt with it. 

But now I have a new hammer, and everything looks like a nail. This is actually an interesting phenomenon - apparently I'm not alone in experiencing a sort of I-can-do-everything mania after incorporating ChatGPT into my development workflow.

Anyway, I wrote a script to fix the indentation. 

See the GitHub git [here](https://gist.github.com/g-simmons/1a29de1a2a9f1cd8f3dd2f743136ffdd)

```javascript
function onOpen() {
  var ui = DocumentApp.getUi();
  ui.createMenu('Custom Menu')
    .addItem('Set Indentation and Font Size', 'setIndentationAndFontSize')
    .addToUi();
}

function setIndentationAndFontSize() {
  // var doc = DocumentApp.getActiveDocument();
  var doc = DocumentApp.openById('<<<<YOUR-DOCUMENT-ID>>>>');
  var body = doc.getBody();
  Logger.log(body);
  
  // Define indentation amounts and font sizes for each nesting level
  var indentationLevelsStart = [0,25,50,75,100,115]; // Adjust indentation values as needed
  var fontSizes = [18,14,10,8,6,6]; // Adjust font sizes as needed
  
  // Get all paragraphs in the document
  var paragraphs = body.getParagraphs();
  var numberedLists = body.getListItems();

  for (var i =0; i < numberedLists.length; i++) {
    var listItem = numberedLists[i];
    var nestingLevel = Math.floor(listItem.getNestingLevel());
    if (nestingLevel >= 0 && nestingLevel <= 6) {
        // Set the appropriate indentation and font size based on nesting level
        var indentationStart = indentationLevelsStart[nestingLevel];
        var indentationFirst = indentationStart + 18;
        var fontSize = fontSizes[nestingLevel];

        listItem.setIndentFirstLine(indentationStart);  
        try {listItem.setIndentStart(indentationFirst);}     
        catch (error){Logger.log(error);}
        
        listItem.setFontSize(fontSize);
        listItem.setGlyphType(DocumentApp.GlyphType.BULLET).setGlyphType(DocumentApp.GlyphType.NUMBER);
      }
  }
}
```

In case you're wondering, a "Glyph" is the the bullet point or string that precedes a list item.
If setting the indentation level is a power-user feature, setting the font size for the glyph must be for Google CEOs only. Since it's not in the API, I tried toggling back and forth between bullet and number glyphs to get the font size to change. This seems to work about every other time I run the script. 