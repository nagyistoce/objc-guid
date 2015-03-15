# Introduction #

This ObjC implementation provides a type safe and efficient way to handle GUIDs/UUIDs within your app.

# Creating GUIDs #

```
// Empty guid
guid = [Guid emptyGuid];

// Random guid
guid = [Guid randomGuid];

// Guid from a string (returns nil if invalid)
guid = [[Guid alloc] initWithString:s];
```

# Converting Guids to strings #

```
s = [guid description];

s = [guid stringValueWithFormat:GuidFormatIncludeDashes];

s = [guid stringValueWithFormat:GuidFormatIncludeDashes | GuidFormatIncludeParenthesis];
```