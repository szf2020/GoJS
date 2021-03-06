This demonstrates how to build a diagram with GoJS source, using webpack.

Because Webpack is able to shake out all functionality not used, this Diagram is truly minimal, and the compiled JS contains no layouts, no GoJS Tools for interactivity, no TreeModel or GraphLinksModel, no SVG rendering capability,

There are many related projects in this directory:

* **minimalSource**, for an example of building GoJS while excluding as many modules as possible. This project uses webpack's tree shaking to remove unused modules.
* **maximalSource**, for an example of building GoJS while including every module.
* **minimalSourceBrowserify**, for another minimal example of building GoJS with Browserify. Also does not use `require`.

With npm, install the dependencies:

```
$ npm install
```

You may also need to install `webpack` globally. Run script with:

```
$ webpack
```

This creates `maximal.js`, which is referenced in `maximal.html`.
