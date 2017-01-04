# govips [![Build Status](https://travis-ci.org/h2non/bimg.svg)](https://travis-ci.org/h2non/bimg) [![GoDoc](https://godoc.org/github.com/davidbyttow/govips?status.svg)](https://godoc.org/github.com/davidbyttow/govips) [![Go Report Card](http://goreportcard.com/badge/davidbyttow/govips)](http://goreportcard.com/report/davidbyttow/govips) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

# A libvips library for Go
This package wraps the core functionality of [libvips](https://github.com/jcupitt/libvips) image processing library by exposing all image operations on first-class types in Go. Additionally, it exposes raw access to call operations directly, for forward compatibility.

How fast is libvips? See this: [Speed and Memory Use](http://www.vips.ecs.soton.ac.uk/index.php?title=Speed_and_Memory_Use)

This library was inspired primarily based on the C++ wrapper in libvips.

The intent for this is to enable developers to build extremely fast image processors in Go, which is suited well for concurrent requests. 

Libvips is generally 4-8x faster than other graphics processors such as GraphicsMagick and ImageMagick.

# Supported image operations
This library supports all known operations available to libvips found here:
- [VIPS function list](http://www.vips.ecs.soton.ac.uk/supported/current/doc/html/libvips/func-list.html)
- [VipsImage](http://www.vips.ecs.soton.ac.uk/supported/current/doc/html/libvips/VipsImage.html)
- [VipsOperation](http://www.vips.ecs.soton.ac.uk/supported/current/doc/html/libvips/VipsOperation.html)

# Requirements
- [libvips](https://github.com/jcupitt/libvips) 8+ (8.3+ recommended for GIF, PDF, SVG support)
- C compatible compiler such as gcc 4.6+ or clang 3.0+
- Go 1.4+

# Installation
```
go get -u gopkg.in/davidbyttow/libvips.v1
```

# Credits
Thank you to [John Cupitt](https://github.com/jcupitt) for maintaining libvips and providing feedback on govips.

# License
MIT - David Byttow
