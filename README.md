# 关于iOS代码风格管理的两三事
<div align=center>
<img src="http://images.bookuu.com/book/C/01400/97871113854482294829-fm.jpg" width = "300" height = "400" alt="代码风格的两三事儿" />
</div>

## 安装

打开终端执行命令:

    curl -ssl https://raw.githubusercontent.com/youngshook/objc-format-check/master/format-check.sh|bash


安装过程首先 format-check 会 clone 下来一个[工具](https://github.com/youngshook/objc-format-check)（这里参考了Space Commander）放在.format-check目录，然后执行我们的工具。
工具主要干了两件事：
  1. 拷贝 `.clang-format` 代码风格约束文件至项目根目录
  2. 给 Git 添加 pre-commit 脚本，使之每次执行 git commit 操作之前进行代码风格检查。

## 卸载
打开终端执行命令:

	curl -ssl https://raw.githubusercontent.com/youngshook/objc-format-check/master/uninstall.sh|bash

## 定制代码风格
默认安装使用项目中的 `.clang-format` 文件, 安装完成后会自动拷贝进项目根目录。
定制代码风格的话只需要修改和 `.git` 同目录下的 `.clang-format` 文件，具体的规则可以参考 [这个](http://clangformat.com/)。

