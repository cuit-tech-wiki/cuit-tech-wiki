## 使用方法（超级精简版，后续完善）

推荐 Git 学习地址：https://www.liaoxuefeng.com/wiki/896043488029600

Bilibili视频讲解地址：https://www.bilibili.com/video/BV1Fg41137qG/



①fork项目建立 git 仓库（必须要递归拉取，否则无法获得子模块）

```
git clone  --recursive https://github.com/cuit-tech-wiki/cuit-tech-wiki/ 
```

②安装依赖文件

```
pip install -r mkdocs-material/requirements.txt
```

③启动服务器实时渲染

```
mkdocs serve
```

④编译完成后Build项目

```
mkdocs build
```

⑤上传项目文件

```
mkdocs gh-deploy --force
git add .
git commit -m "描述"
git push origin master
```



将要添加至 Wiki 的 Markdown 文件保存至  **docs** 下的文件夹中，然后修改 `mkdocs.yml` 中的 **nav** 属性

