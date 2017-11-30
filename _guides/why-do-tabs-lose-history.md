---
layout: page
title: Why do I loose my tab history?
---

This is a known issue I (Adrian Cochrane) am anxious to fix. I've tried some things out, but currently I'm waiting on others<sup title="Specifically WebKitGTK appears to have done their part, but I'm waiting on Debian to package that commit in a software update.">1</sup> to let me fix it.

The problem is that when <i>Odysseus</i> tries to recreate a previous tab it has no way to rebuild the tab history and associate it with that tab. However the data is saving, which should help me fix this problem as early as possible. 


### When does it occur?

When starting up your browser, duplicating tabs, or restoring tabs. 

---

### Things I've tried (for the technically minded)

* Calling <code>history.pushState</code> in JavaScript. Got security errors.
* Treating the history list as mutable. Only causes errors to be reported behind the scenes without fixing the problem. 
* Considered manually navigating to previous pages. Concluded that'll only horribly confuse WebKit. 
