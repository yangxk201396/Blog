# Blog

### 博客主页
    https://yangxk201396.github.io/Blog/
### 1. 创建博客
    hugo new site Blog
### 2. 下载主题
    cd Blog
    git init
    git remote add origin https://github.com/yangxk201396/Blog.git
    方法一:
    git clone https://github.com/adityatelange/hugo-PaperMod.git themes/hugo-PaperMod (--depth=1)
    从 themes/PaperMod 的 exampleSite 分支复制各个文件到 Blog 目录
    更新 .gitmodules 文件
    方法二:
    git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/hugo-PaperMod (--depth=1)
    (更新主题) git submodule update --remote --merge
### 3. 配置文件
    复制 Blog/themes/hermit/exampleSite/config.yml => Blog/config.yml
    配置文件 config.toml 中添加 publishDir = docs
### 4. 添加文章
    hugo new about/_index.md
    hugo new posts/my-first-post.md
### 5. 生成 docs 静态文件
    hugo