# swift-android-trace

C-wrapper for Android Trace utility (trace.h, systrace) for Swift.

## Getting started

Read [Android Native Trace](https://developer.android.com/ndk/guides/tracing.html)

## Installation

 .Package(url: "https://github.com/yuryybk/swift-android-trace.git", .branch("master"))
 
## Usage
 

### Code Example 
 
 ```
 import AndroidSwiftTrace
 
 .....
 
 public func helloWorld() {
    beginSection("Hello")
    
    ....
    
    endSection()
 }
 ```
 
 ### Generate report
 
 Run application. To get .html report run the next command and play with application:
 
 `python $ANDROID_NDK/platform-tools/systrace/systrace.py --time=<trace_duration_seconds> --app=<app_package> -o <output_dir> app`
 
 ## License

This project is licensed under the Apache 2.0 LICENSE - see the [LICENSE.md](LICENSE.md) file for details

