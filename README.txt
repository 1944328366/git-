版本管理方式
1：原始的版本控制（对整个项目源文件的拷贝）：浪费资源，无法进行协调开发，版本定位麻烦
2：集中式版本控制SVN
3：分布式版本控制git

git使用
1：配置全局账号
    git config --global username "你的git账号名"
    git config --global useremail "你的邮箱"
    查看：git config -l
2：创建一个目录
    mkdir 目录名
3：在该目录创建文件
    cd 目录名
    touch READEME.txt
5:编辑
    按Insert键 或 输入vi READEME 都可以进行编辑
    按ESC键 退出编辑
    ：wq 保存并退出
6：预览文件
    cat README.txt

7:项目初始化
    git init   
8：将更改的文件添加到暂存区
    git add README.txt
9：将暂存区的文件提交到本地仓库
    git commit -m "描述信息"
10：再次更改（编辑）
    vi README.txt
11:查看更改内容
    git diff
    8,9,10重复
12：查看提交日志
    git log
13:版本回退（HEAD当前版本 HEAD^上一个版本 HEAD^^上上个版本 HEAD~5上五个版本）
    git reset --hard HEAD^
14:版本回归
    git reset --hard 指纹信息（前几位数）

15：查看历史命令(根据指纹信息可以回退任意版本)
    git reflog
