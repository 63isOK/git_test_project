# git_test_project
学习git时，用到的测试项目

## 测试免密使用github

## git 介绍

- git保存数据，更像一个快照流
- 所有操作都是本地操作，所以非常快
- 一般情况，git只添加数据，因为很多操作都有可逆操作对应，
很难出现要清数据的情况


  git的三种状态：
- committed，数据已提交到本地仓库
- modified，数据未提交到本地仓库
- staged，数据做了标记，下次提交将数据包含在快照中


  git有3个工作区域：
- 本地仓库 .git目录
- 工作目录 一般是checkout的目录
- 暂存区 一个文件保存了提交索引


  git的工作流程：
- 工作区修改文件
- 暂存文件，将暂存文件的快照放到暂存区域
- 提交更新

  git配置优先级：
- .git/config  优先级最高
- ~/.gitconfig ~/.config/git/config 
- /etc/gitconfig 优先级最低

  用户信息很重要，因为每次提交都会带上
可通过上面的配置设置  
  git config --list 查看配置

## git 的基础操作

### 获取git仓库
  有两种方式在本地创建仓库：
- 克隆已有仓库
```shell
    git clone url abc # abc是本地仓库的名字，可以省略
```
- 在指定目录初始一个仓库
```shell
    git init  # 初始化一个本地仓库
    git add .
    git commit -m "init" # 如果目录下有文件，添加到仓库
```

  git传输协议支持https git ssh

  工作目录下的文件状态

