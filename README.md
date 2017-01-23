# HTML5_Reader
webapp HTML5项目包括：
0.base64解析图片icon</br>
1.jsonp请求和ajax请求</br>
2.js闭包</br>
3.本地储存，HTML5特性localstorage</br>
4.项目的搭建
<br/>项目定位：前端入门级玩家，需要项目来提升自己的同学。</br>项目背景：在完成慕课网实战项目视频的学习后，自主完成独立开发。</br>
<h1>项目中我所学到的</h1>
<h2>一、关于性能</h2>
<p>多次使用dom操作的时候，要把它保存在变量中：</p>
```java  
  
   var Dom = {
                    nav_top:$('.top-nav'),
                    nav_pannel:$('.bottom-nav-kind'),
                    font1:$('.font1'),
                    night1:$('.night1'),
                    font_control:$('.font-control'),
                    font_size_large:$('.font-size-large'),
                    font_size_small:$('.font-size-small'),
                    m_read_container:$('.m-read-container'),
                    container:$('.container'),
                    prev_button:$('.prev_button'),
                    next_button:$('.next_button')
                    }
   var win = $(window);
   var doc = $(document);
  
```
<p>小项目中你可能不会发现这么做对性能优化的好处，但当项目越来越大，这些都是拖慢你载入速度的元凶</p>
<h2>二、使用base64插入图片</h2>
<p>这个方法适用于插入小icon小图标，可以减少http请求，也是一种优化。</p>
