
# theos with podfile


本项目旨在探索在theos中使用cocoapods集成库以工theos使用。


传统的办法是新建xcode项目，编译为framework复制回来。

这里使用 `integrate_targets` 不创建新的xcode项目。

```
```bash
pod install
```
然后我们执行
```bash
❯ xcodebuild -project Pods/Pods.xcodeproj -configuration Debug
```
```
```

即可编译出.a 静态库，后续放入 `$THEOS`/lib 继续使用。



也许有更简单的办法？
