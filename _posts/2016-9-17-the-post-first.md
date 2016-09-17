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
