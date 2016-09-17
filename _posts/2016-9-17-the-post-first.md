---
layout: blogs_single
thumbnail: https://github.com/NguyenTungs/NguyenTungs.github.io/blob/master/assets/img/mongodb-logo.png?raw=true
title: Javascript - Add object to array
logouser: https://avatars1.githubusercontent.com/u/15043041?v=3&s=466
description:  de mo
date: 17 Sep 2016
---

#### Cách get param với javascript

``` javascript

console.log(window.location.search);
// "?post=1234&action=edit"

var urlParams = new URLSearchParams(window.location.search);

console.log(urlParams.has('post')); // true
console.log(urlParams.get('action')); // "edit"
console.log(urlParams.getAll('action')); // ["edit"]
console.log(urlParams.toString()); // "?post=1234&action=edit"
console.log(urlParams.append('active', '1')); // "?post=1234&action=edit&active=1"

function getUrlParameter(name) {
    name = name.replace(/[\[]/, '\\[').replace(/[\]]/, '\\]');
    var regex = new RegExp('[\\?&]' + name + '=([^&#]*)');
    var results = regex.exec(location.search);
    return results === null ? '' : decodeURIComponent(results[1].replace(/\+/g, ' '));
};


getUrlParameter('post'); // "1234"
getUrlParameter('action'); // "edit"
```
<hr>
<section class="share">
    <h4>Share this post</h4>
    <a class="icon-twitter" href="http://twitter.com/share?text=Lorem ipsum dolor sit amet&url=https://nguyentungs.github.io/the-post-first/" onclick="window.open(this.href, 'twitter-share', 'width=550,height=235');return false;">
        <span class="hidden">Twitter</span>
    </a>
    <a class="icon-facebook" href="https://www.facebook.com/sharer/sharer.php?u=https://nguyentungs.github.io/the-post-first/" onclick="window.open(this.href, 'facebook-share','width=580,height=296');return false;">
        <span class="hidden">Facebook</span>
    </a>
    <a class="icon-google-plus" href="https://plus.google.com/share?url=https://nguyentungs.github.io/the-post-first/" onclick="window.open(this.href, 'google-plus-share', 'width=490,height=530');return false;">
        <span class="hidden">Google+</span>
    </a>
</section>

<br/>
<article class="post tag-article">
    <footer class="post-footer">
        <section class="author">
            <h4>Nguyen Tungs</h4>
            <img src='https://avatars1.githubusercontent.com/u/15043041?v=3&s=466' />
            <p>I am Nguyen Tungns a web developer from HCM, VietNam.</p>
        </section>
    </footer>
</article>
<br/>
<article class="post tag-article">
    <br/>
    <div id="disqus_thread">Comment here</div>
</article>