## 让你的PC具备推送的功能
2017年11月19日，我在学习git指令

git config --global user.name "xiaoxiaohanhanhan"

git config --globa user.email "627342660@qq.com"
 
ssh-keygen -t rsa -b 4096 -C "627342660@qq.com"

cat ~/.ssh/id_rsa.pub

通过网页，添加你的ssh

## 添加远程仓库的信息
git remote add origin git@github.com:xiaoxiaohanhanhan/maven_repository.git

## 删除远程仓库的信息
git remove remove

## 查看远程仓库的信息
git remote -v

如果是git clone git@github.com:xiaoxiaohanhanhan/gitStuy.git 下来的，自动绑定了远程仓库

root@liuruohan-Inspiron-5447:~/gitStuy# git remote -v

origin  git@github.com:xiaoxiaohanhanhan/gitStuy.git (fetch)

origin  git@github.com:xiaoxiaohanhanhan/gitStuy.git (push)


git remote remove origin

git remote add origin git@github.com:xiaoxiaohanhanhan/gitStuy

git push -u origin master

git push

## mahua.jser.me

		格式

## 如何把一个本地工程demo添加到github上
1. 在你的github账号上，添加你电脑的ｓｓｈ信息,让你的PC具备推送的功能

2. 在你的文件夹下面

		cd demo

		git init

		git add .

		git commit -m "第一个版本"

		（可添加多个对应远程仓库，git remote -v 查看）

		git remote add origin git@github.com:xiaoxiaohanhanhan/demo.git

		git push -u origin master (第一次)

		git push (后面默认用第一次那个)


## 如何在github上已有的工程上接着开发
1. 在你的github账号上，添加你电脑的ｓｓｈ信息,让你的PC具备推送的功能

		git clone git@github.com:xiaoxiaohanhanhan/demo.git(如果之前已经下载可以跳过此步，但必须保证本地文件与远端同步！)
		
		cd demo

		(做你的修改)

		git add .

		git commit -m "提交说明"

		git push				


## vim .gitignore 忽略你的文件,不管你了
		
		#忽略以～结尾的文件
		*~

## 从工程中删除文件

		rm 你要删除的文件
		git rm 你要删除的文件
		git commit -m "删除文件"
		git push
