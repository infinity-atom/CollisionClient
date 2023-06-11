---
title: ChatPrefix
layout: default
---
# How it works - ChatPrefix
**ChatPrefix** is a hack that puts a prefix before your message.

**ChatPrefix** works by setting the `element.value` when you focus onto the chatbox. The prefix can change by changing a variable, through the console or in the GUI.
```javascript
document.addEventListener("keydown", (e) => {
    if(e.keyCode == "Enter") {
        CHATBOX_INPUT.value = PREFIX;
    }
});
```
`CHATBOX_INPUT` and `PREFIX` are placeholders for the actual variables.
There would be extra code to get it to work only when **ChatPrefix** is enabled.