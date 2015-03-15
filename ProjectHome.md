A straight forward and fast type-safe Guid/UUID class for Objective C.  GUID generation is accurate (it uses CFUUIDCreate).

Never use inefficient and type-unsafe strings for GUIDs again!

Obj-guid uses [ARC](http://clang.llvm.org/docs/AutomaticReferenceCounting.html) so that needs to enabled in Xcode/llvm.

```
// Parse a GUID from string
Guid* guidFromString = [[Guid alloc] initWithString:@"21EC2020-3AEA-1069-A2DD-08002B30309D"];

// Create a random GUID
Guid* randomGuid = [Guid randomGuid];

// Convert a GUID to a string
NSString* guidString = [randomGuid stringValueWithFormat: GuidFormatDashed];
```


Browse the header: [Guid.h](http://code.google.com/p/objc-guid/source/browse/Guid.h)

Browse the source: [Guid.m](http://code.google.com/p/objc-guid/source/browse/Guid.m)

[Download the latest release](http://code.google.com/p/objc-guid/downloads/list)