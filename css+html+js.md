 <style> 
    * {
        margin:0;
        padding:0;
    }
     body {
         margin-top: 50px;
         margin-left:580px;
        }
        .circle {
            height: 123px;
            width: 123px;
            background-color: #e8ae5a;
            border-radius: 100%;   
            line-height:123px;    
         }
         .juxing {
             height: 268px;
             width: 137px;
             background-color: #f1d568;
             margin-top: 27px;
             border-radius: 10%;
         }
    </style>
<body>

    <div class="circle"></div> 
    <div class="juxing"></div> 
    </body>

###                               第一次练习多彩感叹号

```
<style>
     .first {
         float:left;
         height: 100px;
         width: 100px;
         background-color: #c5bfbf;
         border-radius: 50%;
         margin-left: 17px;
         border:1px solid black;
         background-color: red;
         }
     .second {
        float:left;
         height: 100px;
         width: 100px;
         background-color: #c5bfbf;
         border-radius: 50%;
         margin-left: 17px;
         border:1px solid #282222;
         background-color: yellow;
     }
     .third {
        float:left;
         height: 100px;
         width: 100px;
         background-color: #c5bfbf;
         border-radius: 50%;
         margin-left: 17px;
         border:1px solid black;
         background-color: green;
     }
 </style>
</head>
<body>
     <div class="first"></div>
     <div class="second"></div>
     <div class="third"></div>
</body>
```

### 第二次练习红路灯

```
.tree {
     margin-top: 100px;
     width: 30px;
     height: 300px;
     background-color: #7d4924;
     border-radius: 5px;
     display: flex;
     flex-direction: column;
     justify-content: space-around;
 }
 .tree .branch {
     width: 160px;
     height: 20px;
     background-color: #a98354;
     border-radius: 10px;
     display:flex;
     justify-content: flex-end;
     transform: rotate(-30deg);
 }
 .tree .branch .leaf {
     width: 40px;
     height: 40px;
     background-color: #34783a;
     border-radius: 100% 0 100% 0;
     transform: translateY(-100%);
 </style>
</head>
<body>
   <figure class="tree">
       <div class="branch">
           <span class="leaf"></span>
           <span class="leaf"></span>
           <span class="leaf"></span>
       </div>
       <div class="branch">
        <span class="leaf"></span>
        <span class="leaf"></span>
       </div>
   </figure>
</body>
```

### 第三次练习三角形

```
 <style>
        .trange {
            width: 500px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .trange div {
            height: 50px;
            margin:5px;
            display: flex;
            justify-content: space-between;
        }
        .trange div span {
            width: 50px;
            height: 50px;
            margin:10px;
            background-color: lightgreen;
            border-radius: 50%;
        }
        .trange div span:first-child, 
        .trange div span:last-child {
            background-color: lightcoral;
        }
    </style>
</head>
<body>
    <figure class="trange">
        <div>
            <span></span>
        </div>
        <div>
            <span></span>
            <span></span>
        </div>
        <div>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
    </figure>
```

：nth-child()伪类流传较为广泛的用法是：nth-child(odd)和nth-child(even),其中：nth-child(odd)表示选择所有第奇数个元素，nth-child(even)表示选择所有第偶数个元素。

### 第四次练习棋盘 

```
<style>
        * {
            margin:0;
            padding:0;
        }
    .big {
        width: 400px;
        background-color: #e4c292;
        border:5px solid darkgray;
    }
    .big div {
        display: flex;
    }
    .big div span {
        width: 100px;
        height: 100px;
    }
    .big div:nth-child(odd) span:nth-child(even),
    .big div:nth-child(even) span:nth-child(odd){
        background-color: #93835f;
    }
    </style>
</head>
<body>
    <figure class="big">
    <div>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
    </div>
    <div>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
    </div>
    <div>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
    </div>
    <div>
        <span></span>
        <span></span>
        <span></span>
       <span></span>
    </div>
    </figure>
</body>
```

### 第五次练习淘宝轮播图

```
 * {
            margin:0;
            padding:0;
        }
        li {
            list-style: none;
        }
        .tb-promo {
            position: relative;
            width: 520px;
            height: 280px;
            background-color: pink;
            margin:100px auto;
        }
        /* 保证图片的大小都是520*280，过大或过小图片都会被压缩或者放大 */
        .tb-promo img {
            width: 520px;
            height: 280px;
        }
        /* 并集选择器可以集体声明相同的样式 */
        .next,.prev {
            position: absolute;
            /* 绝对定位的盒子垂直居中算法 */
            /* 让加了绝对定位盒子向上走盒子高度的一半 */
            top:50%;
            margin-top:-15px;
            /* 加了绝对定位的盒子可以直接设置宽度和高度 */
            width: 20px;
            height: 30px;
            background-color: rgba(0,0,0,.3);
            text-align: center;
            line-height: 30px;
            color:#fff;
            text-decoration: none;
        }
        .prev {
            left: 0;
            border-top-right-radius: 15px;
            border-bottom-right-radius: 15px;
        }
        .next {
            /* 如果一个盒子里既有left属性又有right属性，则默认执行left属性，同理top bottom 会执行bottom */
            right: 0;
            border-top-left-radius: 15px;
            border-bottom-left-radius: 15px;
        }
        .pro-nav {
            position: absolute;
            bottom:15px;
            left:50%;
            margin-left:-35px;
            width: 70px;
            height: 13px;
            background: rgba(255,255,255,.3);
            border-radius: 7px;
        }
        .pro-nav li {
            float:left;
            width: 8px;
            height: 8px;
            background-color: #fff;
            border-radius: 50%;
            margin:3px;
        }
        .pro-nav .selected {
            background-color: #ff5000;
        }
    </style>
</head>
<body>
    <div class="tb-promo">
        <img src="pro_07.jpg" alt="">
        <!-- 左侧按钮箭头 -->
        <a href="#" class="prev"><</a>
        <a href="#" class="next">></a>
        <ul class="pro-nav">
            <li cass="selected"></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>
</body>
```

