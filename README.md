A Chrome Extension and bookmarklet that lets you read webpages one word at a time.
----------------------------------------------------------------------------------

[Extension link](https://chrome.google.com/webstore/detail/spree/aehoaolhojlmaidnfkhdghceloolfojk)
[Bookmarklet link](javascript:!function(a,b){function c(){function j(){var a=b.createElement("div");return a.className="spreeCon",a.innerHTML="<div class='spreeaftwrap'><span style='color:#ffa500;margin-left:-50px'>Spree...</span></div>",b.body.appendChild(a)}function k(c,d){var e=c.length/3>>0,f=b.createElement("span"),g=b.createElement("span"),h=b.createElement("span"),i=b.createElement("div");f.style.float="right",g.style.color="#ffa500",i.className="spreeaftwrap",f.innerText=c.slice(0,e),g.innerText=c[e],h.innerText=c.slice(e+1),i.appendChild(g),i.appendChild(h),d.innerHTML="",d.appendChild(i),d.appendChild(f);var j=a.getComputedStyle(g).width.slice(0,-2)/-2;g.style.marginLeft=j+"px",f.style.marginRight=-j+"px"}function l(){g?(g=0,l.func()):g=1}function m(a){var b=c/5;38===a?c-=b:c+=b,40>c&&(c=40);var d=6e4/(c+50);o(d)}function n(a){if(n.arr.push(a),50===n.arr.length){for(var b=0,c=0;50>c;c++)b+=n.arr[c];o(6e4/(b/50)),n.arr.length=0}}function o(a){var c,d=b.getElementById("spreewpm")||(c=b.createElement("div"),c.id="spreewpm",b.body.appendChild(c));d.innerText="~"+a.toString().slice(0,6)+" wpm"}function p(b,i){var j=b.innerText.split(/\s+/),m=0,o=j.length,q=b.nextElementSibling;b.offsetTop+b.clientHeight+f>e+a.scrollY&&a.scrollTo(0,b.offsetTop+f-100);var r=b.style.cssText;b.style.cssText=h,function s(){if(d)return b.style.cssText=r,void 0;if(g)return l.func=s,void 0;if(o>m){var a=j[m++],e=0;if(a.length){k(a,i);var f=a[a.length-1];","===f?e=c/6:"."===f&&(e=c/3)}var h=c+e+8*a.length;n(h),setTimeout(s,h)}else b.style.cssText=r,q&&setTimeout(function(){p(q,i)})}()}var e,f,c=100,d=0,g=0,h="border-left:3px solid #ffa500; padding-left: 10px; margin-left:-13px",i=function(){var a=b.createElement("style");return a.appendChild(b.createTextNode("")),b.head.appendChild(a),a.sheet}();i.addRule(".spreeCon","position:fixed;color:#444;width:600px;height:100px;top:50%;left:50%;margin:-50px 0 0 -300px;z-index:9999;background:#fffefc;box-shadow:0 4px 6px -4px #666, 0 1px 2px 0 #666;text-align:left;font-size:36px;line-height:100px;font-family:Helvetica;font-weight:300",0),i.addRule(".spreeaftwrap","float:right;width:350px;display:inline-block;background:#fffefc;",1),i.addRule(".spreeaftwrap >span","float:left",2),i.addRule("#spreewpm","position:fixed;top:10px;right:10px;font-size:14px;font-family:Helvetica;background:#fffefc;padding:2px;box-shadow:0 1px 1px 0 #666;text-align:center;z-index:9999;color:#ffa500",3),i.addRule(".spreeaftwrap>span:before",'content: "";border-left: 1px solid #666;height: 25px;position:absolute;left: 249px;',4),i.addRule(".spreeaftwrap>span:after",'content: "";border-left: 1px solid #666;height: 25px;position:absolute;left: 249px;bottom:0px;',5),i.insertRule("@media screen and (max-width : 600px){.spreeCon{margin:-50px 0 0 0; width:100%;left:0}.spreeaftwrap{width:60%;}.spreeaftwrap>span:before,.spreeaftwrap>span:after{left:39.4%;}}",6),l.func=function(){},n.arr=[],a.addEventListener("mousedown",function(g){var h=setTimeout(function(){function i(){d=1,b.body.removeChild(h),b.body.removeChild(b.getElementById("spreewpm")),a.removeEventListener("keydown",k),a.removeEventListener("mousedown",i)}function k(a){a.preventDefault();var b=a.keyCode;return 38===b||40===b?m(b):32===b?l():(i(),void 0)}d=0,f=g.target.parentNode.offsetTop+50,e=a.innerHeight;var h=j();o(6e4/(c+50)),setTimeout(function(){p(g.target,h)},500),a.addEventListener("keydown",k),a.addEventListener("mousedown",i)},1e3),i=a.addEventListener("mouseup",function(){clearTimeout(h),a.removeEventListener("mouseup",i)})})}"loaded"===b.readyState||"complete"===b.readyState?c():a.addEventListener("DOMContentLoaded",c)}(window,document);). Drag onto your bookmarks bar.

* Hold down your mouse for one second over the text you want to read.
* Use the up and down arrows to change the text speed.
* Pause with the spacebar.
* Quit Spree with any other key or click.
