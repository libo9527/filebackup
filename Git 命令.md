## Git 

> [廖雪峰的 Git 教程](<https://xiaosheng.me/ebook/git-tutorial/index.html>)

### rm

> [git rm命令 - 删除文件- 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013758392816224cafd33c44b4451887cc941e6716805c000)

- 从版本库中删除该文件

  ```shell
  git rm test.txt
  ```

  

### checkout

- 还原文件

  ```shell
  git checkout -- test.txt
  ```

  `git checkout`其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”

### 处理 Git 忘记切分支修改了代码的情况

> [处理Git 忘记切分支修改了代码的情况- 致力打造Yii 中国第一社区](https://getyii.com/topic/240)

```shell
git stash

git branch ...

git stash apply
```

