![Maintenance](https://img.shields.io/maintenance/no/2012.svg)

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

The MIT License
---------------

Copyright (c) 2012 Stefan Imhoff

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
