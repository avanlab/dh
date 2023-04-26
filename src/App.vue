<template>
<router-view></router-view>
</template>

<script>

export default {
name: 'App',
created() {
document.title=this.fn.title
if (!localStorage.getItem("userAddWeb")) {
let value = [];
localStorage.setItem("userAddWeb", JSON.stringify(value));
}
let hm = document.createElement("script");
hm.src = "https://hm.baidu.com/hm.js?30a43afea3e1cbad80ee4a2b266f676b";
let s = document.getElementsByTagName("script")[0];
s.parentNode.insertBefore(hm, s);
console.warn('ai爱学习，助你畅游AI世界');
}
}
</script>

<style>
@import url('https://s1.hdslb.com/bfs/static/jinkela/long/font/regular.css');
@import url('https://s1.hdslb.com/bfs/static/jinkela/long/font/medium.css');

a, blockquote, body, code, dd, div, dl, dt, fieldset, form, h1, h2, h3, h4, h5, h6, input, legend, li, ol, p, pre, td, textarea, th, ul {
font-family: -apple-system, HarmonyOS_Regular, HarmonyOS_Medium, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans, sans-serif, Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol, Noto Color Emoji !important;
box-sizing: border-box;
text-decoration: none;
color: #ebebeb;
font-size: 14px;
margin: 0;
}

.black {
color: #8a8b8e;
}

h1, h2, h3, h4, h5, h6, .h1, .h2, .h3, .h4, .h5, .h6 {
font-weight: 500;
}

h4, .h4, h5, .h5, h6, .h6 {
margin-top: 40px;
margin-bottom: 9px;
}

body {
background: linear-gradient(135deg,#c9d6ff,#e2e2e2);
}
</style>