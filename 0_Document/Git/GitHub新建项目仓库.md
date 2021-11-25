# GitHub新建项目仓库

## 将本地已存在仓库推送到远程新建仓库

```bash
git remote add origin git@github.com:727997856/ProjectName.git
git branch -M master
git push -u origin master
```

## 创建新仓库同步到远程新建仓库

```bash
echo "# ProjectName" >> README.md
git init
git add README.md
git commit -m "init commit"
git branch -M master
git remote add origin git@github.com:727997856/ProjectName.git
git push -u origin master
```

## 本地初始化Git及同步远程仓库

```bash
git init
vim .gitignore
git add .
git status
git commit -m "Commit Comments"
git branch --set-upstream-to=origin/master master
git branch -M master
git push -u origin master
git pull
git push
```
