Source-By-Line
----

This is a small tool for inserting code samples into a page from external sources. 
It's original purpose was for use with the [Reveal.js](https://github.com/hakimel/reveal.js/) 
presentation tool, although it could be used anywhere really. Simply include the 
file in a web page with the proper data attributes. It will grab external resources, 
select specific lines, then dump them back into that HTML node, with highlighting 
if you have the [highlight.js](http://highlightjs.org/) library available.


## Basic Usage

```html
<code data-srcbyline='beer.js?1-4;19-20;31-33'></code>

<script src='path/to/srcByLine.js'></script>
```

That's it... the specific lines in the data attribute will be displayed on the page, 
but no other lines in that file. If you specify a line number past the end of the 
file it will just print a blank line. And if you have the highlight.js library 
installed the highlighted HTML will be inserted instead.
