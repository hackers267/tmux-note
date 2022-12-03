# Open

插件`Open`是tmux中打开高亮的文件或链接的一个插件。

## 安装

安装`open`插件，可以在`.tmux.conf`文件中添加以下内容，以使用`Tmux Plugin Manager`安装。
```shell
set -g @plugin 'tmux-plugins/tmux-open'
```
然后，使用`prefix+I`来完成安装就行。

## 使用

在安装成功了`tmux-open`后，就可以使用这个插件来打开高亮的文件或链接了。在这个时候，只要在要选择的文件或链接，再使用快捷键`o`就可以使用对应的程序打开文件或链接了。

## 配置

如果有修改配置的需要，可以以下面的方式修改`.tmux.conf`文件，默认文件是`~/.tmux.conf`。

把默认的快捷键*o*修改为*x*:
```shell
set -g @open 'x'
```
把默认的快捷键*ctrl+o*修改为*o*:
```shell
set -g @open-editor 'ctrl+x'
```
修改搜索引擎:
```shell
set -g @open-S 'https://www.bing.com/search?q='
```
使用多个搜索引擎：
```shell
set -g @open-B 'http://www.bing.com/search?q='
set -g @open-S 'http://www.google.com/search?q='
```