### 第六次练习图片遮罩层

```
<style>
       .tudou {
           position: relative;
           width: 444px;
           height: 320px;
           background-color: pink;
           margin:30px auto;
       }
       .tudou img {
           /* 图片里的宽和高要和父亲盒子一样高 */
           height: 100%;
           width: 100%;
       }
       .mask {
           /* 隐藏遮罩层 */
           display: none;
           position: absolute;
           left:0;
           top:0;
           width: 100%;
           height: 100%;
           background:rgba(0,0,0,.3) url(btn.png) no-repeat center;
       }
       .tudou:hover .mask{
           /* 当我们的鼠标经过了土豆这个盒子，就让里面的遮罩层显示出来 */
           display: block;
       }
   </style>
</head>
<body>
   <div class="tudou">
       <div class="mask"></div>
       <img src="pro_07.jpg" alt="">
       </div>
</body>
```

### <u>字体图标的下载</u>

有两个网站，first icomoon字库，http://icomoon.io

second 阿里iconfont字库， http://www.iconfont.cn/

### 精灵图的使用拼名字

```css
 <style>
     span {
         display: inline-block;
         background: url(abcd.jpg) no-repeat;
     }
     .p {
         width: 100px;
         height: 112px;
         background-position:  -493px -276px;
     }
     .i {
         width: 60px;
         height: 108px;
         background-position:  -327px -141px;
     }
     .n {
         width: 110px;
         height: 113px;
         background-position:  -215px -141px;
     } 
     .k {
         width: 105px;
         height: 114px;
         background-position:  -495px -142px;
     }
   </style>
</head>
<body>
   <span class="p"></span>
   <span class="i"></span>
   <span class="n"></span>
   <span class="k"></span>
</body>
```

### 行内块元素的巧妙应用

只要给父盒子加text-align:center;那这个父盒子里面的行内元素和行内块元素都会水平居中

```css
<style>
     .box {
       text-align: center;
     }
  .box a {
    display: inline-block;
    height: 36px;
    width: 36px;
    background-color: #f7f7f7;
    border:1px solid #ccc;
    text-decoration: none;
    line-height: 36px;
    text-align: center;
    color:#333;
    font-size: 14x;
  }
  .box .prev,.box .next {
    width: 85px;
  }
 .box .current,.box .elp {
   background-color: #fff;
   border: none;
 }
   </style>
</head>
<body>
<div class="box">
  <a href="#" class="prev">&lt;&lt;上一页</a>
  <a href="#" class="current">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#" class="elp">...</a>
  <a href="#" class="next">下一页&gt;&gt;</a>
</div>
</body>
```

![](C:\Users\dell\Desktop\前端练习照片\捕获.PNG)

### 直角三角形的做法：

```css
 width: 0;
 height: 0;
 border-color: transparent red transparent transparent;
 border-style:solid;
 border-witdh: 22px 8px 0 0;
```

<img src="C:\Users\dell\Desktop\前端练习照片\直角三角形.PNG" style="zoom:50%;" />



### 梯形价格标签

```css
<style>
     .price {
       width: 160px;
       height: 24px;
       border:1px solid red;
       margin:0 auto;
       text-align: center;
       line-height: 24px;
       color: #fff;
       font-weight: 700;
     }
     .miaosha {
       position: relative;
       float: left;
       width: 90px;
       height: 100%;
       background-color: red;
       color:black;
     }
     .miaosha i {
       position: absolute;
       right:0;
       width: 0;
       height: 0;
       border-color: transparent #fff transparent transparent;
       border-style: solid;
       border-width: 24px 10px 0 0;
     }
   </style>
</head>
<body>
<div class="box"></div>
<div class="price">
  <span class="miaosha">$1650
    <i></i>
  </span>
  <span>$5650</span>
</div>
</body>
```

<img src="C:\Users\dell\Desktop\前端练习照片\Screenshot 2020-12-05 223131.png" style="zoom:50%;" />

### 京东初始化css

```css
*{
    margin:0;
    padding:0
}
/* 斜体的文字不倾斜 */
em,i{
    font-style:normal
}
/* 去掉li里面的小圆点 */
li{
    list-style:none
}

img{
    /* /border:0* 照顾低版本浏览器 如果图片外面包含了链接会有边框的问题 */ */
    border:0;
    /* 取消图片底侧有空白缝隙的问题 */
    vertical-align:middle
}
button{
    /* 当我们的鼠标经过button的时候，鼠标变成小手 */
    cursor:pointer
}
a{
    /* 所有链接的颜色和取消下划线 */
    color:#666;
    text-decoration:none
}
a:hover{
    /* 鼠标经过会变成红色 */
    color:#c81623
}
button,input{
    /* 指定字体 */
    font-family:Microsoft YaHei,
    Heiti SC,
    tahoma,
    arial,
    Hiragino Sans GB,
    "\5B8B\4F53",
    sans-serif
}
body{
    /* 抗锯齿形，让文字显示的更清晰 */
    -webkit-font-smoothing:antialiased;
    background-color:#fff;
    /* 12像素1.5倍行高 */
    font:12px/1.5 Microsoft YaHei,Heiti SC,tahoma,arial,Hiragino Sans GB,"\5B8B\4F53",sans-serif;
    color:#666
}
.hide,.none
{
    /* 隐藏元素 */
    display:none
}
/* 伪元素清除浮动 */
.clearfix:after{
    visibility:hidden;
    clear:both;
    display:block;
    content:".";
    height:0
}
.clearfix{
    *zoom:1
}
```

### 就业面试技巧与解析：

1、HTML 5中新多媒体元素有哪些？

1、audio元素：播放音频文件；2、video元素：播放视频文件；3、<source>元素：允许用户规定两个视频、音频文件共用浏览器，根据它对媒体类型或者编解码器的支持进行选择。4、embed元素： 插入各种多媒体，格式可以MIDI,WAV,AIFF,AU,MP3等。

