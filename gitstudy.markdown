#### **一、创建版本库**

pwd 命令是用于显示当前的目录
git add readme.txt添加到暂存区里面，没有提示，添加成功
git commit -m “  ？？ ”
git status查看是否还有文件未提交(与git add直接相关)
git status查看结果
git diff readme.txt 查看readme.txt文件修改内容
提交修改和提交文件相同，git add然后git commit
git log查看历史记录

#### **二、操作修改**

1.放在暂存区的内容没有保存，可以直接文档修改，再commit

2.直接恢复到想要的版本：

git reset  –hard HEAD^ 回退到上一个版本，回退到上上个版本只需把HEAD^ 改成 HEAD^^ 
git reset  –hard HEAD~100
改变内容版本号为4566f，回到这一版本可用git reset  –hard 4566f

3.git checkout -- file 可以丢弃工作区的修改（此计算机版本用git checkout  file）

#### 三、文件删除

rm进行文件删除，用git checkout  file恢复文件

#### 四、远程仓库

文件共享？？？

创建艰难，一直显示没有.ssh，重新在目录里打开终端就可以了。

- 创建远程库：

```
git remote add origin https://github.com/z-zhou16/testgit.git
git push -u origin master
```

- 文件从本地到github



- 文件从github到本地

