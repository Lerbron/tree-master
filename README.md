# learn git subTree

## 添加子仓库
```bash
  git subtree add --prefix=sub1 git@github.com:Lerbron/tree-sub1.git master --squash
```
--prefix：添加子仓库的名字/路径；
子仓库的地址
需要添加的分支
--squash: 不拉取历史信息，而只生成一条commit信息

## 简化git subtree命令
```bash
git remote add -f sub1 git@github.com:Lerbron/tree-sub1.git
```
将子仓库的地址作为一个remote，并取名为sub1

## 从源仓库拉取更新
```bash
git subtree pull --prefix=sub1 git@github.com:Lerbron/tree-sub1.git master --squash
```
or
```bash
git subtree pull --prefix=sub1 sub1 master --squash
```
拉取子仓库地址为git@github.com:Lerbron/tree-sub1.git中master的更新至本地sub1

## 在主仓库中修改，并推送到源仓库
git subtree push --prefix=sub1 sub1 master



