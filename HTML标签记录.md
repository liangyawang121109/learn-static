### html标签记录

#### 标题标签

```html
<h1>
    test
</h1>
<h2>
    test2
</h2>
<h3>
    test3
</h3>
<h4>
    test4
</h4>
<h5>
    test5
</h5>
<h6>
    test6
</h6>
```

- 标题标签一共六级 

#### 段落标签

```html
<p>
    我是一个段落标签
</p>
```

- 使用p标签将语句进行段落分段

#### 换行标签

````html
<br /> 
````

- br就是一个换行标签 强制换行 单标签

#### 文本格式化标签

```html
加粗 <strong></strong> 或者 <b></b> *
倾斜 <em></em> 或者<i></i>          *
下划线 <ins></ins> 或者<u></u>
删除线 <del></del> 或者 <s></s>
```

- 文本格式化的语义就是突出重要性 比普通文字更重要

#### div & span 标签

```html
<div>
     它是一个盒子 分割 分区
</div>
<span>
	它是一个小盒子  跨度 跨距
</span>
```

- div 标签是用来布局的 一行只能放一个div 它是一个大盒子
- span 标签是用来布局的 一行能放多个span 他是一个小盒子

#### 图像标签

```html
<img src="xxx/xxx/xx.png" alt=“xx图片显示不出来了” title="xxx" width="500" height="100" border="15">
```

- 用于定义html页面中的图像 单标签
    - src 图片路径 必须属性
    - alt 文本 替换文本 当图片显示不出来的时候就显示这个属性定义的文字
    - title 提示文本 当鼠标放到图片上的时候 就会显示这个属性定义的文字
    - width 图像的宽度设定
    - height 图像的高度设定
    - border 设置图片的边框 需要对边框设定像素 一般由css设定 此处记忆即可

#### 超链接标签

```html
<a href="http://www.baidu.oom" target= "_blank">百度</a>
```

- href 跳转目的地
- target 跳转窗口弹出的方式 其中 _self为默认值 _blank 在新的窗口打开跳转地址

##### 内部链接 空链接  下载链接 网页元素链接

```html
<a href="#" > 空链接 </a>
```

##### 空链接

```html
<a href="index.html"> 内部链接</a>
```

##### 下载链接

```html
<a  href="image.zip"> 下载链接</a>
```

##### 网页元素链接

```html
<a href="http://www.baidu.com"> <img src="img.pg"></a>
```

##### 锚点链接

```html
#在链接文本的属性中国设置属性为#名字的形式 如下：
<a href="#two"> 主要作品 </a>
#找到目标位置标签 里边添加一个id属性 = 刚才链接文本定义的名字 如下：
<h3 id="two">
    作品介绍
</h3>

```

- 当我们点击链接 可以快速定位到页面中的某个位置

#### 注释标签

```htjml
<!-- 我被注释了-->
```

#### 特殊字符

```html
&nbsp;  一个就是一个空格
&lt;    小于号
&gt;    大于号
&amp;   and符 &
&yen;	人民币
&copy;	版权
&reg;	注册商标
&deg;	摄氏度

```

#### 表格标签

```html
//属性由css设置 此处只做记忆
<table align="center" border="1" cellpadding="20" cellspacing="0" width="500" height="300">
   <thead> //划分表格的头部区域
        <tr>
            <th> 年龄</th>
            <th> 性别</th>
            <th> 名字</th>
        </tr>
    </thead>
  
    <tbody> //划分表格的body区域
        <tr>
            <td> 20</td>
            <td> 男</td>
            <td> 梁</td>
        </tr>
    </tbody> 
</table>
```

- 作用 用于显示展示数据 因为它可以让数据显示的非常规整 可读性好
    - tr 定义单元行 必须在 table中
    - td 定义单元格 必须在tr中
    - th 定义表头单元格 表头单元格中的文字 加粗并居中
    - align  规定表格相对周围元素的对齐方式
        - left 
        - center
        - right
    - border 规定表格单元是否有边框 默认没有
    - cellpadding 像素值 规定单元边沿与其内容之间的空白
    - cellspacing 规定单元格之间的空白
    - width 规定表格宽度
    - height 规定表格的高度

##### 表格结构标签

- 作用 使表格的语义更明显

- <thead> 划分表格的头部区域
- <tbody> 划分表格的主体区域

