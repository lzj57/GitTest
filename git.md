## git

+ 初始化git目录仓库

  init后出现.git文件夹，文件夹中存在4个文件夹和3个文件

  - hooks/ 包含客户端和服务端的钩子脚本
  - info/ 包含一个全局性排除文件，用于记录在.gitignore文件中的忽略模式
  - objects/ 存储所有数据内容
  - refs/ 存储指向数据提交的对象的指针
  - config 项目的配置选型
  - description 仅供gitweb程序使用
  - HEAD 指示目前被检出的分支

+ git clone
  
- git clone [url]克隆已有仓库，可以利用git clone [url] [mygitName]克隆项目并将本地克隆项目命名为mygitName。
  
+ git add 还用于合并时，把有冲突的文件标记为已解决状态。

+ 利用.gitignore文件忽略部分文件，文件的格式规范
  - #和空行会被忽略
  - 可以使用标准的glob（shell使用的简化正则表达式）
  - 匹配模式可以以/开头防止递归，以/结尾指定目录
  - 要忽略指定模式以外的文件或目录，可以在模式前加上惊叹号(!)取反。

+ git diff 显示尚未暂存的改动，而不是自上次提交以来所做的所有改动。

	git diff --cached 和git diff --staged可查看暂存的改动

+ git commit -a -m "" ，可以直接跳过git add 操作，直接进行提交
