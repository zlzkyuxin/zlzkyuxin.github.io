
**<center>中科云谷gatLab操作手册</center>**

1. 创建派生库(派生就是基于主库分化,类似于主分支和分支)
![主库](img/1596681300367.jpg "gitlab主库图片")
![派生库](img/1596681934035.jpg "gitlab派生库图片")

2. 将派生库clone到本地
> `git clone http://gitlab.zoomlion.com/yuxin/gitlab-demo.git`

![派生库](img/1596682203984.jpg "gitlab派生库图片")

3. 本地库关联主库
> `git remote add upstream http://gitlab.zoomlion.com/yx/gitlab-demo.git`

![关联主库](img/1596682520332.jpg "gitlab关联主库图片")

4. 将主库文件更新到本地(可能有其它同学更新内容合并到主库,所有合并操作前先将主库内容更新一下)
> `git pull upstream master`

5. 然后再将文件修改后先推送到派生库
>`git status` <br>
> `git add .` <br>
> `git commit -m '提交内容'` <br>
> `git push origin master` <br>

![推送到派生库](img/1596683324834.jpg "gitlab推送到派生库图片")

6. 在派生库中发起合并申请,并选择需要合并的分支
![派生库发起合并申请](img/1596683595820.jpg "gitlab派生库发起合并申请图片")
![派生库发起合并申请](img/1596683938909.jpg "gitlab派生库发起合并申请图片")
![派生库发起合并申请](img/1596684400509.jpg "gitlab派生库发起合并申请图片")

7. 等待主库管理员同意合并,同意后则完成合并请求 
![等待合并](img/1596684607870.jpg "gitlab等待合并图片")
![完成合并](img/1596684701442.jpg "gitlab完成合并图片")

8. 将合并变更信息更新到本地并推送到派生库
> `git pull upstream master` <br>
> `git push origin master` <br>


附图: git常用操作命令

![git常用操作命令](img/20190302200809745.png "git常用操作命令")
