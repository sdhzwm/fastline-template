# fastlane-template

## 安装

如果没有之前从没安装过 `Fastlane` ,可参考  [install fastlane](https://docs.fastlane.tools/getting-started/ios/setup/) 。或者按照如下步骤：

### 1. 安装ruby

```ruby
    brew update
    brew install ruby
```

### 2. 安装 fastlane


```ruby
brew install fastlane
```
或者

```ruby

sudo gem install -n /usr/local/bin fastlane

```

### 3. 使用 fastlane-template

把本工程下的 fastlane 文件 copy 到 所需项目的主工程即可

### 后续后维护具体模板 考虑其复用性

```ruby
import_from_git(url: 'http://172.16.69.171/ios/iosCom/Templates/fastlane-templates', branch: 'master')
```

## 使用

### 发布 私有 pod 库

进入项目的跟目录，然后在终端输入以下命令:

```bash

$ fastlane czpod version:"new version"

```

### 发布自定义 repoName 到 私有库

```bash
$ fastlane czpod repoName:"XXXSpecs" version:"new version"
```

### 可选参数

如果需要添加提交信息，可以添加此参数:

```bash
$ fastlane czpod version:"new version" desc:"commit information"
```


> 注意： **version 等同于 tag **

## License

Fastlane-files is available under the MIT license. See the LICENSE file for more info.
