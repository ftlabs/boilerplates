# boilerplates

## some simple, no-nonsense examples of things Origami.

This repo is intended to help a "I've never used Origami before" user get up and running ASAP.

This repo is *not* intended to answer all questions about Origami. For that, see [the Origami site](http://origami.ft.com/)

Starting with a straightforward html file, simple.html, there are examples of how to style it to look like
* a page on FT.com: simple-ft-styled.html
* a page in the Origami techdocs: simple-ft-techdoc-styled.doc

The basic approach is to construct two urls requesting all the required Origami modules (for css and js) and include them in the page. When the page is rendered in-browser, that css and js payload is compiled at Origami headquarters, with a noticeable delay for the first request, and served to the browser. Subsequent requests are cached, so there is no delay.

Within the page, the Origami includes override some of the basic element styling, e.g. [o-typography](http://registry.origami.ft.com/components/o-typography@3.1.0), or provide css classes to insert into some html elements, e.g. class="o-buttons".

You can consult the Origami docs for how to bring the css and js compilation into your own page build process if you want to have full control over it.
