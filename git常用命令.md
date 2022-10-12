# stash

版权声明：本文为CSDN博主「淹不死的水」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/stone_yw/article/details/80795669

## $ git stash

```sh
$ git stash
Saved working directory and index state WIP on master: b2f489c second
```

## $ git status

```shell
$ git status
On branch master
nothing to commit, working tree clean
```

> git stash的效果：
> `stash@{0}: WIP on master: b2f489c second`
> git stash save “test1”的效果：
> `stash@{0}: On master: test1`

## $ git stash list

查看当前stash中的内容

## $ git stash pop

将当前stash中的内容弹出，并应用到当前分支对应的工作目录上。
注：该命令将堆栈中最近保存的内容删除（栈是先进后出）