2、HTML 5中分组元素有哪些？

1、<hgroup>元素用于对网页或者区段（section）的标题进行分组，<hgroup>元素通常会将会h1-h6元素进行分组，比如一个内容区块的标题及其子标题算一组。2、<figure>标签用来表示网页上一块独立的内容，将其从网页上移除后不会对网页上的其他内容产生影响。3、<figcaption>元素的作用是为<figure>元素定义标题。

# Javascript

## js倒计时

```js
function countDown (time) {
    var nowTime = +new Date();
    // 返回当前时间总的毫秒数
    var inputTime = +new Date(time);
    // 返回的是用户输入时间总的毫秒数
    var times = (inputTime-nowTime) / 1000;
    // times是剩余时间的总数
    var d = parseInt(times / 60 /60 / 24);//天
    d = d < 10 ? '0' + d : d;
    var h = parseInt(times / 60 /60 % 24);//时
    h = h < 10 ? '0' + h : h;
    var m = parseInt(times / 60 % 60);//分
    m = m < 10 ? '0' + m : m;
    var s = parseInt(times % 60);//秒
    s = s < 10 ? '0' + s : s;
    return d + '天' + h + '时' + m + '分' + s + '秒';
  }
console.log(countDown('2021-3-22 21:00:00'));
var date = new Date();
console.log(date);
```



## 仿淘宝关闭二维码

```js
  .box{
      position: relative;
      width: 74px;
      height: 88px;
      border:1px solid #ccc;
      margin:100px auto;
      font-size: 12px;
      text-align: center;
      color:#f40;
    }
  .box img {
    width: 60px;
    margin-top: 5px;
  }
  .close-btn{
    position: absolute;
    top: -1px;
    left: -16px;
    width: 14px;
    height: 14px;
    border:1px solid #ccc;
    line-height: 14px;
    font-family: Arial, Helvetica, sans-serif;
    cursor: pointer;
  }
  </style>
</head>
<body>
 <div class="box">
   淘宝二维码
   <img src="jsapis_material\第一天\images\tao.png" alt="">
   <i class="close-btn">×</i>
 </div>
  <script>
    var btn = document.querySelector('.close-btn');
    var box = document.querySelector('.box');
    btn.onclick = function(){
      box.style.display = 'none';
    }
```

<img src="C:\Users\dell\Desktop\前端练习照片\js_files\tao.png" style="zoom:33%;" />

## 精灵图关键代码

```js
var lis = document.querySelectorAll('li');
           for(var i=0;i<lis.length;i++){
             var index = i*44;
             lis[i].style.backgroundPosition='0 -' +　index　+ 'px';
           }
```

## 京东输入框

```js
<style>
   input {
     color: #999;
     }
  </style>
</head>
<body>
 <input type="text" value="手机">       
     <script>
        var text = document.querySelector('input');
        //获取焦点
        text.onfocus = function(){
        if(this.value == '手机'){
          this.value = '';
        }
        //输入的文字颜色变深，利用了element.style
        this.style.color = '#333';
        }
        //失去焦点
        text.onblur = function(){
         if(this.value==''){
           this.value = '手机';
         }
         //失去焦点后，颜色变浅
         this.style.color = '#999';
        }
    </script>
```

## 仿注册页面

```js
<style>
        div {
            width: 600px;
            margin: 100px auto;
        }
        
        .message {
            display: inline-block;
            font-size: 12px;
            color: #999;
            background: url(images/mess.png) no-repeat left center;
            padding-left: 20px;
        }
        
        .wrong {
            color: red;
            background-image: url(images/wrong.png);
        }
        
        .right {
            color: green;
            background-image: url(images/right.png);
        }
    </style>
</head>

<body>
    <div class="register">
        <input type="password" class="ipt">
        <p class="message">请输入6~16位密码</p>
    </div>
    <script>
        // 首先判断的事件是表单失去焦点 onblur
        // 如果输入正确则提示正确的信息颜色为绿色小图标变化
        // 如果输入不是6到16位，则提示错误信息颜色为红色 小图标变化
        // 因为里面变化样式较多，我们采取className修改样式
        // 1.获取元素
        var ipt = document.querySelector('.ipt');
        var message = document.querySelector('.message');
        //2. 注册事件 失去焦点
        ipt.onblur = function() {
            // 根据表单里面值的长度 ipt.value.length
            if (this.value.length < 6 || this.value.length > 16) {
                // console.log('错误');
                message.className = 'message wrong';
                message.innerHTML = '您输入的位数不对要求6~16位';
            } else {
                message.className = 'message right';
                message.innerHTML = '您输入的正确';
            }
        }
    </script>
```

## 新浪下拉菜单