##### 合并单元格

```html
<table align="center" border="1" cellpadding="20" cellspacing="0" width="500" height="300">
   <thead> //划分表格的头部区域
  		<tr> <td></td> <td olspan="2"></td></tr>
  		<tr> <td rowspan="2"></td> <td></td> <td></td></tr>
  		<tr>  <td></td> <td></td></tr>
  		<tr> <td></td> <td></td> <td></td></tr>
    </tbody> 
</table>
```

- 跨行合并 rowspan="合并的单元格的数量"
- 跨列合并 colspan="合并的单元格的数量"

#### 列表标签

- 列表最大的特点就是整齐 整洁有序 他作为布局会更加自由和方便

##### 无序列表

```html
<ul>
    <li>列表1</li>
    <li>列表2</li>
    <li>列表3</li>
    <li>列表4</li>
</ul>
```

- ul 中只能嵌套li标签
- li里边可以嵌套任意元素标签
- 无序列表 各个列表之间是没有顺序级别之分的 他们是并列的

##### 有序列表

```html
<ol>
    <li>li-1</li>
    <li>li-2</li>
    <li>li-3</li>
    <li>li-4</li>
</ol>
```

##### 自定义列表

```html
<dl>
    <dt> 名词1</dt>
    <dd>名词解释</dd>
    <dd>名词相关</dd>
</dl>
```

#### 表单标签

- 表单由三部分组成 表单域 表单控件 提示信息

##### 表单域

```html
<form action="url地址" method="post" name="user">
    
</form>
```

- 将表单域内的信息提交给后台进行记录
- action url地址 用于指定接收并处理表单数据的服务器程序url地址
- method post/get 用于设置表单提交方式
- name 用于指定表单的名称 以区分同一个页面中的多个表单域

##### 表单控件

###### input 输入表单元素

```html
<form action="url地址" method="post" name="user">
    用户名：<input type="text" name="username" value="请输入用户名"> <br/ >
    密码： <input type="password" name="password" value="请输入密码" maxlength="6"> <br />
    性别： 男<input type="radio" name="sex" checked="checked">  女<input type="radio" name="sex"> <br />
    爱好：  吃饭<input type="checkbox" name="hobby" checked="checked"> 睡觉<input type="checkbox" name="hobby"> 玩儿<input type="checkbox" name="hobby"> <br />
    <input type="submit" value="免费提交">
    <input type="reset" value="重新输入">
    <input type="button" value="获取验证码"> <br />
    <input type="file" value="请上传文件">
    <input type="image" >
    
</form>
```

- 单标签
- type 属性设置不同指定不同的控件类型
- text 定义单行的输入字段 用户可以在输入框中输入任何文本
- password 定义密码字段 将密码掩盖
- radio 单选按钮  可以实现多选 默认是多选 如果单选必须name属性名字相同才可实现多选一
- checkbox 多选按钮
- name 用于区别input表单的不同
- value 在输入框里显示的
- checked 规定此input 元素首次加载时 被选中
- maxlength 规定输入框中最大的输入长度
- submit 定义提交按钮 直接将表单域内的值 送给服务器
- reset 重置按钮 会将表单域内的数据清除
- button 定义点击按钮 通常和js脚本结合
- file 文件域 提供文件上传
- image 定义图像形式的提交按钮

###### label标签

```html
<label for="user">用户名：</label> <input type="text" id="user" name="username" value="请输入用户名"><br/ >
```

- label 标签用于绑定一个表单元素 当点击label标签内的文本时 浏览器就会自动将光标转到或者选择对应的表单元素上 增加用户体验
- label 标签的for属性应当与相关元素的id属性相同

###### select 下拉表单元素

```html
<select>
    <option selected="selected">选项1</option>
    <option>选项2</option>
    <option>选项3</option>
    <option>选项4</option>
</select>
```

- select中至少包含一对option
- 在option中定义selected="selected"时 当前选项即为默认选项

###### textarea 文本域元素

```html
今日反馈：
<textarea cols="50" rows="5">这是默认的页面展示的几个字 可删</textarea>
```

- 当用户内容较多的情况下 使用文本域标签 多行输入
- cols 每行中的字符数
- rows 显示的行数 在实际使用中 不使用这两个属性 用css来定义大小

