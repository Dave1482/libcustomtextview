# libcustomtextview
libcustomtextview
(NOT YET RELEASED)

This has a subclass for UITextView that allows customization for a selected string that appears in the UITextView, just replace your instance of UITextView with DTCustomTextView.

It may be possible to add your own subclasses to this GitHub, who knows, it may end up as part of the lib...

So far it only supports the system font, and cannot do both bold and italics on the same string.

Usage:
Add libcustomtextview.h and DTCustomTextView.h to iPhoneOSX.X.sdk/usr/include/libcustomtextview/
On Mac it'll usually be /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk/usr/include/libcustomtextview/
Add libcustomtextview.dylib to iPhoneOSX.X.sdk/usr/lib/
Mac xCode: /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk/usr/lib
Add libcustomtextview as a dependency for your package
Add libcustomtextview to your project's Frameworks

//Bolds string with boldSystemFontOfSize:16.0
[nameOfDTCustomTextView boldSubstring:@"String"];

//Bolds string with boldSystemFontOfSize:size (you choose the size)
[nameOfDTCustomTextView boldSubstring:@"String" ofSize:anyCGFloatValue];

//Bolds string with boldSystemFontOfSize:16.0 and colorWithRed:(you choose the red value) green:(you choose the green value) blue:(you choose the blue value) alpha:(you choose the alpha value)
[nameOfDTCustomTextView boldSubstring:@"String" colorWithRed:redCGFloatValue green:greenCGFloatValue blue:blueCGFloatValue alpha:alphaCGFloatValue];

//Bolds string with boldSystemFontOfSize:(you choose the size) and colorWithRed:(you choose the red value) green:(you choose the green value) blue:(you choose the blue value) alpha:(you choose the alpha value)
[nameOfDTCustomTextView boldSubstring:@"String" ofSize:anyCGFloatValue colorWithRed:redCGFloatValue green:greenCGFloatValue blue:blueCGFloatValue alpha:alphaCGFloatValue];

//italics string with italicSystemFontOfSize:16.0
[nameOfDTCustomTextView italicSubstring:@"String"];

//italics string with italicSystemFontOfSize:size (you choose the size)
[nameOfDTCustomTextView italicSubstring:@"String" ofSize:anyCGFloatValue];

//italics string with italicSystemFontOfSize:16.0 and colorWithRed:(you choose the red value) green:(you choose the green value) blue:(you choose the blue value) alpha:(you choose the alpha value)
[nameOfDTCustomTextView italicSubstring:@"String" colorWithRed:redCGFloatValue green:greenCGFloatValue blue:blueCGFloatValue alpha:alphaCGFloatValue];

//italics string with italicSystemFontOfSize:(you choose the size) and colorWithRed:(you choose the red value) green:(you choose the green value) blue:(you choose the blue value) alpha:(you choose the alpha value)
[nameOfDTCustomTextView italicSubstring:@"String" ofSize:anyCGFloatValue colorWithRed:redCGFloatValue green:greenCGFloatValue blue:blueCGFloatValue alpha:alphaCGFloatValue];