```js
<style>
  * {
            margin: 0;
            padding: 0;
        }
        
        li {
            list-style-type: none;
        }
        
        a {
            text-decoration: none;
            font-size: 14px;
        }
        
        .nav {
            margin: 100px;
        }
        
        .nav>li {
            position: relative;
            float: left;
            width: 80px;
            height: 41px;
            text-align: center;
        }
        
        .nav li a {
            display: block;
            width: 100%;
            height: 100%;
            line-height: 41px;
            color: #333;
        }
        
        .nav>li>a:hover {
            background-color: #eee;
        }
        
        .nav ul {
            display: none;
            position: absolute;
            top: 41px;
            left: 0;
            width: 100%;
            border-left: 1px solid #FECC5B;
            border-right: 1px solid #FECC5B;
        }
        
        .nav ul li {
            border-bottom: 1px solid #FECC5B;
        }
        
        .nav ul li a:hover {
            background-color: #FFF5DA;
        }
</style>
<body>
    <ul class="nav">
        <li>
            <a href="#">微博</a>
            <ul>
                <li>
                    <a href="#">私信</a>
                </li>
                <li>
                    <a href="#">评论</a>
                </li>
                <li>
                    <a href="#">@我</a>
                </li>
                
            </ul>
        </li>
        <li>
            <a href="#">微博</a>
            <ul>
                <li>
                    <a href="#">私信</a>
                </li>
                <li>
                    <a href="#">评论</a>
                </li>
                <li>
                    <a href="#">@我</a>
                </li>
                
            </ul>
        </li>
        <li>
            <a href="#">微博</a>
            <ul>
                <li>
                    <a href="#">私信</a>
                </li>
                <li>
                    <a href="#">评论</a>
                </li>
                <li>
                    <a href="#">@我</a>
                </li>
                
            </ul>
        </li>
        <li>
            <a href="#">微博</a>
            <ul>
                <li>
                    <a href="#">私信</a>
                </li>
                <li>
                    <a href="#">评论</a>
                </li>
                <li>
                    <a href="#">@我</a>
                </li>
                
            </ul>
        </li>
    </ul>
    <script>
        var nav = document.querySelector('.nav');
        var lis = nav.children;
        for(var i= 0 ;i<lis.length;i++){
            lis[i].onmouseover = function(){
                this.children[1].style.display = 'block';
            }
            lis[i].onmouseout = function(){
                this.children[1].style.display = 'none';
            }
        } 
    </script>
</body>
```



## 开关灯案例

```js
<body>
 <button id="btn">开关灯</button>
   <script>
    var open = document.getElementById('btn');
    var flag = 0;
    open.onclick = function(){
      if (flag == 0){
        //注意这里是改变body的样式，而且不能只用body,只能用document.body.
     document.body.style.backgroundColor = 'black';
      flag = 1;
    }
    else {
     document.body.style.backgroundColor = '#fff';
      flag = 0;
       }
    }
   </script>
</body>
```

## 排他思想（算法）

```js
<body>
 <button>按钮1</button>
 <button>按钮2</button>
 <button>按钮3</button>
 <button>按钮4</button>
 <button>按钮5</button>
   <script>
    var btn =document.querySelectorAll('button');
    //btn得到的是伪数组，具体里面的元素要用btn[i]表示。
    //利用循环给所有的按钮绑定了事件。
  for(var i = 0;i<btn.length;i++){
    btn[i].onclick = function(){
      //先把所有的背景颜色去掉
      for(var i = 0;i<btn.length;i++){
      btn[i].style.backgroundColor = '';
    }
    //然后让当前的元素背景为pink色，
      this.style.backgroundColor = 'pink';
  }
}
//首先排除其他人，然后再设置自己的样式，称为排他思想。
   </script>
</body>
```

## 百度换肤

```js
	<style>
  * {
    padding:0;
    margin:0;
  }
  body {
    background: url(images/1.jpg) no-repeat center top;
  }
  .baidu {
    overflow: hidden;
    margin:100px auto;
    background-color: #fff;
    width: 410px;
    padding-top: 3px;
  }
.baidu li {
  list-style: none;
  /* 去掉小圆点 */
  float:left;
  margin:0 1px;
  cursor: pointer;
}
.baidu img {
  width: 100px;
}
</style>
<body>
 <ul class="baidu">
   <li><img src="images/1.jpg"></li>
   <li><img src="images/2.jpg"></li>
   <li><img src="images/3.jpg"></li>
   <li><img src="images/4.jpg"></li>
 </ul>
   <script>
    var pic =document.querySelector('.baidu').querySelectorAll('img');
    //btn得到的是伪数组，具体里面的元素要用btn[i]表示。
    //利用循环给所有的按钮绑定了事件。
  for(var i = 0;i<pic.length;i++){
    pic[i].onclick = function(){
      //this.src可以获得当前图片的路径
      //把这个路径给body就可以了
      document.body.style.backgroundImage = 'url('+this.src+')';
    
  }
}
   </script>
</body>
```

## 表单隔行变色关键语句

```js
<script>
     //获取元素获取tbody里面的所有的行
    var trs = document.querySelector('tbody').querySelectorAll('tr');
    for (var i=0;i<trs.length;i++){
    //利用循环绑定事件
    //鼠标经过事件 onmouseover
    trs[i].onmouseover = function(){
    this.className = 'bg'
    //当前添加了bg这个类
    }
    //鼠标离开事件onmouseout
    trs[i].onpointerout = function(){
      this.className = '';
    }
    }
   </script>
```

## 表单全选取消全选

```js
<style>
       table {
            width: 200px;
            margin: 100px auto;
            text-align: center;
            border-collapse: collapse;
            border: 1px solid #c0c0c0c0;
            font-size: 14px;
            border-spacing: 0;
        }
        thead tr {
            height: 30px;
            background-color: skyblue;
        }
        tbody tr {
            height: 30px;
        }
        tbody td {
            border-bottom: 1px solid #d7d7d7;
            font-size: 12px;
            color: blue;
        }
        th,td{
            border:1px solid #c0c0c0c0;
        }
</style>
<body>
 <div>
  <table>
    <thead>
       <tr>
           <th>
               <input type = "checkbox" id="j_c" >
           </th>
           <th>商品</th>
           <th>价钱</th>
       </tr>
    </thead>
    <tbody id="j_tb">
        <tr>
            <td><input type = "checkbox"></td>
            <td>iPhone8</td>
            <td>8000</td>
        </tr>
        <tr>
            <td><input type = "checkbox"></td>
            <td>iPad pro</td>
            <td>5000</td>
        </tr>
        <tr>
            <td><input type = "checkbox"></td>
            <td>iPad Air</td>
            <td>2000</td>
        </tr>
        <tr>
            <td><input type = "checkbox"></td>
            <td>Apple Watch</td>
            <td>2000</td>
        </tr>
    </tbody>
   </table>
  </div>
  <script>
      var j_c = document.getElementById('j_c');
      var j_tbs = document.getElementById('j_tb').getElementsByTagName('input');
      j_c.onclick = function(){
          //this.checked可以得到当前复选框的选中状态
for(var i = 0;i<j_tbs.length;i++){
    //把当前全选选没选中的状态this.checked赋值给所有复选框j_tbs[i]就可以了，复选框选没选中的状态就是j_tbs[i].checked
    j_tbs[i].checked = this.checked;
    }
      }
      //下面是复选框全部选中，上面的全选才能选中做法，给下面的所有复选框绑定点击事件，每次点击，都要循环检查
for(var i = 0;i<j_tbs.length;i++){
    j_tbs[i].onclick = function(){
        //flag控制全选按钮是否选中
        var flag = true;
        //每次点击都要循环检查4个小按钮是否被全部选中
        for(var i = 0; i < j_tbs.length;i++){
            if(!j_tbs[i].checked) {
                flag = false;
            }
        }
        j_c.checked = flag;
    }
}
     </script>
</body>
```

