# context-manager [![NPM version](https://badge.fury.io/js/context-manager.png)](http://badge.fury.io/js/context-manager)

> Manage context for templates.

## Install
#### Install with [npm](npmjs.org)

```bash
npm i context-manager --save
```

## Usage

```js
var context = require('context-manager');
```

## API
### Context


Create an instance of `Context`.


### add

Add a context level, optionally passing a value to start with.

* `type` **{String}**: The kind of context to add.  
* `level` **{Number}**: Numerical value representing the order in which this level should be merged versus other levels.  
* `value` **{Object}**: Optionally pass a starting object.  

```js
context.add('locals', {a: 'b'});
```


### get

Return the context for `type`.

* `type` **{String}**: The context type to get.  
* returns: {*}  

```js
context.set('a', {a: 'b'});
context.get('a');
// => {a: 'b'}
```


### setLevel

Set the level (number) for the specified context `type`.

* `type` **{String}**: The context type to get.  
* returns **{Number}** `num`  

```js
context.set('a', {a: 'b'});
context.get('a');
// => {a: 'b'}
```


### getLevel

Get the level (number) for the specified context `type`.

* `type` **{String}**: The context type to get.  
* returns: {Number}  

```js
context.setLevel('a', 1);
context.getLevel('a');
// => '1'
```


### extend


Extend the context.


### extend


Extend the context.


### calculate


Calculate the context


### reset


Remove a context.


### remove


Remove a context.


### clear


Clear all contexts.

## Author

**Jon Schlinkert**
 
+ [github/assemble](https://github.com/assemble)
+ [twitter/assemble](http://twitter.com/assemble) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on August 15, 2014._