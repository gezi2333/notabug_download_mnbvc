# notabug平台代码仓库下载

写在前边：本人计算机小白，只了解一点点基本的爬虫知识和python用法。代码写的可能不规范也不太完善，求各位佬轻喷。

## notabug简述

### 平台地址与基本情况

```
https://notabug.org/
```

NotABug.org is a free-software code collaboration platform for freely licensed projects. We exist to help projects that distribute under any free license.（来源自其[官网介绍](https://notabug.org/about)）

截至2023年10月24日，其共有仓库17936个。

### 爬取难度

notabug基本没有反爬措施，爬取难度较低，且其访问与下载不需要登录及cookie。

通过以下url即可提取得到其每页的仓库名

```
https://notabug.org/explore/repos?page=2&q=
```

通过以下url可提取得到单个仓库的.zip及.tar.gz的下载链接

```
https://notabug.org+仓库名
```

直接运行wget命令即可下载相应仓库。



所以，整体流程难度不高。

## 代码说明

所有代码都在.ipynb文件中，依次运行每个单元格即可。

其中，

01get_repo_name.ipynb 为获取仓库名的代码

02get_zip_url.ipynb 为获取各仓库下载链接的代码

03download_files.ipynb 为下载各仓库的代码



由于网络问题，可能部分片段需要不止执行一次，尤其是下载部分。