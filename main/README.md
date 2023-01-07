# 随机二次元图片
<br>

>## 前言
> 文档更新日期：2023.1.7
>- 因前几天某博再次加强了防盗链机制，导致之前所有图片无法访问，接口被迫暂停。
>- 现接口升级为3.0且已把所有图片转移至别处进行存储。
>- 接口的访问速度没有之前快而且直接访问接口会直接下载图片。
>- JSON调用暂时停止，恢复时间待定。
>- king参数改为tag

- 所有图片均来源于网络
- 为保证图片质量，所有图片均为手动添加和分类
- 截止至目前为止已经收录有5000+的二次元图片
- 图片最后更新时间为：2023.1.1
- [点击前往](https://tuku.xieweiling.top/)我搭建的图库在线看图

>## API基本调用格式
>- 调用方法：GET

- [点击前往](https://api.xieweiling.top/) 

```HTTPS
https://api.xieweiling.top/
```
<br>

>## 图片类型
>#### 原"king="参数改为"tag="
>- 参数：tag=
>- 如果不带参数默认为全部图随机

- 随机： [点击前往](https://api.xieweiling.top/?tag=random) 

```HTTPS
https://api.xieweiling.top/?tag=random
```
<!--
- 最新： [点击前往](https://api.xieweiling.top/?tag=zx) 

```HTTPS
https://api.xieweiling.top/?tag=zx
```-->
- 横屏： [点击前往](https://api.xieweiling.top/?tag=pc) 

```HTTPS
https://api.xieweiling.top/?tag=pc
```
- 竖屏： [点击前往](https://api.xieweiling.top/?tag=mp)

```HTTPS
https://api.xieweiling.top/?tag=mp
```
- 风景： [点击前往](https://api.xieweiling.top/?tag=fj)

```HTTPS
https://api.xieweiling.top/?tag=fj
```
- 兽耳： [点击前往](https://api.xieweiling.top/?tag=cat) 

```HTTPS
https://api.xieweiling.top/?tag=cat
```
- 泳装： [点击前往](https://api.xieweiling.top/?tag=yz) 

```HTTPS
https://api.xieweiling.top/?tag=yz
```
- 女仆： [点击前往](https://api.xieweiling.top/?tag=np) 

```HTTPS
https://api.xieweiling.top/?tag=np
```
- 制服： [点击前往](https://api.xieweiling.top/?tag=zf) 

```HTTPS
https://api.xieweiling.top/?tag=zf
```
- 丝袜： [点击前往](https://api.xieweiling.top/?tag=sw) 

```HTTPS
https://api.xieweiling.top/?tag=sw
```
- 唯美： [点击前往](https://api.xieweiling.top/?tag=wm) 

```HTTPS
https://api.xieweiling.top/?tag=wm
```
- 其他： [点击前往](https://api.xieweiling.top/?tag=qt) 

```HTTPS
https://api.xieweiling.top/?tag=qt
```

>## 请求图片规格大小

- 参数：size

- 默认为原图 large

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
