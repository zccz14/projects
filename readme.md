# Projects

突然想到可以用 Git Submodule 来管理我的所有项目，于是就这样试试看，意外地好用呢。

这样就可以跨设备管理我的项目了。

当我到一台新的电脑上，安装完必要的工具(Git)以及配置(SSH)以后，克隆这个项目就可以克隆我所有的项目。

```bash
$ git clone git@github.com:zccz14/projects.git
```

当然这个时候子项目们都还是空的，我可以按需要克隆，毕竟没必要把所有的都弄下来嘛。

然后我可以按项目克隆我需要的项目：

```bash
$ git submodule init zccz14.com # init git repo
$ git submodule update zccz14.com # update submodule from remote
```

简直excited！

要导入新的项目到我的项目集合里来的话，只需要：

```bash
$ git submodule add <RepoURI>
```

这样就可以把 RepoURI 对应的项目添加进项目集合了。

详情参见帮助文档：

```bash
$ git help submodule
```

如果有更有趣的应用请分享给我！