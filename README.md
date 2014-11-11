js-dom-tools
============

JavaScript DOM tools library: collection of useful simple functions for interacting with the DOM

Vanilla JS

RequireJS AMD module

Mobile Ready : tested on Android 2.3, 4 + iOS 6, 8

Please test and report / fix if you see any "KO" in the test page

Features
========

* loadAsyncScript(src, id, callback)

Asyncronious javascript ressource loading into the document.body DOM page.
src: mandatory => source of the script to load.
id: optional => set the new script tag this id name
callback: optional => call this function when the script has been loaded

* loadAsyncScript(src, callback)

Asyncronious CSS files loading into the document.body DOM page.
src: mandatory => source of the CSS to load.
callback: optional => call this function when the script has been loaded

* findParentNodeWithNodeName(element, nodeName)

Returns the first DOM parent element from a child element, with this nodeName (ex: search 'div' parent of a "span" tag). Return null if not found.
element: mandatory => the child element
nodeName: mandatory => name of the parent node to find

* findParentNodeWithClassName(element, className)

Same as findParentNodeWithNodeName but using a className. (ex: search the first parent that has the '.pressed' class of a "span" tag)

* findParentNodeWithAttribute(element, attributeName)

Same as findParentNodeWithNodeName but using an attribute name. (ex: search the first parent that has the 'data-pressed' attribute of a "span" tag)

* objectTotalLength(object)

Return the lenght of this object/array/... if we can find a length.

* getOffsetSum(elem)

Get the offset position (top & left) of an element. Needs to process of the children to know this value...

* isEmpty(data)

Very handy function that prevent 'undefined' errors. Checks if any object given is not undefined, null, empty...

* getItemHeight(element), * getItemWidth(element)

Get the computed height / width of an element. Much faster than the jQuery equivalent.

