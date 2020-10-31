---
layout: post
title: githubpages�����
categories: github

tag: github
---


# ʹ��git

## 1. ����git

https://git-scm.com/download/win

## 2. �����˻�

��git�Ŀ���̨����

![image-20201027205553631]({{site.baseurl}}/blogimg/image-20201027205553631.png)

��������������������

```git
git config --global user.name "github���û���"
git config --global user.email "github������"
```

ʹ�����������鿴�Ƿ����óɹ�

```git
git cofig --global --list 
```



## 3. ����ssh

```git
ssh-keygen -t rsa
```

Ȼ��һ·�س���

���������еĸ�Ŀ¼������ssh�ļ���

<img src="{{site.baseurl}}/blogimg/image-20201027210214111.png" alt="image-20201027210214111" />

## 4. ��ssh�еĹ�Կ��id_rsa.pub����ӵ�github����ƽ̨

### ��1�������µ�ssh key

<img src="{{site.baseurl}}/blogimg/image-20201027212403163.png" alt="image-20201027212403163" style="zoom:67%;" />





![image-20201027212426042]({{site.baseurl}}/blogimg/image-20201027212426042.png)



![image-20201027212442972]({{site.baseurl}}/blogimg/image-20201027212442972.png)

### ��2������Կ��ӽ���

![image-20201027212637085]({{site.baseurl}}/blogimg/image-20201027212637085.png)



## 5. �����Ƿ����óɹ�

����git������в���

```git
ssh -T git@github.com
```

���óɹ�

![image-20201027213016144]({{site.baseurl}}/blogimg/image-20201027213016144.png)



# �����ش����ϴ���github�ֿ�

## 1. ����git�ֿ�

```git
git init
git status �鿴Ŀ¼���ļ�״̬
```

![image-20201027213939938]({{site.baseurl}}/blogimg/image-20201027213939938.png)

## 2. ����Ŀ���ļ���ӵ����ϴ��ļ��б�

```git
git add --all  �������ļ���ӽ����ϴ��ļ��б�  git add  �ļ��� ��ӵ����ļ�
git status
```



��ɫ���ļ�������ɫ

![image-20201027214240804]({{site.baseurl}}/blogimg/image-20201027214240804.png)



## 3. ��add���ļ�commit���ֿ�

```git
git commit -m "�������"
```

## 4. ��github�ϴ���һ���µĲֿ�

## 5. �����زֿ������github

![image-20201027223200281]({{site.baseurl}}/blogimg/image-20201027223200281.png)

```git
git remote add origin git@github.com:WoodsonWang/Pyqt5.git
```

## 6. �ϴ����뵽github�ֿ�

```git
git push -u origin master
```



# ʹ��github��������

## ����githubpages



![image-20201027224134442]({{site.baseurl}}/blogimg/image-20201027224134442.png)



ѡ��һ������



![image-20201027224155740]({{site.baseurl}}/blogimg/image-20201027224155740.png)

��ȴ��ܾá�����������

![image-20201027225606583]({{site.baseurl}}/blogimg/image-20201027225606583.png)

���commit changes

Ȼ��Ϳ��Է����Լ�����ҳ�ˣ����� 

�����Ҵ����ľ�̬��ҳ���ʵ�ַ���£�

https://woodsonwang.github.io/Notes/





clone��Ŀ������

![image-20201027230551483]({{site.baseurl}}/blogimg/image-20201027230551483.png)

```git
git clone git@github.com:WoodsonWang/Notes.git
```



�޸Ĳ�������ķ���

https://www.jianshu.com/p/418b5695e6ea





##  ʹ��jekyll

### 1. ��װRuby

���ذ�װexe����ַ��http://rubyinstaller.org/downloads/

### 2.  ��װjekyll

git bash������һ�����װjekyll

```git
gem install jekyll

���԰�װ�Ƿ�ɹ�
jekyll -v
����jekyll��Ŀ
jekyll new myblog
cd myblog
jekyll serve ��������ͨ���˿ڷ�����վ
```



![image-20201028005754837]({{site.baseurl}}/blogimg/image-20201028005754837.png)



### 3. �޸�����

��������  http://jekyllthemes.org/

����ʹ�õ�ģ�� https://leopardpan.cn/

����һ������



ɾ�����߱�ǵ��ļ�



![image-20201028113619043]({{site.baseurl}}/blogimg/image-20201028113619043.png)



�Ҽ�����bash

![image-20201028102741243]({{site.baseurl}}/blogimg/image-20201028102741243.png)

���������������

```git
jekyll serve
```

���������������

![image-20201028105831222]({{site.baseurl}}/blogimg/image-20201028105831222.png)

����������

```git
bundle install
```

install���֮������������

�����������������

![image-20201028105927569]({{site.baseurl}}/blogimg/image-20201028105927569.png)

��Ҫ���������������������

```git
bundle exec jekyll serve
```

���������ɹ�

![image-20201028110355316]({{site.baseurl}}/blogimg/image-20201028110355316.png)

������վ�Ϳ��Գɹ�������



·������

![image-20201028142101131]({{site.baseurl}}/blogimg/image-20201028142101131.png)

��������з��ʵ�ַʱ����Ҫ������·��Notes����Ϊ��Ŀ������ΪNotes

�޸�_config.yml�ļ�

![image-20201028100440122]({{site.baseurl}}/blogimg/image-20201028100440122.png)

![image-20201031203847646]({{site.baseurl}}/blogimg/image-20201031203847646.png)



��notepad++ �б༭�ļ�������·�����滻

![image-20201028142323258]({{site.baseurl}}/blogimg/image-20201028142323258.png)



##  ����ϵͳ

![image-20201028163825412]({{site.baseurl}}/blogimg/image-20201028163825412.png)



���ư�װ���룬�滻��comments.html ��section ��ǩ�еĴ��뼴��ʹ���ˡ�

<img src="{{site.baseurl}}/blogimg/image-20201028164113305.png" alt="image-20201028164113305" style="zoom:80%;" />



## дblog

��_posts�ļ����½���md�ļ�

�������� '2020-11-11-�ļ���.md'

md�ļ�ͷ���������������

```markdown
--- 
title: postName #����ҳ���ϵ���ʾ���ƣ�һ�������� 
date: 2013-12-02 15:30:16 #��������ʱ�䣬һ�㲻�ģ���ȻҲ���������޸� 
categories: Ĭ�Ϸ��� #���� 
tags: [tag1,tag2,tag3] #���±�ǩ���ɿգ����ǩ���ø�ʽ��ע��:�����и��ո� 
description: ����һ������ժҪ�����������140�����ڣ��������meta��description���� ---
```

����Ŀpush��github�Ϳ��Է�����

