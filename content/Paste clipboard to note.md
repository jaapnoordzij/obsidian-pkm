---
{"publish":true,"title":"Paste clipboard to note","created":"2025-12-12","modified":"2025-12-14T19:29:50.328+01:00","cssclasses":""}
---

This is a small utility Shortcut that should be called from another shortcut. Its main intention is to past the content of the MacOs clipboard into you note at the current position. Exactly like Control-V would do - I made this only because i needed a way to user Control-V without switching to Obisidian.

The Shortcut is realised by calling "Avanced Uri" to execute a Templater script Command with the name `Templater: Insert tp_paste`

All this templates does is get the clipboard and leave the contents in the text. 
```
<%*
// Simply paste the clipboard contents. Used in Shortcuts.
let clipboard = await tp.system.clipboard(); // Paste link
%>
<% clipboard %>
```

Screenshot of the Apple Shortcut