## 自定义属性的操作

####     获取属性值：

​              element.属性      获取属性值（获取内置属性值）；element.getAttribute('属性')；（获取自定义的属性）；

#### 设置属性值：

​           element.属性 = '值'，element.setAttribute('属性')；H5规定自定义属性是以data开头作为属性名并且赋值。<div data-index = '1'></div>

#### 获取元素的方法：

 1、利用DOM提供的方法获取元素：document.getElementById();     document .getElementTagName();    document.querySelector();                                                           2、 利用节点层级关系获取元素：父子兄层级关系<div class="box"><span class="erweim"></span></div>       要是想获取div里面的元素可以通过儿子 var box = document.querySelector('.erweima');       erweima.parentNode就可以得到最近父亲元素。                                                                                                                                      子节点：一般不提倡parentNode.childNodes,        直接使用非标准的parentNode.children.                    parentNode.firstElementChild.返回第一个子元素节点    ，  parentNode.lastElementChild.返回最后一个子元素节点    ，  

```js
var ul = document.querySelector('ul');
for(var i = 0; i < ul.childNodes.length;i++){
if(ul.childSelector[i].nodeType == 1){
     //ul.childSelector[i]是元素节点
    console.log(ul.childNodes[i]);
   }
}
```

兄弟节点：

```js
<body>
    <div>我是div</div>
    <span>我是span</span>
    <script>
        var div = document.querySelector('div');
        //nextSibling下一个兄弟节点，包含元素节点，文本节点等
        //nextElementSibling返回兄弟的下一个元素节点
        console.log(div.nextSibling);
        console.log(div.nextElementSibling);
        //上一个兄弟元素节点是previousElementSibling 考虑兼容性
    </script>
    
</body>
```

#### 动态创建和添加元素(节点)

```js
<body>
   <ul></ul> 
   <!-- 父元素 -->
   <script>
       var li = document.createElement('li');//1、创建节点createElement();
       var ul = document.querySelector('ul');//获取父元素；
       ul.appendChild(li);//2、添加节点 node.appendChild(child),其中node是父级，child是子级
       //3、在指定元素前添加元素node.insertBefore(child,指定元素)；
       var lili = document.createElement('li');
       ul.insertBefore(lili,ul.children[0]);
       //4、我们想要页面添加一个新的元素：1、创建元素，2、添加元素
   </script> 
   
</body>
```

#### 删除节点和复制节点

node.removeChild(node.children[0]);node父亲                                                                                   node.cloneNode()

## tab切换制作

```js
<style>
     * {
            margin: 0;
            padding: 0;
        }
        
        li {
            list-style-type: none;
        }
        
        .tab {
            width: 978px;
            margin: 100px auto;
        }
        
        .tab_list {
            height: 39px;
            border: 1px solid #ccc;
            background-color: #f1f1f1;
        }
        
        .tab_list li {
            float: left;
            height: 39px;
            line-height: 39px;
            padding: 0 20px;
            text-align: center;
            cursor: pointer;
        }
        
        .tab_list .current {
            background-color: #c81623;
            color: #fff;
        }
        
        .item_info {
            padding: 20px 0 0 20px;
        }
        
        .item {
            display: none;
        }
</style>
<body>
    <div class="tab">
        <div class="tab_list">
            <ul>
                <li class="current">商品介绍</li>
                <li>规格与包装</li>
                <li>售后保障</li>
                <li>商品评价</li>
                <li>手机社区</li>
            </ul>
        </div>
        <div class="tab_con">
            <div class="item" style="display: block;">商品介绍模块内容</div>
            <div class="item">规格与包装模块内容</div>
            <div class="item">售后保障模块内容</div>
            <div class="item">商品评价</div>
            <div class="item">手机模块</div>
        </div>
    </div>
  <script>
      var tab_list = document.querySelector('.tab_list');
      var lis = tab_list.querySelectorAll('li');
      var items = document.querySelectorAll('.item');
      for(var i = 0;i < lis.length;i++){
          //开始给5个小li设置索引号
          lis[i].setAttribute('index',i);
          lis[i].onclick = function(){
            for(var i = 0;i<lis.length;i++){
                //清除其余li的class类
                lis[i].className = '';
            }
            //留下当前的
            this.className = 'current';
            // 2、下面的显示内容模块
             var index = this.getAttribute('index');
             //干掉所有人，让其余的item 这些div隐藏
             for(var i = 0;i < items.length;i++){
                 items[i].style.display = 'none';
             }
             //留下我自己，让对应的item显示出来
         items[index].style.display = 'block';
          }
      }
  </script>
```

## 简单版发布留言（添加节点和删除节点）

