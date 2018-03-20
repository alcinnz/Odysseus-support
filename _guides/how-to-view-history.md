---
layout: page
title: How do I find I page I've visited before?
---

All pages you've visited are accessible at [odysseus:history](odysseus:history), which is linked to from the newtab page and the gear menu. That page lists your browser history from the time you've updated to version 1.1.0 in reverse chronological order, whilst highlighting changes in hours, days, months, and years to make it easier to skim.

Alternatively you can attempt to recall a web address you've visited before and Odysseus will suggest what it might have been.

## Components of the history viewer
The main contents of the [history viewer](odysseus:history) is a list of links to pages you've visited. The different days you've surfed the web are labelled as headers in this list, and the time you've visited a page precedes the link to it. Changes in these dates and times are highlighted in bold for easy skimming.

In the topright is written the time-range of all the history records visible on the current page and on the bottom each dot links to other timeranges of your browser history. Hover over a dot for the timerange to which it links. And in the topleft is a searchbox into which you can enter words to limit your visible browser history to records which matches at least one of those words.

## Searchbox details

At it's most basic, the searchbox allows you to enter words to see all history records which shares at least one of those words, ignoring most suffixes. However other query forms are supported as well:

<style>code {background: #aaa; font: monospace; font-weight: normal;}</style>

<table>
  <tr>
    <th><code>"</code>text...<code>"</code></th>
    <td>Matches records which contains the quoted <em>text</em> in sequence, again ignoring most suffixes.</td>
  </tr>
  <tr>
    <th>term <code>+</code> term2</th>
    <td>Matches records where <em>term2</em> immediately follows <em>term</em>.</td>
  </tr>
  <tr>
    <th>prefix <code>*</code></th>
    <td>Matches records containing a term prefixed by <em>prefix</em>.</td>
  </tr>
  <tr>
    <th><code>^</code> term</th>
    <td>Matches records whose title starts with <em>term</em>.</td>
  </tr>
  <tr>
    <th><code>NEAR(</code>terms..., N<code>)</code></th>
    <td><p>Matches records where all the specified <em>terms</em> are within <em>N</em> words of each other.</p>
      <p>If N is not specified N = 10.</p></td>
  </tr>
  <tr>
    <th><code>uri:(</code>terms...<code>)</code></th>
    <td><p>Matches the <em>terms</em> exclusively against the the URIs of the history records.</p>
        <p>If your matching just one term, the parenthesese are optional.</p></td>
  </tr>
  <tr>
    <th><code>title:(</code>terms...<code>)</code></th>
    <td>As per uri: but matches against the title of the visited pages.</p>
  </tr>
  <tr>
    <th>query <code>AND</code> query2</th>
    <td>Matches records only if they match both <em>query</em> and <em>query2</em>.</td>
  </tr>
  <tr>
    <th>query <code>OR</code> query2</th>
    <td>Matches records if at least one of <em>query</em> or <em>query2</em> matches.</td>
  </tr>
  <tr>
    <th>query <code>NOT</code> query2</th>
    <td>Matches records which match <em>query</em> but not <em>query2</em>.</td>
  </tr>
</table>
