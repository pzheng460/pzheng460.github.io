---
title: hexo指南
date: '2023-10-04'
summary: hexo使用
---

# 命令
```
npm install hexo -g #安装Hexo  
npm update hexo -g #升级  
hexo init #初始化博客  
  
命令简写  
hexo n "我的博客" == hexo new "我的博客" #新建文章  
hexo g == hexo generate #生成  
hexo s == hexo server #启动服务预览  
hexo d == hexo deploy #部署  
  
hexo server #Hexo会监视文件变动并自动更新，无须重启服务器  
hexo server -s #静态模式  
hexo server -p 5000 #更改端口  
hexo server -i 192.168.1.1 #自定义 IP  
hexo clean #清除缓存，若是网页正常情况下可以忽略这条命令
```

## 重新生成文件并部署
```
hexo cl && hexo g && hexo d
```

## 重新生成文件并在本地服务器调试
```
hexo cl && hexo g && hexo s
```
# 建站指南
[文档 | Hexo](https://hexo.io/zh-cn/docs/)
[hexo博客中如何插入图片-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1736563)
