# tmux-cheatsheet

[参考](https://gist.github.com/ryerh/14b7c24dfd623ef8edc7)

prefix: ctrl+b

## 窗口

```
c 创建新窗口
, 重命名
w 列出所有窗口
' 然后输入数字可以跳转到置顶窗口，这个功能主要用于窗口序号大于 10 的情况
  因为窗口序号大于 10 ，就不能用 `prefix + b + 数字` 跳转了
```

## 窗格

```
% 垂直分割
" 水平分割
q 显示窗格序号，再次输入对应序号后会切换到该窗格
z 窗格最大最小化
o 交换窗格
space 下一个布局
:setw synchronize-panes 同步窗格，在所有窗格中同步输入，再次执行则关闭同步
```

## 调整窗格尺寸

```
:resize-pane -D          当前窗格向下扩大 1 格
: resize-pane -U          当前窗格向上扩大 1 格
: resize-pane -L          当前窗格向左扩大 1 格
: resize-pane -R          当前窗格向右扩大 1 格
: resize-pane -D 20       当前窗格向下扩大 20 格
: resize-pane -t 2 -L 20  编号为 2 的窗格向左扩大 20 格
```
