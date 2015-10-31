# python-epub-builder
This is a small python library for programmatically building EPUB books. It provides API for easily constructing and packaging EPUBs from text content.

To retain full power of the EPUB specification, the library makes little abstraction over EPUB constructs such as spine and TOC map, so you need to understand them (the EPUB specification makes a short and easy read, or you can use this tutorial) to get the most out of it. On the other hand, the API hides many of the technical details of the XML-based specification from you, so that you can focus on generating and manipulating text content.

Finally, a even simpler API is provided to allow you to make EPUB with a single function call. There's an example for converting a Project Gutenburg book from TXT to EPUB in 5 minutes.

The library uses Genshi for HTML/XML template, but you can use whatever mechanism for generating your content pages. Also, there is a dependency on lxml to parse EPUB manifest file. Finally, I use epubcheck to validate EPUB, so you should copy the jar file into the same directory as the py files. 
