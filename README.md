# jquery弹出框1Popup1
效果如下：
![](images/img.gif)

all code:
```
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>JQuery-CSS3制作简洁的弹框</title>
    <link rel="stylesheet" href="css/style.css"/>
</head>
<body>
<div class="checkbox">
    <a href="javascript:0;" class="cd-popup-trigger0">样式1</a>
    <a href="javascript:0;" class="cd-popup-trigger1">样式2</a>
    <a href="javascript:0;" class="cd-popup-trigger2">样式3</a>
    <a href="javascript:0;" class="cd-popup-trigger3">样式4</a>
</div>
<!--弹框-->
<div class="cd-popup">
    <div class="cd-popup-container">
        <p>几种常见的简洁弹框</p>
        <div class="cd-buttons">
            自定义整体容器宽高度及内容，高度可自适应可固定,样式可以定义自己喜欢的样式，这里就不做美观了
        </div>
        <a href="#0" class="cd-popup-close">close</a>
    </div>
</div>

<div class="cd-popup1">
    <div class="cd-popup-container1">
        <p>几种常见的简洁弹框</p>
        <div class="cd-buttons">
            自定义整体容器宽高度及内容，高度可自适应可固定,样式可以定义自己喜欢的样式，这里就不做美观了
        </div>
        <a href="#0" class="cd-popup-close">close</a>
    </div>
</div>

<div class="cd-popup2">
    <div class="cd-popup-container2">
        <p>几种常见的简洁弹框</p>
        <div class="cd-buttons">
            自定义整体容器宽高度及内容，高度可自适应可固定,样式可以定义自己喜欢的样式，这里就不做美观了
        </div>
        <a href="#0" class="cd-popup-close">close</a>
    </div>
</div>

<div class="cd-popup3">
    <div class="cd-popup-container3">
        <p>几种常见的简洁弹框</p>
        <div class="cd-buttons">
            自定义整体容器宽高度及内容，高度可自适应可固定,样式可以定义自己喜欢的样式，这里就不做美观了
        </div>
        <a href="#0" class="cd-popup-close">close</a>
    </div>
</div>
</body>
</html>
<script src="js/jquery-1.7.2.min.js"></script>
<script>
    /*弹框JS内容*/
    jQuery(document).ready(function($){
        //打开窗口
        $('.cd-popup-trigger0').on('click', function(event){
            event.preventDefault();
            $('.cd-popup').addClass('is-visible');
            //$(".dialog-addquxiao").hide()
        });
        //关闭窗口
        $('.cd-popup').on('click', function(event){
            if( $(event.target).is('.cd-popup-close') || $(event.target).is('.cd-popup') ) {
                event.preventDefault();
                $(this).removeClass('is-visible');
            }
        });
        //ESC关闭
        $(document).keyup(function(event){
            if(event.which=='27'){
                $('.cd-popup').removeClass('is-visible');
            }
        });

        //打开窗口
        $('.cd-popup-trigger1').on('click', function(event){
            event.preventDefault();
            $('.cd-popup1').addClass('is-visible1');
            //$(".dialog-addquxiao").hide()
        });
        //关闭窗口
        $('.cd-popup1').on('click', function(event){
            if( $(event.target).is('.cd-popup-close') || $(event.target).is('.cd-popup1') ) {
                event.preventDefault();
                $(this).removeClass('is-visible1');
            }
        });
        //ESC关闭
        $(document).keyup(function(event){
            if(event.which=='27'){
                $('.cd-popup1').removeClass('is-visible1');
            }
        });

        //打开窗口
        $('.cd-popup-trigger2').on('click', function(event){
            event.preventDefault();
            $('.cd-popup2').addClass('is-visible2');
            //$(".dialog-addquxiao").hide()
        });
        //关闭窗口
        $('.cd-popup2').on('click', function(event){
            if( $(event.target).is('.cd-popup-close') || $(event.target).is('.cd-popup2') ) {
                event.preventDefault();
                $(this).removeClass('is-visible2');
            }
        });
        //ESC关闭
        $(document).keyup(function(event){
            if(event.which=='27'){
                $('.cd-popup2').removeClass('is-visible2');
            }
        });

        //打开窗口
        $('.cd-popup-trigger3').on('click', function(event){
            event.preventDefault();
            $('.cd-popup3').addClass('is-visible3');
            //$(".dialog-addquxiao").hide()
        });
        //关闭窗口
        $('.cd-popup3').on('click', function(event){
            if( $(event.target).is('.cd-popup-close') || $(event.target).is('.cd-popup3') ) {
                event.preventDefault();
                $(this).removeClass('is-visible3');
            }
        });
        //ESC关闭
        $(document).keyup(function(event){
            if(event.which=='27'){
                $('.cd-popup3').removeClass('is-visible3');
            }
        });
    });
</script>

```

