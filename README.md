项目地址: http://wiki.100ask.org/Ti437x


# 配置repo
## 下载repo
根据您的办公网络情况，从以下链接获取repo工具。
git clone https://gerrit.googlesource.com/git-repo (谷歌官方源)
git clone https://mirrors.tuna.tsinghua.edu.cn/git/git-repo (国内清华源) 
git clone https://gerrit-googlesource.lug.ustc.edu.cn/git-repo (国内中科大源)
## 配置REPO_URL
在到构建和谐社会的前提下，需要修改REPO_URL，可参考以下修改：

  vim repo

```
## REPO_URL = 'https://gerrit-googlesource.proxy.ustclug.org/git-repo'
REPO_URL = 'https://mirrors.tuna.tsinghua.edu.cn/git/git-repo/'
```

# 初始化仓库 repo init

新建目录存放仓库

```
$ mkdir -p ti437x
$ cd ti437x
$ repo init -u https://github.com/tinylaker/manifest -m default.xml --no-repo-verify
```

# 同步代码repo sync

```
$ repo sync -j4

```
# 代码目录
查看下载好的源码目录

