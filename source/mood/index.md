---
title: 心情墙
type: 心情墙
noDate: 'true'
comments: 'false'
aside: false
---

<script src="https://cdn.bootcss.com/jquery/3.1.1/jquery.min.js"></script>
<link type="text/css" rel="styleSheet"  href="https://cdn.jsdelivr.net/gh/qiaoyihe/Figure-bed/css/mood.css" />
<center>  
<section class="timeline" style="padding-bottom: 50px">
<ul>
<li class="in-view">
	<div>
	<time>2021/1/4</time>
	<div class="discovery">
		<span >come</span>
		<p> 认真复习！</p>
	</div>
</li>
<li class="in-view">
	<div>
	<time>2021/1/4</time>
	<div class="discovery">
		<span >come</span>
		<p> 认真复习！</p>
	</div>
</li>
<li class="in-view">
	<div>
	<time>2021/1/4</time>
	<div class="discovery">
		<span >come</span>
		<p> 认真复习！</p>
	</div>
</li>
<li class="in-view">
	<div>
	<time>2021/1/4</time>
	<div class="discovery">
		<span >come</span>
		<p> 认真复习！</p>
	</div>
</li>
<li class="in-view">
	<div>
	<time>2020/7/1</time>
	<div class="discovery">
		<span >行动起来</span>
		<p> 倒计时30天考试！</p>
	</div>
</li>
<li class="in-view">
	<div>
	<time>2020/6/5</time>
	<div class="discovery">
		<span >心情墙</span>
		<p> 博客添加心情墙，记录生活中的点滴😁！</p>
	</div>
</li>

            
</ul>
</section>

<script>

        $(function () {
            function isEmpty(obj) {
                if (typeof obj == "undefined" || obj == null || obj == "") {
                    return true;
                } else {
                    return false;
                }
            }

        })
        var items = document.querySelectorAll(".timeline li");

        function isElementInViewport(el) {
            var rect = el.getBoundingClientRect();
            return (
                rect.top >= 0 &&
                rect.left >= 0 &&
                rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
                rect.right <= (window.innerWidth || document.documentElement.clientWidth)
            );
        }

        function callbackFunc() {
            for (var i = 0; i < items.length; i++) {
                if (isElementInViewport(items[i])) {
                    if (!items[i].classList.contains("in-view")) {
                        items[i].classList.add("in-view");
                    }
                } else if (items[i].classList.contains("in-view")) {
                    items[i].classList.remove("in-view");
                }
            }
        }

        window.addEventListener("load", callbackFunc);
        window.addEventListener("scroll", callbackFunc);
    </script>

  