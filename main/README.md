# 随机二次元图片
<br>

>## 前言
>### 此次为接口大幅度更新！！！请认真阅读文档内容！！！
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
>- 可添加多个标签，如需多标签，请在每个标签后面添加一个英文逗号
>- 填写多标签会自动返回拥有其中一个标签的图片，不一定会返回同时包含多个填写的标签的图片
>- 如果想要同时查找包含多个标签的图片，请继续往下阅读文档

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
<td><a href="https://api.xieweiling.top/?tags=唯美" target="_blank">https://api.xieweiling.top/?tags=唯美</a></td>
</tr>
<tr>
<td>风景</td>
<td><a href="https://api.xieweiling.top/?tags=风景" target="_blank">https://api.xieweiling.top/?tags=风景</a></td>
</tr>
<tr>
<td>兽耳</td>
<td><a href="https://api.xieweiling.top/?tags=兽耳" target="_blank">https://api.xieweiling.top/?tags=兽耳</a></td>
</tr>
<tr>
<td>泳装</td>
<td><a href="https://api.xieweiling.top/?tags=泳装" target="_blank">https://api.xieweiling.top/?tags=泳装</a></td>
</tr>
<tr>
<td>女仆</td>
<td><a href="https://api.xieweiling.top/?tags=女仆" target="_blank">https://api.xieweiling.top/?tags=女仆</a></td>
</tr>
<tr>
<td>制服</td>
<td><a href="https://api.xieweiling.top/?tags=制服" target="_blank">https://api.xieweiling.top/?tags=制服</a></td>
</tr>
<tr>
<td>丝袜</td>
<td><a href="https://api.xieweiling.top/?tags=丝袜" target="_blank">https://api.xieweiling.top/?tags=丝袜</a></td>
</tr>
<tr>
<td>其他</td>
<td><a href="https://api.xieweiling.top/?tags=其他" target="_blank">https://api.xieweiling.top/?tags=其他</a></td>
</tr>
<tr>
<td>唯美+泳装</td>
<td><a href="https://api.xieweiling.top/?tags=唯美,泳装" target="_blank">https://api.xieweiling.top/?tags=唯美,泳装</a></td>
</tr>
<tr>
<td>制服+兽耳</td>
<td><a href="https://api.xieweiling.top/?tags=制服,兽耳" target="_blank">https://api.xieweiling.top/?tags=制服,兽耳</a></td>
</tr>
</tbody></table>

<br>

>## 多标签精准搜索
>- 参数：search=
>- 默认为0，如果是1则为精准搜索，0则是模糊搜索
>- 精准搜索会同时查找所填写的多个标签，只会输出包含填写的所有标签的图片，如果没有找到，会自动输出提示
>- 模糊搜索就是填写多标签后会自动返回拥有其中一个标签的图片

<table>
<thead>
<tr>
<th>搜索模式</th>
<th>参数</th>
<th>图片标签</th>
<th>示例</th>
</tr>
</thead>
<tbody>
<tr>
<td>模糊搜索</td>
<td>0</td>
<td>泳装+兽耳</td>
<td><a href="https://api.xieweiling.top/?tags=泳装,兽耳&search=0" target="_blank">https://api.xieweiling.top/?tags=泳装,兽耳&search=0</a></td>
</tr>
<tr>
<td>精准搜索</td>
<td>1</td>
<td>泳装+兽耳</td>
<td><a href="https://api.xieweiling.top/?tags=泳装,兽耳&search=1" target="_blank">https://api.xieweiling.top/?tags=泳装,兽耳&search=1</a></td>
</tr>
<tr>
</tbody></table>

<br>

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
<td><a href="https://api.xieweiling.top/?size=large" target="_blank">https://api.xieweiling.top/?size=large</a></td>
</tr>
<tr>
<td><code>略缩图</code></td>
<td>medium</td>
<td><a href="https://api.xieweiling.top/?size=medium" target="_blank">https://api.xieweiling.top/?size=medium</a></td>
</tr>
</tbody></table>

<br>

>## JSON基础调用格式
>- type=json

- 示例： [点击前往](https://api.xieweiling.top/?type=json) 
```HTTPS
https://api.xieweiling.top/?type=json
```

- 返回格式:

```
[
    {
        "id": "212",
        "imgurl": "https://img.beiko.top/img/mp/2q6oWF2h8aE=.jpg",
        "tags": "唯美;",
        "Upload_time": "2023-05-28"
    }
]
```
<br>

>## JSON进阶参数
>- num=
>- 默认为1张图片，最多20张，超出20之后都算20张

- 示例： [点击前往](https://api.xieweiling.top/?type=json&num=5) 
```HTTPS
https://api.xieweiling.top/?type=json&num=5
```
- 返回格式：
```
[
    {
        "id": "3801",
        "imgurl": "https://img.beiko.top/img/mp/jWSCKHGmc0I=.png",
        "tags": "丝袜;制服;",
        "Upload_time": "2023-05-28"
    },
    {
        "id": "3952",
        "imgurl": "https://img.beiko.top/img/mp/uYK[iWXr0Fs=.jpg",
        "tags": "唯美;",
        "Upload_time": "2023-05-28"
    },
    {
        "id": "3547",
        "imgurl": "https://img.beiko.top/img/mp/[AoM+vVmP2U=.jpg",
        "tags": "兽耳;",
        "Upload_time": "2023-05-28"
    },
    {
        "id": "5139",
        "imgurl": "https://img.beiko.top/img/pc/Q2+4LgKuKwI=.jpg",
        "tags": "兽耳;",
        "Upload_time": "2023-05-28"
    },
    {
        "id": "810",
        "imgurl": "https://img.beiko.top/img/mp/ca0NuJXRHbQ=.jpg",
        "tags": "制服;",
        "Upload_time": "2023-05-28"
    }
]
```
