Jekyll plugin Abbreviation
==========================

A simple plugin for Jekyll (or Octopress) that will surround abbreviations with `<abbr>` tags and a title. The title is taken from a YAML file.

It only matches full word abbreviations, so no matches for spaces,
dots ... (e.g. will not work as abbreviation). It won’t replace
abbreviations in attributes or already surrounded by an abbreviation.

If you have abbreviations with multiple meanings add `#` plus a number to
differentiate (DSL#1, DSL#2). During rendering this will be cut of.

For more examples how this works look into abbreviation.yml.

And as always: with REGEX – there might be some edge cases where
it won’t work

Usage
-----

    <div class="entry-content">{{ content | abbr }}</div>

Input (example)
---------------

    HTML

Output (example)
----------------

    <abbr title="Hypertext Markup Language">HTML</abbr>
