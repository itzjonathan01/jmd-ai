# JMD AI

A self-contained AI that runs entirely in your browser. One HTML file, no
server, no API key, no account. Open it and it works.

**Live: https://itzjonathan01.github.io/jmd-ai/**

It ships with its own trained model — embeddings, an intent classifier, a
knowledge base and a 37,815-word dictionary — all inlined into the page. Your
conversations, your corrections and everything it learns from you stay in your
browser's local storage and are never sent anywhere.

## What it does

- **Answers from what it knows**, offline, with no network at all
- **Learns while you use it** — tell it a fact, correct it, rate an answer, and
  it updates and remembers across reloads
- **Fixes your spelling** before it answers, using edit distance, keyboard
  layout, how the word sounds, and word frequency
- **Checks the web** when a question actually needs current information, and
  tells you which source it used
- **Installs to your home screen** as an app

## Web access

The web layer only works from a real `https://` origin. Served from GitHub
Pages, or opened as a downloaded file, it works with nothing to configure.
Embedded in a sandboxed viewer that sets `connect-src 'self'`, the browser
blocks every outbound request before it leaves — the app detects this and says
so rather than pretending.

## Source

Built from [JMD-Virtual-PC-Web](https://github.com/itzjonathan01/JMD-Virtual-PC-Web).
This repository holds only the built file.
