Ajax.js
=======

A useless and redundant library to make Ajax calls.

I got a little tired of loading all of jQuery/Prototype/mootools/...
just to do Ajax requests, but I also wanted something a little fancier than plain JS.
Hence Ajax.js, a simple, lightweight library to perform Ajax requests in a semi-chainable
manner.

Usage
-----

Include the library, then call it like this:

Simple Ajax Request
-------------------

```javascript
Ajax({ url : "http://target.url" });
```

Handling Responses
------------------

```javascript
Ajax({ url : "http://target.url" }).done(function(data) {
	
});
```

Sending Data
------------

```javascript
Ajax(
{
	url : "http://target.url",
	data : {
		"key" : "value"
	}
});
```

Mixing URL Parameters and Data
------------------------------

```javascript
Ajax(
{
	url : "http://target.url?parameter=value",
	data : {
		"key" : "value"
	}
});
```