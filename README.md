Example of Bundle Id warning - FB13704644

To reproduce:
1. Xcode 15.3 build 15E204a
2. Run from terminal: `xcodebuild -project SwiftNIOBundleIDWarning.xcodeproj -scheme SwiftNIOBundleIDWarningUITests build-for-testing -quiet`

3. You will see the warnings below:
```
warning: invalid character in Bundle Identifier. This string must be a uniform type identifier (UTI) that contains only alphanumeric (A-Z,a-z,0-9), hyphen (-), and period (.) characters. (in target '_NIODataStructures' from project 'swift-nio')
warning: invalid character in Bundle Identifier. This string must be a uniform type identifier (UTI) that contains only alphanumeric (A-Z,a-z,0-9), hyphen (-), and period (.) characters. (in target '_NIOBase64' from project 'swift-nio')
```
