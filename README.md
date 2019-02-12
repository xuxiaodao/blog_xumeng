# blog_xumeng

如果喜欢本网站，请动动手指 [Star](https://github.com/a88053443/blog_xumeng/stargazers) 支持一下



> 如果没有更改过主题源文件,也不需要代码优化可以跳过1,2,3步骤


1. gulp打包构建，拷贝主题目录下`package.json`文件到Hexo根目录下，然后安装项目的开发依赖。  [Gulp入门指南](http://www.gulpjs.com.cn/docs/getting-started/)
``` bash
npm i   //安装项目依赖
```

2. 在Hexo根目录下创建一个名为 gulpfile.js 的文件：
``` bash
require('./themes/hexo-theme-snippet/gulpfile');
```

3. 运行 gulp：
``` bash
gulp 或者 gulp default   //执行打包任务
```

4. 清空hexo静态文件和缓存，并重新生成
``` bash
hexo clean && hexo g  //清空缓存并生成静态文件
```

5. 本地预览，确没有问题再进行发布
``` bash
hexo s -p 4000 或者 hexo s  //启动本地服务默认
```

6. 当gulp执行完成，并提示  `please execute： hexo d` 时，可以进行发布
``` bash
hexo d 或者 gulp deploy  //部署发布
```

