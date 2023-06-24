# 随机二次元图片
<br>

>## 前言
>## 此次为接口大幅度更新！！！请认真阅读文档内容！！！
> 文档更新日期：2023.6.24
>- 访问接口原图参数会直接下载图片
>- JSON调用已恢复且进行了升级
>- 接口默认图片清晰度为默认略缩图
>- 图片新增全新参数imtype、search、num、tags具体使用方法请看下面解释
>- 图片标签参数由"tag"改为"imgtype"

- 所有图片均来源于网络
- 为保证图片质量，所有图片均为手动添加和分类
- 截止至目前为止已经收录有6000+的二次元图片
- 图片最后更新时间为：2023.6.24
- [点击前往](https://tuku.xieweiling.top/)我搭建的图库在线看图

>## API基本调用格式
>- 调用方法：GET

- [点击前往](https://api.xieweiling.top/) 

```HTTPS
https://api.xieweiling.top/
```
<br>

>## 图片类型
>#### 原"tag="参数改为"imgtype="
>- 参数：imgtype=
>- 如果不带参数默认为全部图随机

- 全站图随机： [点击前往](https://api.xieweiling.top/?imgtype=random) 

```HTTPS
https://api.xieweiling.top/?imgtype=random
```

- 最新图片： [点击前往](https://api.xieweiling.top/?imgtype=zx) 

```HTTPS
https://api.xieweiling.top/?imgtype=zx
```
- 横屏图片： [点击前往](https://api.xieweiling.top/?imgtype=pc) 

```HTTPS
https://api.xieweiling.top/?imgtype=pc
```
- 竖屏图片： [点击前往](https://api.xieweiling.top/?imgtype=mp)

```HTTPS
https://api.xieweiling.top/?imgtype=mp
```
<br>

>## 图片标签
>#### 原来是包含在图片类型参数里面，现单独分开成一个参数
>- 参数：tags=
>- 如果不带参数默认随机输出一张图片

<table>
<thead>
<tr>
<th>图片参数</th>
<th>示例</th>
</tr>
</thead>
<tbody>
<tr>
<td>唯美</td>
<td><a href="https://api.xieweiling.top/?tags=唯美" target="_blank">https://api.xieweiling.top/?tag=random&size=large</a></td>
</tr>
<tr>
<td>风景</td>
<td><a href="https://api.xieweiling.top/?tags=风景" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>兽耳</td>
<td><a href="https://api.xieweiling.top/?tags=兽耳" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>泳装</td>
<td><a href="https://api.xieweiling.top/?tags=泳装" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>女仆</td>
<td><a href="https://api.xieweiling.top/?tags=女仆" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>制服</td>
<td><a href="https://api.xieweiling.top/?tags=制服" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>丝袜</td>
<td><a href="https://api.xieweiling.top/?tags=丝袜" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
<tr>
<td>其他</td>
<td><a href="https://api.xieweiling.top/?tags=其他" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
</tbody></table>

>## 请求图片规格大小

- 参数：size

- 默认为略缩图 medium

<table>
<thead>
<tr>
<th>图片大小</th>
<th>图片参数</th>
<th>示例</th>
</tr>
</thead>
<tbody><tr>
<td><code>原图</code></td>
<td>large</td>
<td><a href="https://api.xieweiling.top/?tag=random&size=large" target="_blank">https://api.xieweiling.top/?tag=random&size=large</a></td>
</tr>
<tr>
<td><code>略缩图</code></td>
<td>medium</td>
<td><a href="https://api.xieweiling.top/?tag=random&size=medium" target="_blank">https://api.xieweiling.top/?tag=random&size=medium</a></td>
</tr>
</tbody></table>

>## json调用待适配


<!--

>## JSON基础调用格式
>- type=json

- 示例： [点击前往](https://api.xieweiling.top/?tag=random&type=json) 
```HTTPS
https://api.xieweiling.top/?tag=random&type=json
```

- 返回格式:

```{"pic":"https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h3we4nb9sdj33vw230kjm.jpg"}```

>## JSON进阶格式
>- type=json1—10  

- 返回1到10张图（最高为10超出自动返图）

- 示例： [点击前往](https://api.xieweiling.top/?tag=random&type=json5) 
```HTTPS
https://api.xieweiling.top/?tag=random&type=json5
```
- 返回格式：
```
{
    "pic": [
        "https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h5fneir0akj31yv3hzkjm.jpg",
        "https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h5flerlmv5j317c22kb29.jpg",
        "https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h5fhespzdlj33jy4yo1l2.jpg",
        "https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h5fdriqh8gj31y00vihb6.jpg",
        "https:\/\/tva1.sinaimg.cn\/large\/008eUSAtgy1h5fkta1lfqj31c31y3ha6.jpg"
    ]
}
```
-->
