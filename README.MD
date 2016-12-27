# viewport-overlap-checker 

[![NPM](https://nodei.co/npm/easy-promise-queue.png)](https://nodei.co/npm/easy-promise-queue/)
> Easy promise queue. Set a concurrency to execute promises in the queue.

[![Build Status](https://travis-ci.org/chenzhihao/easy-promise-queue.svg)](https://travis-ci.org/chenzhihao/easy-promise-queue)

## Installation
```bash
$ npm install easy-promise-queue
```

## Usage

### Check if an element is totally in viewport
```js
import {isElementFullyInViewport} from 'viewport-overlap-checker';

const image = document.getElementById('img');

isElementFullyInViewport(image);
// true
```
![](//i.imgur.com/JMT7ACYg.png =600x)
 
 
### Check if an element is totally in viewport
```js
import {isElementFullyInViewport} from 'viewport-overlap-checker';

const image = document.getElementById('img');

isElementFullyInViewport(image);
// true
```
![](http://i.imgur.com/JMT7ACYg.png =600x)

### Check if an element is overlap with viewport
```js
import {isElementPartInViewport} from 'viewport-overlap-checker';

const image = document.getElementById('img');

isElementPartInViewport(image);
// true
```
![](http://i.imgur.com/gETmAW3.png =600x)

### Check if an element is close to viewport
```js
import {isElementCloseToViewport} from 'viewport-overlap-checker';

const image = document.getElementById('img');

isElementCloseToViewport(image, {top: 10});
// true

// this means the margin between top of element and bottom of viewport is no more than 10px;

// if we used it like isElementCloseToViewport(image, {top: 10, left: 20});
// this means the left of element is close to left of viewport in 20px AND top is close to bottom
// of viewport in 10px.

// Trikcy: the {top, bottom, left, right} values can be negative so you can restrict 
// the element is in center of viewport.

```
![](http://i.imgur.com/P3x2ul7.png =600x)

## License
[MIT](https://tldrlegal.com/license/mit-license)