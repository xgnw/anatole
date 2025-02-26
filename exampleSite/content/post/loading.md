+++
author = "爸比娃娃"
title = "loading效果"
date = "2025-02-13"
tags = [
    "网站制作",
]
+++

##第一步：
新建一个loading样式css
将以下代码放进去 然后引用这个文件

```
#Loadanimation{
    background-color:#fff;
    height:100%;
    width:100%;
    position:fixed;
    z-index:1;
    margin-top:0px;top:0px;
    
}
#Loadanimation-center{
    width:100%;
    height:100%;
    position:relative;
    
}
#Loadanimation-center-absolute{
    position:absolute;
    left:50%;
    top:50%;
    height:200px;
    width:200px;
    margin-top:-100px;
    margin-left:-100px;
    
}
.xccx_object{
    -moz-border-radius:50% 50% 50% 50%;
    -webkit-border-radius:50% 50% 50% 50%;
    border-radius:50% 50% 50% 50%;
    position:absolute;
    border-left:5px solid #87CEFA;
    border-right:5px solid #FFC0CB;
    border-top:5px solid transparent;
    border-bottom:5px solid transparent;
    -webkit-animation:animate 2.5s infinite;
    animation:animate 2.5s infinite;
    
}
#xccx_one{
    left:75px;
    top:75px;
    width:50px;
    height:50px;
    
}
#xccx_two{
    left:65px;
    top:65px;
    width:70px;
    height:70px;
    -webkit-animation-delay:0.1s;
    animation-delay:0.1s;
    
}
#xccx_three{
    left:55px;
    top:55px;
    width:90px;
    height:90px;
    -webkit-animation-delay:0.2s;animation-delay:0.2s;
    
}
#xccx_four{
    left:45px;
    top:45px;
    width:110px;
    height:110px;
    -webkit-animation-delay:0.3s;
    animation-delay:0.3s;
    
}
@-webkit-keyframes animate{50%{
    -ms-transform:rotate(180deg);
    -webkit-transform:rotate(180deg);
    transform:rotate(180deg);
    
}
100%{-ms-transform:rotate(0deg);
    -webkit-transform:rotate(0deg);
    transform:rotate(0deg);
    
}
    
}
@keyframes animate{50%{
    -ms-transform:rotate(180deg);
    -webkit-transform:rotate(180deg);
    transform:rotate(180deg);
    
}
100%{
    -ms-transform:rotate(0deg);
    -webkit-transform:rotate(0deg);
    transform:rotate(0deg);
    
}
}
```


##第二步：
将以下代码填写入头部文件 一般都为 header.php

<div id="Loadanimation" style="z-index:999999;">
<div id="Loadanimation-center">
    <div id="Loadanimation-center-absolute">
        <div class="xccx_object" id="xccx_four"></div>
        <div class="xccx_object" id="xccx_three"></div>
        <div class="xccx_object" id="xccx_two"></div>
        <div class="xccx_object" id="xccx_one"></div>
    </div>
</div>
</div>
<script>
$(function(){ 
    $("#Loadanimation").fadeOut(540); 
});
</script>
注意 注意 fadeOut 里面填写的是毫秒数

###后言
本loading可以自定义 网上也有很多css的 只要替换第二步的代码都可以成功(js代码别替换)
