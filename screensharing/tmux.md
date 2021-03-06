# 终端复用软件-tmux
## 应用场景介绍
### 1、在linux终端下需要开启多个窗口执行不同的任务而又不想每次都连接建立新的会话
### 2、建立linux连接后并执行一个长期任务不希望中途断掉，且该会话可永远保留随时连接
### 3、想要分享自己在终端操作的内容给其他同学
### 4、自己有个树莓派没有屏幕，想要通过浏览器解决显示的问题
>tmux可以满足以上4个场景，使得我们的工作方式得到极大的便捷，又好玩又好用
## 安装
```bash
sudo yum install tmux
```
## 使用
### 创建会话
```bash
$tmux new -s test -n test1 #创建一个会话名为test的窗口为test1的会话
```
### 退出并关闭会话
```bash
C+d
```
### 退出保留会话
```bash
<C+b> d
```
### 查看会话
```bash
$tmux ls
```
### 连接会话
```bash
$tmux attach -t test
```
### 删除会话
```bash
$tmux kill-session -t test
```
### 在会话中的操作手册<C+b> ?
- 在会话中创建窗口
- 在会话中分割窗口
- 在会话中关闭窗口
- 在会话中移动激活窗口
- 向会话执行命令
