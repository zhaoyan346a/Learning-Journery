# Git是分布式版本控制系统，CVS和SVN都是集中式版本控制系统。
# 集中式版本控制系统：版本库是存放在中央服务器的，工作时要先从中央服务器获取最新版本，自己修改完后再上传到中央服务器，是必须要联网才能完成这项工作的。而且如果中央服务器出了问题，那大家都不能工作了。
分布式版本控制系统：没有中央服务器，每个人的电脑都是一个完整的版本库，更安全，多人合作时只需要把修改的文件推给对方让其看到即可。
1、安装Git
windows平台安装git后，还要输入
git config --global user.name "Your Name"
git config --global user.email "Your email"
这是为了给自己电脑添加一个标识。
在本机上查看名字和邮件：git config user.name   git config user.email
2、创建版本库
2.1  创建一个空目录  
2.2  用git init 把这个目录变成Git可以管理的仓库
注意：Windows平台下不要用自带的记事本，使用Notepad++，默认编码改为UTF-8 without BOM
2.3  用git add 命令添加文件(可多次添加)
git add file.txt   //添加file.txt或修改file.txt为可提交状态
(git reset file.txt //修改file.txt为不可提交状态)
git add file1.txt file2.txt   //添加file1.txt和file2.txt
git add .  //添加所有新添加的文件
2.4  用git commit -m "注释" 命令提交文件
git commit -m "wrote a file" //提交file文件到仓库
