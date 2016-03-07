# tessellex
A responsive, mobile-first, progressively-enhanced CSS2/CSS3 grid

### design

Tessellex is a grid designed to allow you to give some structure to old-school
browsers using a traditional float-based approach which gets replaced with
turbo-charged flexbox awesomeness on newer, more capable browsers.

The traditional grid is more limited in its capabilities than its flexbox-based
counterpart. See the feature comparison table below.

### how to use

1. Include `tessellex.css` in your project, either via compiling the Sass or using the pre-compiled CSS file.
2. Include [modernizr](https://modernizr.com/) in your project - specifically, the [Flexbox feature detection](https://modernizr.com/download?flexbox-setclasses&q=flex), if you're using a custom build.

Tessellex relies on modernizr to feature-detect browsers that are flexbox-ready.
On these browsers, a `flexbox` class will be added to your root `<html>` element,
which will let Tessellex know it's cleared to work its magic.

If you're only interested in tailoring your grid to newer browsers, you could also
just omit modernizr and make sure one of your root elements (`html`, `body`, or a
similar page container) possesses the `flexbox` class.

### feature comparison table

| Feature | Traditional grid | Flexbox grid |
| --- | :---: | :---: |
| # columns | 6 | 6/12 |
| rtl/reverse | &#10004; | &#10004; |
| gutters | &#10004; | &#10004; |
| vertical alignment |   | &#10004; |