```js
<body>
   
   <textarea name="" id="" cols="30" rows="10"></textarea>
   <button>发布</button>
   <ul>
    
   </ul>
   <script>
       var btn = document.querySelector('button');
       var text = document.querySelector('textarea');
       var ul = document.querySelector('ul');
       btn.onclick = function(){
           if(text.value == ''){
               alert('您没有输入内容')
               return false;
           }else {
           var li = document.createElement('li');
           li.innerHTML = text.value + "<a href='javascript:;'>删除</a>";
           ul.insertBefore(li,ul.children[0]);
           //删除节点，给li里面添加一个删除链接
           var as = document.querySelectorAll('a');
           for(var i= 0;i< as.length;i++){
               as[i].onclick = function(){
                   //a(this.parentNode) 的父亲就是li,li的父亲是ul
                   ul.removeChild(this.parentNode);
               }
           }
           }
       }
   </script>
</body>
```

## 动态生成表格案例

```js
  <style>
        table {
            width: 500px;
            margin: 100px auto;
            border-collapse: collapse;
            text-align: center;
        }
        
        td,
        th {
            border: 1px solid #333;
        }
        
        thead tr {
            height: 40px;
            background-color: #ccc;
        }
    </style>
</head>

<body>
    <table cellspacing="0">
        <thead>
            <tr>
                <th>姓名</th>
                <th>科目</th>
                <th>成绩</th>
                <th>操作</th>
            </tr>
        </thead>
        <tbody>

        </tbody>
    </table>
    <script>
        // 1.先去准备好学生的数据
        var datas = [{
            name: '魏璎珞',
            subject: 'JavaScript',
            score: 100
        }, {
            name: '弘历',
            subject: 'JavaScript',
            score: 98
        }, {
            name: '傅恒',
            subject: 'JavaScript',
            score: 99
        }, {
            name: '明玉',
            subject: 'JavaScript',
            score: 88
        }, {
            name: '大猪蹄子',
            subject: 'JavaScript',
            score: 0
        }];
        // 2. 往tbody 里面创建行： 有几个人（通过数组的长度）我们就创建几行
        var tbody = document.querySelector('tbody');
        for (var i = 0; i < datas.length; i++) { // 外面的for循环管行 tr
            // 1. 创建 tr行
            var tr = document.createElement('tr');
            tbody.appendChild(tr);
            // 2. 行里面创建单元格(跟数据有关系的3个单元格) td 单元格的数量取决于每个对象里面的属性个数  for循环遍历对象 datas[i]
            for (var k in datas[i]) { // 里面的for循环管列 td
                // 创建单元格 
                var td = document.createElement('td');
                // 把对象里面的属性值 datas[i][k] 给 td  
                // console.log(datas[i][k]);
                td.innerHTML = datas[i][k];
                tr.appendChild(td);
            }
            // 3. 创建有删除2个字的单元格 
            var td = document.createElement('td');
            td.innerHTML = '<a href="javascript:;">删除 </a>';
            tr.appendChild(td);

        }
        // 4. 删除操作 开始 
        var as = document.querySelectorAll('a');
        for (var i = 0; i < as.length; i++) {
            as[i].onclick = function() {
                // 点击a 删除 当前a 所在的行(链接的爸爸的爸爸)  node.removeChild(child)  
                tbody.removeChild(this.parentNode.parentNode)
            }
        }
        // for(var k in obj) {
        //     k 得到的是属性名
        //     obj[k] 得到是属性值
        // }
    </script>
</body>
```

#### 三种动态创建元素方式

1、document.write()创建元素，如果页面文档流加载完毕，再调用这句话会导致页面重绘，2、innerHTML      3、document.createElement()创建元素。

#### 注册事件概述

给元素添加事件有两种方式：称为注册事件或者绑定事件，                                                       传统注册方式：利用on开头的事件onclick;       特点是：注册事件的唯一性

```js
<button onclick - "alert('hi~')"></button>
btn.onclick = function(){
alert('hi~');
}
//删除事件btn.onclick = null;
```

方法监听注册方式：addEventListener( '事件类型'，函数(){})它是一个方法，特点：同一个元素可以添加多个侦听器（事件处理程序）

```js
<button onclick - "alert('hi~')"></button>
btn.addEventListener('click',function(){
alert(22);
})
//删除事件:btn.addEventListener('click',fn)
function fn (){
alert(22);
btn.removeEventListener('click',fn)//移除fn
}
```

#### DOM事件流

事件发生时会在元素节点之间按照规定的顺序传播，这个传播过程即DOM事件流         DOM事件流分为三个阶段：1、捕获阶段，2、当前目标阶段，3、冒泡阶段

#### e.target和this

e.target返回的是触发事件的元素（点击了那个元素就返回哪个元素），this返回的是绑定事件元素（那个元素绑定了点击事件，就返回谁）

#### 事件委托的原理

事件委托也称为事件代理，在jquery里面称为事件委派，原理：不是每个子节点单独设置时间监听器，而是时间监听器设置在其父节点上，然后利用冒泡原理影响设置每个子节点。

#### 	常用鼠标事件：

onclick:左键触发；

onmouseover:鼠标经过触发；

onmouseout:鼠标离开触发；

onfocus/onblur:鼠标获得焦点触发/失去焦点触发

onmousemove:移动触发

onmousedown:鼠标按下触发

contextmenu:禁止鼠标右键菜单

```js
document.addEventListener('contextmenu',function(e){
e.preventDefault();
})
```

selectstart:禁止鼠标选中；

```js
document.addEventListener('selectstart',function(e){
e.preventDefault();
}
```

#### 鼠标事件对象

e.pageX,Y相当于文档页面

e.srceenX,Y相当于电脑屏幕

```js
 <script>
        document.addEventListener('click',function(e){
            //鼠标在可视区内的x坐标
       console.log(e.clientX);
       console.log(e.clientY);
        })
    </script>
```

## 跟随鼠标的小精灵

```js
<body>
    <img src="D:\js素材\第三天\images\angel.gif" alt="">
    <script>
        var pic = document.querySelector('img');
        document.addEventListener('mousemove',function(e){
            console.log(1);
            var x = e.pageX;
            var y = e.pageY;
            console.log(x,y);
            pic.style.left = x-50 + 'px';
            pic.style.top = y-40 + 'px';
        })
    </script>
```

