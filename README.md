# BlogHexo

博客的源码,主题为NexT  [官网](http://theme-next.iissnan.com/)  
博客所用博客框架,Hexo  [官网](https://hexo.io/zh-cn/)  

## 重新部署到github流程

### 一、在我的gitee中把源码拷贝下来

```
    git clone git@gitee.com:wyongt/BlogHexo.git
```

### 二、修改博客中的域名和git地址

######  修改_config.yml
######  url

```
    url:http://wangyt.xyz
```

###### git地址

```
    deploy:
    - type:git
      repo: git@github.com:wangyongtan/wangyongtan.github.io.git
```



### 三、生成博客并把博客部署

```
    hexo clean
    hexo g 
    hexo d
```

### 四、域名解析

#### 得到的ip绑定到A上

```
    ping wangyongtan.github.io 
```

#### 把CANME绑定

```
    wangyongtan.github.io
```

### 五、添加域名到hexo的public中
- 在public中建立CNAME文件
- 添加域名
```
    wwangyt.xyz
    www.wangyt.xyz
```

### 六、添加域名到github page中

- 在github page中的设置中找到 Custom domain
- 添加域名 

``` 
    wangyt.xyz
```


