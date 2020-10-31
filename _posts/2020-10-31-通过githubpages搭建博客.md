---
layout: post
title: githubpages搭建博客
categories: github

tag: github
---


# 使用git

## 1. 下载git

https://git-scm.com/download/win

## 2. 配置账户

打开git的控制台程序

![image-20201027205553631]({{site.baseurl}}/blogimg/image-20201027205553631.png)

输入下面的命令进行配置

```git
git config --global user.name "github的用户名"
git config --global user.email "github的邮箱"
```

使用下面的命令查看是否配置成功

```git
git cofig --global --list 
```



## 3. 生成ssh

```git
ssh-keygen -t rsa
```

然后一路回车键

会在命令行的根目录下生成ssh文件夹

<img src="{{site.baseurl}}/blogimg/image-20201027210214111.png" alt="image-20201027210214111" />

## 4. 将ssh中的公钥（id_rsa.pub）添加到github管理平台

### （1）创建新的ssh key

<img src="{{site.baseurl}}/blogimg/image-20201027212403163.png" alt="image-20201027212403163" style="zoom:67%;" />





![image-20201027212426042]({{site.baseurl}}/blogimg/image-20201027212426042.png)



![image-20201027212442972]({{site.baseurl}}/blogimg/image-20201027212442972.png)

### （2）将公钥添加进来

![image-20201027212637085]({{site.baseurl}}/blogimg/image-20201027212637085.png)



## 5. 测试是否配置成功

输入git命令进行测试

```git
ssh -T git@github.com
```

配置成功

![image-20201027213016144]({{site.baseurl}}/blogimg/image-20201027213016144.png)



# 将本地代码上传到github仓库

## 1. 建立git仓库

```git
git init
git status 查看目录下文件状态
```

![image-20201027213939938]({{site.baseurl}}/blogimg/image-20201027213939938.png)

## 2. 将项目的文件添加到待上传文件列表

```git
git add --all  将所有文件添加进待上传文件列表  git add  文件名 添加单个文件
git status
```



红色的文件会变成绿色

![image-20201027214240804]({{site.baseurl}}/blogimg/image-20201027214240804.png)



## 3. 将add的文件commit到仓库

```git
git commit -m "添加描述"
```

## 4. 在github上创建一个新的仓库

## 5. 将本地仓库关联到github

![image-20201027223200281]({{site.baseurl}}/blogimg/image-20201027223200281.png)

```git
git remote add origin git@github.com:WoodsonWang/Pyqt5.git
```

## 6. 上传代码到github仓库

```git
git push -u origin master
```



# 使用github创建博客

## 建立githubpages



![image-20201027224134442]({{site.baseurl}}/blogimg/image-20201027224134442.png)



选择一个主题



![image-20201027224155740]({{site.baseurl}}/blogimg/image-20201027224155740.png)

会等待很久。。。。。。

![image-20201027225606583]({{site.baseurl}}/blogimg/image-20201027225606583.png)

点击commit changes

然后就可以访问自己的网页了！！！ 

例如我创建的静态网页访问地址如下：

https://woodsonwang.github.io/Notes/





clone项目到本地

![image-20201027230551483]({{site.baseurl}}/blogimg/image-20201027230551483.png)

```git
git clone git@github.com:WoodsonWang/Notes.git
```



修改博客主题的方法

https://www.jianshu.com/p/418b5695e6ea





##  使用jekyll

### 1. 安装Ruby

下载安装exe，地址：http://rubyinstaller.org/downloads/

### 2.  安装jekyll

git bash中输入一下命令安装jekyll

```git
gem install jekyll

测试安装是否成功
jekyll -v
创建jekyll项目
jekyll new myblog
cd myblog
jekyll serve 启动服务，通过端口访问网站
```



![image-20201028005754837]({{site.baseurl}}/blogimg/image-20201028005754837.png)



### 3. 修改主题

主题下载  http://jekyllthemes.org/

本文使用的模板 https://leopardpan.cn/

下载一个主题



删除红线标记的文件



![image-20201028113619043]({{site.baseurl}}/blogimg/image-20201028113619043.png)



右键调出bash

![image-20201028102741243]({{site.baseurl}}/blogimg/image-20201028102741243.png)

输入命令，启动服务

```git
jekyll serve
```

若出现下面的问题

![image-20201028105831222]({{site.baseurl}}/blogimg/image-20201028105831222.png)

则输入命令

```git
bundle install
```

install完成之后，再启动服务

若还出现下面的问题

![image-20201028105927569]({{site.baseurl}}/blogimg/image-20201028105927569.png)

则要输入下面的命令启动服务

```git
bundle exec jekyll serve
```

服务启动成功

![image-20201028110355316]({{site.baseurl}}/blogimg/image-20201028110355316.png)

这样网站就可以成功访问了



路径问题

![image-20201028142101131]({{site.baseurl}}/blogimg/image-20201028142101131.png)

从浏览器中访问地址时，需要带上子路径Notes，因为项目的名字为Notes

修改_config.yml文件

![image-20201028100440122]({{site.baseurl}}/blogimg/image-20201028100440122.png)

![image-20201031203847646]({{site.baseurl}}/blogimg/image-20201031203847646.png)



在notepad++ 中编辑文件，进行路径的替换

![image-20201028142323258]({{site.baseurl}}/blogimg/image-20201028142323258.png)



##  评论系统

![image-20201028163825412]({{site.baseurl}}/blogimg/image-20201028163825412.png)



复制安装代码，替换掉comments.html 里section 标签中的代码即可使用了。

<img src="{{site.baseurl}}/blogimg/image-20201028164113305.png" alt="image-20201028164113305" style="zoom:80%;" />



## 写blog

在_posts文件夹下建立md文件

命名规则 '2020-11-11-文件名.md'

md文件头部须有下面的内容

```markdown
--- 
title: postName #文章页面上的显示名称，一般是中文 
date: 2013-12-02 15:30:16 #文章生成时间，一般不改，当然也可以任意修改 
categories: 默认分类 #分类 
tags: [tag1,tag2,tag3] #文章标签，可空，多标签请用格式，注意:后面有个空格 
description: 附加一段文章摘要，字数最好在140字以内，会出现在meta的description里面 ---
```

将项目push到github就可以访问了