#### 常用键盘事件

onkeyup:某个按键被松开时触发

keydown:按键被按下时触发

onkeypress:按下是除法，不识别功能键。

#### 键盘属性

  `    keydown` 与 `keyup` 事件捕获了键盘按键的操作，而 `keypress` 反映了具体输入某个字符的值。比如, 小写"a" 在`keydown` 和 `keyup`事件中输出的是大写A的Unicode编码65，但是在`keypress`中输出的就是小写"a"的Unicode编码97。大写 "A"在这些事件中输出的都是Unicode编码65。

键盘事件只能由 ``, `` 以及任何具有 `contentEditable` 或 `tabindex="-1"`属性的组件触发。

## 倒计时效果

```js
<style>
     div {
            margin: 200px;
        }
    span{
        display: inline-block;
        border: 1px solid #ccc;
        background-color: black;
        color:#ccc;
        width: 40px;
        height: 40px;
        text-align: center;
        line-height: 40px;
        font-size: 20px;
    }
</style>
<body>
    <div>
        <span class = "hour">1</span>
        <span class = "minute">2</span>
        <span class = "second">3</span>
    </div>
    <script>
        var hour  = document.querySelector('.hour');
        var minute = document.querySelector('.minute');
        var second = document.querySelector('.second');
        var inputTime = +new Date('2021-4-5 20:00:00');
    // 返回的是用户输入时间总的毫秒数
    countDown();
    setInterval(countDown,1000);
        function countDown () {
    var nowTime = +new Date();
    // 返回当前时间总的毫秒数
    var times = (inputTime-nowTime) / 1000;
    // times是剩余时间的总数
    var h = parseInt(times / 60 /60 % 24);//时
    h = h < 10 ? '0' + h : h;
    hour.innerHTML = h;
    var m = parseInt(times / 60 % 60);//分
    m = m < 10 ? '0' + m : m;
    minute.innerHTML = m;
    var s = parseInt(times % 60);//秒
    s = s < 10 ? '0' + s : s;
    second.innerHTML = s;
        }   
    </script>
</body>
```

## 发送短信案例

```js
<body>
    手机号码<input type="number"><button>发送</button>
    <script>
        var btn = document.querySelector('button');
        var time = 3;
        btn.addEventListener('click',function(){
            btn.disabled = true;//按钮点击之后要禁用按钮
           var timer = setInterval(function(){
               if(time == 0){
                   //清除定时器和复原按钮
                   clearInterval(timer);
                   btn.disabled = false;
                   btn.innerHTML = '发送';
                   time = 3;//需要从新开始
               }
                 else {
                     btn.innerHTML = '还剩下' + time + '秒';
                 time--;
                     }
           },1000)
        })
    </script>
```

```
(function flexible(window, document) {
    // 获取的html 的根元素
    var docEl = document.documentElement
        // dpr 物理像素比
    var dpr = window.devicePixelRatio || 1

    // adjust body font size  设置我们body 的字体大小
    function setBodyFontSize() {
        // 如果页面中有body 这个元素 就设置body的字体大小
        if (document.body) {
            document.body.style.fontSize = (12 * dpr) + 'px'
        } else {
            // 如果页面中没有body 这个元素，则等着 我们页面主要的DOM元素加载完毕再去设置body
            // 的字体大小
            document.addEventListener('DOMContentLoaded', setBodyFontSize)
        }
    }
    setBodyFontSize();

    // set 1rem = viewWidth / 10    设置我们html 元素的文字大小
    function setRemUnit() {
        var rem = docEl.clientWidth / 10
        docEl.style.fontSize = rem + 'px'
    }

    setRemUnit()

    // reset rem unit on page resize  当我们页面尺寸大小发生变化的时候，要重新设置下rem 的大小
    window.addEventListener('resize', setRemUnit)
        // pageshow 是我们重新加载页面触发的事件
    window.addEventListener('pageshow', function(e) {
        // e.persisted 返回的是true 就是说如果这个页面是从缓存取过来的页面，也需要从新计算一下rem 的大小
        if (e.persisted) {
            setRemUnit()
        }
    })

    // detect 0.5px supports  有些移动端的浏览器不支持0.5像素的写法
    if (dpr >= 2) {
        var fakeBody = document.createElement('body')
        var testElement = document.createElement('div')
        testElement.style.border = '.5px solid transparent'
        fakeBody.appendChild(testElement)
        docEl.appendChild(fakeBody)
        if (testElement.offsetHeight === 1) {
            docEl.classList.add('hairlines')
        }
        docEl.removeChild(fakeBody)
    }
}(window, document))
```

## 淘宝flexible.js源码分析

```js
(function flexible(window, document) {
    // 获取的html 的根元素
    var docEl = document.documentElement
        // dpr 物理像素比
    var dpr = window.devicePixelRatio || 1

    // adjust body font size  设置我们body 的字体大小
    function setBodyFontSize() {
        // 如果页面中有body 这个元素 就设置body的字体大小
        if (document.body) {
            document.body.style.fontSize = (12 * dpr) + 'px'
        } else {
            // 如果页面中没有body 这个元素，则等着 我们页面主要的DOM元素加载完毕再去设置body
            // 的字体大小
            document.addEventListener('DOMContentLoaded', setBodyFontSize)
        }
    }
    setBodyFontSize();

    // set 1rem = viewWidth / 10    设置我们html 元素的文字大小
    function setRemUnit() {
        var rem = docEl.clientWidth / 10
        docEl.style.fontSize = rem + 'px'
    }

    setRemUnit()

    // reset rem unit on page resize  当我们页面尺寸大小发生变化的时候，要重新设置下rem 的大小
    window.addEventListener('resize', setRemUnit)
        // pageshow 是我们重新加载页面触发的事件
    window.addEventListener('pageshow', function(e) {
        // e.persisted 返回的是true 就是说如果这个页面是从缓存取过来的页面，也需要从新计算一下rem 的大小
        if (e.persisted) {
            setRemUnit()
        }
    })

    // detect 0.5px supports  有些移动端的浏览器不支持0.5像素的写法
    if (dpr >= 2) {
        var fakeBody = document.createElement('body')
        var testElement = document.createElement('div')
        testElement.style.border = '.5px solid transparent'
        fakeBody.appendChild(testElement)
        docEl.appendChild(fakeBody)
        if (testElement.offsetHeight === 1) {
            docEl.classList.add('hairlines')
        }
        docEl.removeChild(fakeBody)
    }
}(window, document))
```

