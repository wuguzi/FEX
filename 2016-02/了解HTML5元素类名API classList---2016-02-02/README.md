#### 了解HTML5元素类名API classList

> HTML5以前的API可以用反人类来形容
> 
> 不过HTML5后很多API好了很多，其中classList方法和jQuery操作类的功能没有相似
>
> 我们先对比一下，然后详细分析


<table>
	<tr>
		<td>功能</td>
		<td>jQuery</td>
		<td>classList</td>
	</tr>
	<tr>
		<td>添加</td>
		<td>addClass</td>
		<td>add</td>
	</tr>

	<tr>
		<td>删除</td>
		<td>removeClass</td>
		<td>remove</td>
	</tr>
	<tr>
		<td>查询</td>
		<td>hasClass</td>
		<td>contains</td>
	</tr>
	<tr>
		<td>切换</td>
		<td>toggleClass</td>
		<td>toggle</td>
	</tr>
	<tr>
		<td>索引</td>
		<td>---</td>
		<td>item</td>
	</tr>
</table>

#####支线任务1
添加

```
jQuery:
$('#div').addClass('active');

JS:
document.querySelector('#div').classList.add('active');

```
> 返回undefined，所以不能连续操作

#####支线任务2
删除

```
jQuery:
$('#div').removeClass('active');

JS:
document.querySelector('#div').classList.remove('active');

```
> 返回undefined，所以不能连续操作

#####支线任务3
查询

```
jQuery:
$('#div').hasClass('active');

JS:
document.querySelector('#div').classList.constains('active');

```
> 返回true 表示存在
> 
> 返回false 表示不存在
> 
> 返回undefined，所以不能连续操作

#####支线任务4
切换

```
jQuery:
$('#div').toggleClass('active');

JS:
document.querySelector('#div').classList.toggle('active');

```
> 如果存在则删除
> 
> 如果不存在则添加
> 
> 返回undefined，所以不能连续操作

#####支线任务5
```
JS:
document.querySelector('#div').item(0);

```
> 如果没有返回null
