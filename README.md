# Buildsystem

This is a c++ buildsystem for compiling c++ files with g++ on an OSX/macOS machine.

  

1) put stdc++.h into:

/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/*ChosenMacOSSDK*/usr/include/bits.

Note: if there is no bits directory in your "include" create one yourself.

2) At the top of your c++ files use like so:  ```#include <bits/stdc++.h>```

gpp.sublime-build is a plain build system that compiles to the directory of your c++ file and creates a binary with the same name of your c++ file, whereas gppB.sublime-build is one that allows you to read from stdin and output to stdout. You need to create the ```output.in``` and ```input.in``` files in the directory of your c++ files.

3) To hook  gpp.sublime-build with SublimeText IDE, Navigate to Prefrences > Browse Packages 
and copy your preferred gpp.sublime-build to /User directory.

4) Restart Sublime Text and select Tools > Build System and  select your newly added gpp / gppB.

See [Documentation Thread](https://codeforces.com/blog/entry/47152) for more info : 