## 淘宝侧边栏

```js
<style>
    .slider-bar {
        position: absolute;
        left: 50%;
        top: 300px;
        margin-left: 600px;
        width: 45px;
        height: 130px;
        background-color: pink;
    }
    .w {
            width: 1200px;
            margin: 10px auto;
        }
    .header{
        height: 150px;
        background-color: rgb(155, 202, 241);
    }
    .banner{
        height: 250px;
        background-color: rgb(235, 168, 173);
    }
    .main{
        height: 1000px;
        background-color: rgb(146, 243, 89);
    }
    span{
        display: none;
        position: absolute;
        bottom:0;
    }
</style>
<body>
    <div class = "slider-bar">
        <span class="goback">返回顶部</span>
    </div>
    <div class = "header w">头部区域</div>
    <div class = "banner w">banner区域</div>
    <div class = "main w">主题部分</div>
    <script>
        //获取元素
        var sliderbar = document.querySelector('.slider-bar');
        var banner = document.querySelector('.banner');
        var bannertop = banner.offsetTop;
        var sliderbartop = sliderbar.offsetTop-bannertop;
        var main =document.querySelector('.main');
        var goback = document.querySelector('.goback');
        var mainTop = main.offsetTop;
        //页面滚动事件scroll
        document.addEventListener('scroll',function(){
        if(window.pageYOffset >=bannertop){
            //当页面被卷的头部大于等于172时，此时侧边栏要改为固定定位。
            sliderbar.style.position = 'fixed';
            sliderbar.style.top = sliderbartop + 'px';
        }else{
            sliderbar.style.position = 'absolute';
            sliderbar.style.top = '300px';
        }
        if(window.pageYOffset >=mainTop){
            //当页面被卷的头部大于等于172时，此时侧边栏要改为固定定位。
            goback.style.display = 'block';
        }else{
            goback.style.display = 'none';
        }
        })
    </script>
</body>
```

## 动画原理

```js
<body>
    <div></div>
    <script>
        // 动画原理
        // 1. 获得盒子当前位置  
        // 2. 让盒子在当前位置加上1个移动距离
        // 3. 利用定时器不断重复这个操作
        // 4. 加一个结束定时器的条件
        // 5. 注意此元素需要添加定位， 才能使用element.style.left
        var div = document.querySelector('div');
        var timer = setInterval(function() {
            if (div.offsetLeft >= 400) {
                // 停止动画 本质是停止定时器
                clearInterval(timer);
            }
            div.style.left = div.offsetLeft + 1 + 'px';
        }, 30);
    </script>
</body>
```

## 简单动画封装

```js
 <style>
        div {
            position: absolute;
            left: 0;
            width: 100px;
            height: 100px;
            background-color: pink;
        }
        
        span {
            position: absolute;
            left: 0;
            top: 200px;
            display: block;
            width: 150px;
            height: 150px;
            background-color: purple;
        }
    </style>
</head>

<body>
    <button>点击夏雨荷才走</button>
    <div></div>
    <span>夏雨荷</span>
    <script>
        // var obj = {};
        // obj.name = 'andy';
        // 简单动画函数封装obj目标对象 target 目标位置
        // 给不同的元素指定了不同的定时器
        function animate(obj, target) {
            // 当我们不断的点击按钮，这个元素的速度会越来越快，因为开启了太多的定时器
            // 解决方案就是 让我们元素只有一个定时器执行
            // 先清除以前的定时器，只保留当前的一个定时器执行
            clearInterval(obj.timer);
            obj.timer = setInterval(function() {
                if (obj.offsetLeft >= target) {
                    // 停止动画 本质是停止定时器
                    clearInterval(obj.timer);
                }
                obj.style.left = obj.offsetLeft + 1 + 'px';

            }, 30);
        }

        var div = document.querySelector('div');
        var span = document.querySelector('span');
        var btn = document.querySelector('button');
        // 调用函数
        animate(div, 300);
        btn.addEventListener('click', function() {
            animate(span, 200);
        })
    </script>
</body>
```

## 缓冲动画

```js
    <style>
        * {
            margin: 0;
            padding: 0;
        }
      div {
          position: absolute;
          left:0;
          width: 100px;
          height: 100px;
          background-color: rgb(248, 190, 190);
      }
      span{
          position: absolute;
          top:100px;
          display: block;
          width: 150px;
          height: 150px;
          background-color: rgb(197, 243, 241);
      }
    </style>
</head>
<body>
    <button>点击走500</button>
    <button class="btn2">点击走800</button>
    <div></div>
    <span></span>
    <script>
        function animate(obj,target){
            clearInterval(timer);
            var timer =  setInterval(function(){
            var step =(target - obj.offsetLeft) / 10;
            step = step > 0 ? Math.ceil(step) : Math.floor(step);
            if(obj.offsetLeft==target){
                clearInterval(timer);
            }else
            obj.style.left = obj.offsetLeft +step + 'px';
        },30)
}
      var span = document.querySelector('span');
      var btn = document.querySelector('button');
      var btn1 = document.querySelector('.btn2');
      btn.addEventListener('click',function(){
        animate(span,500);
      })
      btn1.addEventListener('click',function(){
        animate(span,800);
      })
    </script>
</body>
```

