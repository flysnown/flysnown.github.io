# Mkdocs+github pages

如何部署建设自己的blog站
##mkdocs的安装

1. 首先安装[Python](https://www.python.org/)（目前mkdocs最高支持python3.8）
2. 安装pip（python3.8自带pip工具此步可省略）
3. 使用pip下载Mkdocs库，执行  
	
    pip  install  mkdocs  

## 下载git

访问[Git网站](https://git-scm.com/downloads)
下载最新的Git工具

## 创建自己的GitHub网站

### 创建自己的账号

访问[Github社区](https://github.com/)
创建自己的账号

### 创建自己的仓库


1. 在任何页面的右上角，使用+下拉菜单选择 New repository（新建仓库）。
	<center>
	![](/image/A1.png)
	</center>
2. 为仓库输入名称，建议使用<用户名>.github.io

	<center>
	![](/image/A2.png)
	</center>

3. （可选）添加仓库的说明。

	<center>
	![](/image/A3.png)
	</center>
4. 选择仓库可见性。 

	<center>
	![](\image\A4.png)
	</center>
5. 选择 Initialize this repository with a README（使用自述文件初始化此仓库）。

	<center>
	![](/image/A5.png)
	</center>
6. 点击 Create repository

	<center>
	![](/image/A6.png)
	</center>
7. 创建成功

### 上传SSH秘钥

1. 打开Git Bash
2. 输入以下内容  
	
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"** 

这将创建以所提供的电子邮件地址为标签的新 SSH 密钥。
3. 提示您“Enter a file in which to save the key（输入要保存密钥的文件）”时，按 Enter 键。 这将接受默认文件位置。
4. 在提示时输入安全密码。（可以不输）
5. 根据提示找到SSH秘钥生成位置，找到生成的.pub文件，用记事本打开，复制里面的全部内容
6. 登入GitHub网站，在页面的右上角，单击您的个人资料照片，然后单击 Settings（设置）

<center>
![](/image/A7.png)
</center>
7. 在用户设置侧边栏中，单击 SSH and GPG keys（SSH 和 GPG 密钥）。

<center>
![](/image/A8.png)
</center>
8. 单击 New SSH key（新 SSH 密钥）或 Add SSH key（添加 SSH 密钥）。

<center>
![](/image/A9.png)
</center>
9. 在 "Title"（标题）字段中，为新密钥添加描述性标签。

<center>
![](/image/A10.png)
</center>
10. 将密钥粘贴到 "Key"（密钥）字段。

<center>
![](/image/A11.png)
</center>
11. 单击 Add SSH key（添加 SSH 密钥）。

<center>
![](/image/A12.png)
</center>
12. 有可能会提示输入登入密码

## 编辑mkdocs

1. 打开Git Bash软件
2. 在本地合适的位置使用命令clone线上仓库到线下，输入：  
    git clone git@github.com:<用户名>/<用户名>.github.io.git  

此处建议使用SSHclone
3. 使用cd  <用户名>.github.io进去仓库
4. 创建文档项目，执行  

    mkdocs new <文件名>** 
 
执行完成后会在本地会生成一个文件夹，此文件夹中包含站点所有文件信息
5. 输入`cd 文件名`进入文件
6. 输入`mkdocs serve`站点开启成功后会的提示站点默认地址为：[https://127.0.0.1:8000](https://127.0.0.1:8000)
7. 在电脑上找到此文件夹，打开后找到一个以**docs**命名的文件夹，里面有一个index.md文件，编辑此文件可在[https://127.0.0.1:8000](https://127.0.0.1:8000)上显示。（此步不使用Git，以上步骤在Git Bash中完成）

##上传到GitHub



1. 打开Git Bash软件
2. 进入上步创建的mkdocs文件中
3. 在创建的mkdocs文件夹目录下生成站点文件，执行  

`mkdocs build`   

执行成功后会在本地文档项目文件夹中生成一个名为site的文件夹，site文件夹就是通过mkdocs编译生成的包含index.html的可被浏览器直接打开的静态前端站点
4. 进入site文件夹，将文件夹里的文件拷贝到git本地仓库中（此步需要手动实现）
5. 在本地git仓库先后执行
    
    git add -A  
    git commit -m "commit words"  
    git push  

  将本地仓库中的文件同步到github的main branch上
6. 此时通过*https://<用户名>.github.io*域名就可以访问到mkdocs静态网页站点
7. 使用这种方法每次更新本地站点文件需要手动同步一次到github上。


##参考来源

1. [简书](https://www.jianshu.com/p/b07dc1fd4f9e?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)
2. [Github Help](https://docs.github.com/cn)