# What is mniobj ?
mniobj is a 3D mesh file specification made by Montreal Neurological Institute. We use it mainly within [BrainBrowser](https://brainbrowser.cbrain.mcgill.ca) because it is convenient and simple to use to load 3D shapes in webGL.

# What is mniobjReader ?
It's a reader and parser for mniobj files in Javascript (browser) with no dependencies. The parsed data format is intentionally left relatively raw, mainly using typed arrays. Having no dependencies makes it easier to run the parsing from within a web worker.  
In the following, examples are given for both the mono-thread **and** the web-workers way of loading mniobj files.

# How to use it ?
In the following examples, you have to open the JS console to see what's happening. (nothing is *printed* onto the page.)
## The almost sync way (no web workers)
See `simple.html`.

## The very async way (with web workers)
See `simpleWorker.html`.

# How to actually display something?
Here, we are using [ThreeJS](https://threejs.org) to display the parsed mniobj.
## The almost sync way (no web workers)
See `shape.html`.

## The very async way (with web workers)
See `shapeWorker.html`.

# License
MIT
