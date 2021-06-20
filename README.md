[howiechen95.github.io](http://howiechen95.github.io)

node version : 13    
install hexo
```
npm install -g hexo-cli
npm install hexo
```

change themes
```
git clone -b master https://github.com/jerryc127/hexo-theme-butterfly.git themes/butterfly

npm install hexo-renderer-pug hexo-renderer-stylus
```

update  _config.yml
```
theme: butterfly
```

run
```
hexo clean && hexo generate && hexo server
```

themes
* [butterfly](https://github.com/jerryc127/hexo-theme-butterfly.git)
* [yilia](https://github.com/litten/hexo-theme-yilia)
* [cafe](https://github.com/giscafer/hexo-theme-cafe)


* [travis-ci自动部署](https://lanlan2017.github.io/blog/13f63c39/)
* [Hexo博客多主题自动部署方案](https://www.jianshu.com/p/f8ffcd755e7a)