---
description: Turn a script into a narration you can paste into ElevenLabs.
argument-hint: [script file | paste the script]
---

Make a paste-ready narration from $ARGUMENTS.

1. Take the script from the file the user names in the tidbit project folder, or from the chat.
2. Rewrite it for speech: short sentences, numbers and symbols written as spoken words, no Markdown.
3. Call `save_narration` with the text, the project id (or a title to start a project) and the target length in seconds.
4. If it lists problems, fix them and call it again. Use `force` only if the user asks to keep it as is.
5. Show the `paste_ready` text in a code block and say how many seconds it runs.
