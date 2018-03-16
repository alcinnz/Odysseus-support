---
layout: page
title: What's the version numbering scheme?
---

Odysseus stores data regarding the pages and links you see in it in a special file hidden in your filesystem (specifically under `~/.config/com.github.alcinnz.Odysseus/`). Any changes that don't alter how this file is structured increments the third number, anything that adds to it's structure increments the second, and any changes that might loose your data increments the first.

In practice this roughly means that the second number is reserved for majour features whilst I'll hopefully never increment the first number again.
