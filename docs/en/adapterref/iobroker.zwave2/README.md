![Logo](admin/zwave2.svg)

# ioBroker.zwave2

[![NPM version](http://img.shields.io/npm/v/iobroker.zwave2.svg)](https://www.npmjs.com/package/iobroker.zwave2)
[![Downloads](https://img.shields.io/npm/dm/iobroker.zwave2.svg)](https://www.npmjs.com/package/iobroker.zwave2)
[![Dependency Status](https://img.shields.io/david/AlCalzone/iobroker.zwave2.svg)](https://david-dm.org/AlCalzone/iobroker.zwave2)
[![Known Vulnerabilities](https://snyk.io/test/github/AlCalzone/ioBroker.zwave2/badge.svg)](https://snyk.io/test/github/AlCalzone/ioBroker.zwave2)

[![NPM](https://nodei.co/npm/iobroker.zwave2.png?downloads=true)](https://nodei.co/npm/iobroker.zwave2/)

**Tests:**: [![Travis-CI](http://img.shields.io/travis/AlCalzone/ioBroker.zwave2/master.svg)](https://travis-ci.org/AlCalzone/ioBroker.zwave2)

## zwave2 adapter for ioBroker

Alternative Z-Wave implementation

## Changelog
<!-- 
	Placeholder for next versions:
	### __WORK IN PROGRESS__
-->

### 0.3.3 (2019-12-01)
* Updated `zwave-js` to v2.1.0. This includes the following changes:
	* Support for the `Meter CC`
	* Support for unsigned configuration parameters

### 0.3.2 (2019-11-28)
* Fixed a crash when property(Key) names contain weird punctuation

### 0.3.1
* Fixed a crash from v0.3.0

### 0.3.0
* Updated `zwave-js` to v2.0.0. For the full list of changes, see [here](https://github.com/AlCalzone/node-zwave-js/blob/master/CHANGELOG.md#200-2019-11-26). Notable improvements include:
	* Added configuration files for over 1000 devices. This improves support for some older devices and greatly improves the `Configuration CC`.
	* `Basic` CC is now hidden if a node support other Actuator CCs
	* Fixed `Binary Sensor` support
* Improved generation of state names for complex property names

### 0.2.1
* The network map now correctly displays the nodes' IDs

### 0.2.0
* Update `zwave-js` from v1.5.0 to v1.7.0. For the full list of changes, see [here](https://github.com/AlCalzone/node-zwave-js/blob/master/CHANGELOG.md#170-2019-11-03). Notable improvements include:
	* Complete `Multi Channel` support
	* Improved `Multilevel Switch` support
* improve value/metadata logging and change loglevel to debug
* use unit from value metadata
* use translated property keys to name states

### 0.1.3
* Update `zwave-js` dependency. Notable improvements include:
	* Support for `Time` and `Time Parameters` CCs. This automatically sets the correct time on supporting nodes.
	* Support for `Battery` CC v2
	* Cleanup of CC values
* Update misc. dependencies

### 0.1.2
* Several bugfixes and working admin menu

### 0.0.1
* initial release

## License
MIT License

Copyright (c) 2019 AlCalzone

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
