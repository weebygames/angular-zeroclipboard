# Angular ZeroClipboard

An angular wrapper for ZeroClipboard

## Install

```
bower install angular-zeroclipboard
```

or, you can download 'angular-zeroclipboard.js' form 'src' manualy

## Setup

#### sample

```
angular.module('demo', ['angular.zeroclipboard']).
  config(['uiZeroclipConfigProvider', function(uiZeroclipConfigProvider) {

    // config ZeroClipboard
    uiZeroclipConfigProvider.setZcConf({
      moviePath: '../bower_components/zeroclipboard/ZeroClipboard.swf'
    });

    // set directive options
    uiZeroclipConfigProvider.setOptions({
      buttonText: 'Copy Me!'
    });

  }]);
```


## Config

* `uiZeroclipConfigProvider.setZcConf({})` Config the ZeroClipboard

The params is an object. and just same as [ZeroClipboard official config](https://github.com/zeroclipboard/zeroclipboard/blob/1.x-master/docs/instructions.md)

* `uiZeroclipConfigProvider.setOptions()` Config this directive Config

```
{
    // set the button class
    buttonClass: '',

    // set button's Text
    buttonText: 'Copy',

    // set the callback function of the events which ZeroClipboard dispataches
    load: null,
    mouseover: null,
    mouseout: null,
    mousedown: null,
    mouseup: null,
    complete: null,
    noflash: null,
    wrongflash: null,
    dataRequested: null
}
```

## LICENSE

Copyright (C) 2014 lisposter(Leigh Zhu)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
