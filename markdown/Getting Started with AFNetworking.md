# Getting Started with AFNetworking

## Step 1: 下载 CocoaPods

CocoaPods 是一个负责管理 iOS 项目中第三方开源代码的工具，可以使类似 AFNetworking 这样的第三方类库自动化和简单化。

CocoaPods 作为一个 Ruby gem 分发，它的可以通过命令行的方式在**终端**中安装。

```
$ sudo gem install cocoapods
$ pod setup
```

> 根据你 Ruby 的设置，你可以不需要使用 **sudo** 来安装 CocoaPods gem。

## Setp 2: 创建一个 Podfile

CocoaPods 指定一个叫做 **Podfile** 的文件来管理项目依赖包。 在你的 Xcode 项目 (.xcodeproj) 的目录中创建这个文件。

```
$ touch Podfile
$ open -a Xcode Podfile
```

创建成功后使用 Xcode 打开。

复制以下命令到 TextEdit 窗口:

```
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '7.0'
pod 'AFNetworking', '~> 2.5'
```

> 不要使用 TextEdit 来编辑 pod 文件，这将导致 CocoaPods 发生错误。请使用 Xcode 或其他编辑器来进行编辑。

## Step 3: 安装依赖包

在你的项目中按照依赖：

```
$ pod install
```

到这里，一定要确保一直打开 Xcode 的工作区 (.xcworkspace) 而不是项目文件当你编译你的项目时:

```
$ open <YourProjectName>.xcworkspace
```

## Step 4: 尽情享用吧！

到此为止，所有的准备工作都已经准备完成。只需要在需要的地方导入 **AFNetworking** 的头文件就可以使用了！




