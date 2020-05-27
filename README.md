# learn git subTree

## 添加子仓库
```bash
  git subtree add --prefix=sub1 git@github.com:Lerbron/tree-sub1.git master --squash
```
--prefix：添加子仓库的名字/路径；
子仓库的地址
需要添加的分支
--squash: 不拉取历史信息，而只生成一条commit信息
