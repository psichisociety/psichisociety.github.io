<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">	
	<head><script type="text/javascript">window.NREUM||(NREUM={});NREUM.info = {"beacon":"bam.nr-data.net","errorBeacon":"bam.nr-data.net","licenseKey":"fbe52127be","applicationID":"110202938","transactionName":"b1FaNUtUV0dWV0xYClYbbRNQGl5RWVFKUAkXV00STVpUGlZHSA==","queueTime":0,"applicationTime":310,"agent":"","atts":""}</script><script type="text/javascript">(window.NREUM||(NREUM={})).loader_config={xpid:"VQYOUVZbCRABVVFQBwMOVVw="};window.NREUM||(NREUM={}),__nr_require=function(t,n,e){function r(e){if(!n[e]){var o=n[e]={exports:{}};t[e][0].call(o.exports,function(n){var o=t[e][1][n];return r(o||n)},o,o.exports)}return n[e].exports}if("function"==typeof __nr_require)return __nr_require;for(var o=0;o<e.length;o++)r(e[o]);return r}({1:[function(t,n,e){function r(t){try{s.console&&console.log(t)}catch(n){}}var o,i=t("ee"),a=t(16),s={};try{o=localStorage.getItem("__nr_flags").split(","),console&&"function"==typeof console.log&&(s.console=!0,o.indexOf("dev")!==-1&&(s.dev=!0),o.indexOf("nr_dev")!==-1&&(s.nrDev=!0))}catch(c){}s.nrDev&&i.on("internal-error",function(t){r(t.stack)}),s.dev&&i.on("fn-err",function(t,n,e){r(e.stack)}),s.dev&&(r("NR AGENT IN DEVELOPMENT MODE"),r("flags: "+a(s,function(t,n){return t}).join(", ")))},{}],2:[function(t,n,e){function r(t,n,e,r,s){try{p?p-=1:o(s||new UncaughtException(t,n,e),!0)}catch(f){try{i("ierr",[f,c.now(),!0])}catch(d){}}return"function"==typeof u&&u.apply(this,a(arguments))}function UncaughtException(t,n,e){this.message=t||"Uncaught error with no additional information",this.sourceURL=n,this.line=e}function o(t,n){var e=n?null:c.now();i("err",[t,e])}var i=t("handle"),a=t(17),s=t("ee"),c=t("loader"),f=t("gos"),u=window.onerror,d=!1,l="nr@seenError",p=0;c.features.err=!0,t(1),window.onerror=r;try{throw new Error}catch(h){"stack"in h&&(t(8),t(7),"addEventListener"in window&&t(5),c.xhrWrappable&&t(9),d=!0)}s.on("fn-start",function(t,n,e){d&&(p+=1)}),s.on("fn-err",function(t,n,e){d&&!e[l]&&(f(e,l,function(){return!0}),this.thrown=!0,o(e))}),s.on("fn-end",function(){d&&!this.thrown&&p>0&&(p-=1)}),s.on("internal-error",function(t){i("ierr",[t,c.now(),!0])})},{}],3:[function(t,n,e){t("loader").features.ins=!0},{}],4:[function(t,n,e){function r(t){}if(window.performance&&window.performance.timing&&window.performance.getEntriesByType){var o=t("ee"),i=t("handle"),a=t(8),s=t(7),c="learResourceTimings",f="addEventListener",u="resourcetimingbufferfull",d="bstResource",l="resource",p="-start",h="-end",m="fn"+p,v="fn"+h,w="bstTimer",y="pushState",g=t("loader");g.features.stn=!0,t(6);var b=NREUM.o.EV;o.on(m,function(t,n){var e=t[0];e instanceof b&&(this.bstStart=g.now())}),o.on(v,function(t,n){var e=t[0];e instanceof b&&i("bst",[e,n,this.bstStart,g.now()])}),a.on(m,function(t,n,e){this.bstStart=g.now(),this.bstType=e}),a.on(v,function(t,n){i(w,[n,this.bstStart,g.now(),this.bstType])}),s.on(m,function(){this.bstStart=g.now()}),s.on(v,function(t,n){i(w,[n,this.bstStart,g.now(),"requestAnimationFrame"])}),o.on(y+p,function(t){this.time=g.now(),this.startPath=location.pathname+location.hash}),o.on(y+h,function(t){i("bstHist",[location.pathname+location.hash,this.startPath,this.time])}),f in window.performance&&(window.performance["c"+c]?window.performance[f](u,function(t){i(d,[window.performance.getEntriesByType(l)]),window.performance["c"+c]()},!1):window.performance[f]("webkit"+u,function(t){i(d,[window.performance.getEntriesByType(l)]),window.performance["webkitC"+c]()},!1)),document[f]("scroll",r,{passive:!0}),document[f]("keypress",r,!1),document[f]("click",r,!1)}},{}],5:[function(t,n,e){function r(t){for(var n=t;n&&!n.hasOwnProperty(u);)n=Object.getPrototypeOf(n);n&&o(n)}function o(t){s.inPlace(t,[u,d],"-",i)}function i(t,n){return t[1]}var a=t("ee").get("events"),s=t(19)(a,!0),c=t("gos"),f=XMLHttpRequest,u="addEventListener",d="removeEventListener";n.exports=a,"getPrototypeOf"in Object?(r(document),r(window),r(f.prototype)):f.prototype.hasOwnProperty(u)&&(o(window),o(f.prototype)),a.on(u+"-start",function(t,n){var e=t[1],r=c(e,"nr@wrapped",function(){function t(){if("function"==typeof e.handleEvent)return e.handleEvent.apply(e,arguments)}var n={object:t,"function":e}[typeof e];return n?s(n,"fn-",null,n.name||"anonymous"):e});this.wrapped=t[1]=r}),a.on(d+"-start",function(t){t[1]=this.wrapped||t[1]})},{}],6:[function(t,n,e){var r=t("ee").get("history"),o=t(19)(r);n.exports=r,o.inPlace(window.history,["pushState","replaceState"],"-")},{}],7:[function(t,n,e){var r=t("ee").get("raf"),o=t(19)(r),i="equestAnimationFrame";n.exports=r,o.inPlace(window,["r"+i,"mozR"+i,"webkitR"+i,"msR"+i],"raf-"),r.on("raf-start",function(t){t[0]=o(t[0],"fn-")})},{}],8:[function(t,n,e){function r(t,n,e){t[0]=a(t[0],"fn-",null,e)}function o(t,n,e){this.method=e,this.timerDuration=isNaN(t[1])?0:+t[1],t[0]=a(t[0],"fn-",this,e)}var i=t("ee").get("timer"),a=t(19)(i),s="setTimeout",c="setInterval",f="clearTimeout",u="-start",d="-";n.exports=i,a.inPlace(window,[s,"setImmediate"],s+d),a.inPlace(window,[c],c+d),a.inPlace(window,[f,"clearImmediate"],f+d),i.on(c+u,r),i.on(s+u,o)},{}],9:[function(t,n,e){function r(t,n){d.inPlace(n,["onreadystatechange"],"fn-",s)}function o(){var t=this,n=u.context(t);t.readyState>3&&!n.resolved&&(n.resolved=!0,u.emit("xhr-resolved",[],t)),d.inPlace(t,y,"fn-",s)}function i(t){g.push(t),h&&(x?x.then(a):v?v(a):(E=-E,O.data=E))}function a(){for(var t=0;t<g.length;t++)r([],g[t]);g.length&&(g=[])}function s(t,n){return n}function c(t,n){for(var e in t)n[e]=t[e];return n}t(5);var f=t("ee"),u=f.get("xhr"),d=t(19)(u),l=NREUM.o,p=l.XHR,h=l.MO,m=l.PR,v=l.SI,w="readystatechange",y=["onload","onerror","onabort","onloadstart","onloadend","onprogress","ontimeout"],g=[];n.exports=u;var b=window.XMLHttpRequest=function(t){var n=new p(t);try{u.emit("new-xhr",[n],n),n.addEventListener(w,o,!1)}catch(e){try{u.emit("internal-error",[e])}catch(r){}}return n};if(c(p,b),b.prototype=p.prototype,d.inPlace(b.prototype,["open","send"],"-xhr-",s),u.on("send-xhr-start",function(t,n){r(t,n),i(n)}),u.on("open-xhr-start",r),h){var x=m&&m.resolve();if(!v&&!m){var E=1,O=document.createTextNode(E);new h(a).observe(O,{characterData:!0})}}else f.on("fn-end",function(t){t[0]&&t[0].type===w||a()})},{}],10:[function(t,n,e){function r(t){var n=this.params,e=this.metrics;if(!this.ended){this.ended=!0;for(var r=0;r<d;r++)t.removeEventListener(u[r],this.listener,!1);if(!n.aborted){if(e.duration=a.now()-this.startTime,4===t.readyState){n.status=t.status;var i=o(t,this.lastSize);if(i&&(e.rxSize=i),this.sameOrigin){var c=t.getResponseHeader("X-NewRelic-App-Data");c&&(n.cat=c.split(", ").pop())}}else n.status=0;e.cbTime=this.cbTime,f.emit("xhr-done",[t],t),s("xhr",[n,e,this.startTime])}}}function o(t,n){var e=t.responseType;if("json"===e&&null!==n)return n;var r="arraybuffer"===e||"blob"===e||"json"===e?t.response:t.responseText;return h(r)}function i(t,n){var e=c(n),r=t.params;r.host=e.hostname+":"+e.port,r.pathname=e.pathname,t.sameOrigin=e.sameOrigin}var a=t("loader");if(a.xhrWrappable){var s=t("handle"),c=t(11),f=t("ee"),u=["load","error","abort","timeout"],d=u.length,l=t("id"),p=t(14),h=t(13),m=window.XMLHttpRequest;a.features.xhr=!0,t(9),f.on("new-xhr",function(t){var n=this;n.totalCbs=0,n.called=0,n.cbTime=0,n.end=r,n.ended=!1,n.xhrGuids={},n.lastSize=null,p&&(p>34||p<10)||window.opera||t.addEventListener("progress",function(t){n.lastSize=t.loaded},!1)}),f.on("open-xhr-start",function(t){this.params={method:t[0]},i(this,t[1]),this.metrics={}}),f.on("open-xhr-end",function(t,n){"loader_config"in NREUM&&"xpid"in NREUM.loader_config&&this.sameOrigin&&n.setRequestHeader("X-NewRelic-ID",NREUM.loader_config.xpid)}),f.on("send-xhr-start",function(t,n){var e=this.metrics,r=t[0],o=this;if(e&&r){var i=h(r);i&&(e.txSize=i)}this.startTime=a.now(),this.listener=function(t){try{"abort"===t.type&&(o.params.aborted=!0),("load"!==t.type||o.called===o.totalCbs&&(o.onloadCalled||"function"!=typeof n.onload))&&o.end(n)}catch(e){try{f.emit("internal-error",[e])}catch(r){}}};for(var s=0;s<d;s++)n.addEventListener(u[s],this.listener,!1)}),f.on("xhr-cb-time",function(t,n,e){this.cbTime+=t,n?this.onloadCalled=!0:this.called+=1,this.called!==this.totalCbs||!this.onloadCalled&&"function"==typeof e.onload||this.end(e)}),f.on("xhr-load-added",function(t,n){var e=""+l(t)+!!n;this.xhrGuids&&!this.xhrGuids[e]&&(this.xhrGuids[e]=!0,this.totalCbs+=1)}),f.on("xhr-load-removed",function(t,n){var e=""+l(t)+!!n;this.xhrGuids&&this.xhrGuids[e]&&(delete this.xhrGuids[e],this.totalCbs-=1)}),f.on("addEventListener-end",function(t,n){n instanceof m&&"load"===t[0]&&f.emit("xhr-load-added",[t[1],t[2]],n)}),f.on("removeEventListener-end",function(t,n){n instanceof m&&"load"===t[0]&&f.emit("xhr-load-removed",[t[1],t[2]],n)}),f.on("fn-start",function(t,n,e){n instanceof m&&("onload"===e&&(this.onload=!0),("load"===(t[0]&&t[0].type)||this.onload)&&(this.xhrCbStart=a.now()))}),f.on("fn-end",function(t,n){this.xhrCbStart&&f.emit("xhr-cb-time",[a.now()-this.xhrCbStart,this.onload,n],n)})}},{}],11:[function(t,n,e){n.exports=function(t){var n=document.createElement("a"),e=window.location,r={};n.href=t,r.port=n.port;var o=n.href.split("://");!r.port&&o[1]&&(r.port=o[1].split("/")[0].split("@").pop().split(":")[1]),r.port&&"0"!==r.port||(r.port="https"===o[0]?"443":"80"),r.hostname=n.hostname||e.hostname,r.pathname=n.pathname,r.protocol=o[0],"/"!==r.pathname.charAt(0)&&(r.pathname="/"+r.pathname);var i=!n.protocol||":"===n.protocol||n.protocol===e.protocol,a=n.hostname===document.domain&&n.port===e.port;return r.sameOrigin=i&&(!n.hostname||a),r}},{}],12:[function(t,n,e){function r(){}function o(t,n,e){return function(){return i(t,[f.now()].concat(s(arguments)),n?null:this,e),n?void 0:this}}var i=t("handle"),a=t(16),s=t(17),c=t("ee").get("tracer"),f=t("loader"),u=NREUM;"undefined"==typeof window.newrelic&&(newrelic=u);var d=["setPageViewName","setCustomAttribute","setErrorHandler","finished","addToTrace","inlineHit","addRelease"],l="api-",p=l+"ixn-";a(d,function(t,n){u[n]=o(l+n,!0,"api")}),u.addPageAction=o(l+"addPageAction",!0),u.setCurrentRouteName=o(l+"routeName",!0),n.exports=newrelic,u.interaction=function(){return(new r).get()};var h=r.prototype={createTracer:function(t,n){var e={},r=this,o="function"==typeof n;return i(p+"tracer",[f.now(),t,e],r),function(){if(c.emit((o?"":"no-")+"fn-start",[f.now(),r,o],e),o)try{return n.apply(this,arguments)}catch(t){throw c.emit("fn-err",[arguments,this,t],e),t}finally{c.emit("fn-end",[f.now()],e)}}}};a("actionText,setName,setAttribute,save,ignore,onEnd,getContext,end,get".split(","),function(t,n){h[n]=o(p+n)}),newrelic.noticeError=function(t,n){"string"==typeof t&&(t=new Error(t)),i("err",[t,f.now(),!1,n])}},{}],13:[function(t,n,e){n.exports=function(t){if("string"==typeof t&&t.length)return t.length;if("object"==typeof t){if("undefined"!=typeof ArrayBuffer&&t instanceof ArrayBuffer&&t.byteLength)return t.byteLength;if("undefined"!=typeof Blob&&t instanceof Blob&&t.size)return t.size;if(!("undefined"!=typeof FormData&&t instanceof FormData))try{return JSON.stringify(t).length}catch(n){return}}}},{}],14:[function(t,n,e){var r=0,o=navigator.userAgent.match(/Firefox[\/\s](\d+\.\d+)/);o&&(r=+o[1]),n.exports=r},{}],15:[function(t,n,e){function r(t,n){if(!o)return!1;if(t!==o)return!1;if(!n)return!0;if(!i)return!1;for(var e=i.split("."),r=n.split("."),a=0;a<r.length;a++)if(r[a]!==e[a])return!1;return!0}var o=null,i=null,a=/Version\/(\S+)\s+Safari/;if(navigator.userAgent){var s=navigator.userAgent,c=s.match(a);c&&s.indexOf("Chrome")===-1&&s.indexOf("Chromium")===-1&&(o="Safari",i=c[1])}n.exports={agent:o,version:i,match:r}},{}],16:[function(t,n,e){function r(t,n){var e=[],r="",i=0;for(r in t)o.call(t,r)&&(e[i]=n(r,t[r]),i+=1);return e}var o=Object.prototype.hasOwnProperty;n.exports=r},{}],17:[function(t,n,e){function r(t,n,e){n||(n=0),"undefined"==typeof e&&(e=t?t.length:0);for(var r=-1,o=e-n||0,i=Array(o<0?0:o);++r<o;)i[r]=t[n+r];return i}n.exports=r},{}],18:[function(t,n,e){n.exports={exists:"undefined"!=typeof window.performance&&window.performance.timing&&"undefined"!=typeof window.performance.timing.navigationStart}},{}],19:[function(t,n,e){function r(t){return!(t&&t instanceof Function&&t.apply&&!t[a])}var o=t("ee"),i=t(17),a="nr@original",s=Object.prototype.hasOwnProperty,c=!1;n.exports=function(t,n){function e(t,n,e,o){function nrWrapper(){var r,a,s,c;try{a=this,r=i(arguments),s="function"==typeof e?e(r,a):e||{}}catch(f){l([f,"",[r,a,o],s])}u(n+"start",[r,a,o],s);try{return c=t.apply(a,r)}catch(d){throw u(n+"err",[r,a,d],s),d}finally{u(n+"end",[r,a,c],s)}}return r(t)?t:(n||(n=""),nrWrapper[a]=t,d(t,nrWrapper),nrWrapper)}function f(t,n,o,i){o||(o="");var a,s,c,f="-"===o.charAt(0);for(c=0;c<n.length;c++)s=n[c],a=t[s],r(a)||(t[s]=e(a,f?s+o:o,i,s))}function u(e,r,o){if(!c||n){var i=c;c=!0;try{t.emit(e,r,o,n)}catch(a){l([a,e,r,o])}c=i}}function d(t,n){if(Object.defineProperty&&Object.keys)try{var e=Object.keys(t);return e.forEach(function(e){Object.defineProperty(n,e,{get:function(){return t[e]},set:function(n){return t[e]=n,n}})}),n}catch(r){l([r])}for(var o in t)s.call(t,o)&&(n[o]=t[o]);return n}function l(n){try{t.emit("internal-error",n)}catch(e){}}return t||(t=o),e.inPlace=f,e.flag=a,e}},{}],ee:[function(t,n,e){function r(){}function o(t){function n(t){return t&&t instanceof r?t:t?c(t,s,i):i()}function e(e,r,o,i){if(!l.aborted||i){t&&t(e,r,o);for(var a=n(o),s=m(e),c=s.length,f=0;f<c;f++)s[f].apply(a,r);var d=u[g[e]];return d&&d.push([b,e,r,a]),a}}function p(t,n){y[t]=m(t).concat(n)}function h(t,n){var e=y[t];if(e)for(var r=0;r<e.length;r++)e[r]===n&&e.splice(r,1)}function m(t){return y[t]||[]}function v(t){return d[t]=d[t]||o(e)}function w(t,n){f(t,function(t,e){n=n||"feature",g[e]=n,n in u||(u[n]=[])})}var y={},g={},b={on:p,addEventListener:p,removeEventListener:h,emit:e,get:v,listeners:m,context:n,buffer:w,abort:a,aborted:!1};return b}function i(){return new r}function a(){(u.api||u.feature)&&(l.aborted=!0,u=l.backlog={})}var s="nr@context",c=t("gos"),f=t(16),u={},d={},l=n.exports=o();l.backlog=u},{}],gos:[function(t,n,e){function r(t,n,e){if(o.call(t,n))return t[n];var r=e();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(t,n,{value:r,writable:!0,enumerable:!1}),r}catch(i){}return t[n]=r,r}var o=Object.prototype.hasOwnProperty;n.exports=r},{}],handle:[function(t,n,e){function r(t,n,e,r){o.buffer([t],r),o.emit(t,n,e)}var o=t("ee").get("handle");n.exports=r,r.ee=o},{}],id:[function(t,n,e){function r(t){var n=typeof t;return!t||"object"!==n&&"function"!==n?-1:t===window?0:a(t,i,function(){return o++})}var o=1,i="nr@id",a=t("gos");n.exports=r},{}],loader:[function(t,n,e){function r(){if(!E++){var t=x.info=NREUM.info,n=p.getElementsByTagName("script")[0];if(setTimeout(u.abort,3e4),!(t&&t.licenseKey&&t.applicationID&&n))return u.abort();f(g,function(n,e){t[n]||(t[n]=e)}),c("mark",["onload",a()+x.offset],null,"api");var e=p.createElement("script");e.src="https://"+t.agent,n.parentNode.insertBefore(e,n)}}function o(){"complete"===p.readyState&&i()}function i(){c("mark",["domContent",a()+x.offset],null,"api")}function a(){return O.exists&&performance.now?Math.round(performance.now()):(s=Math.max((new Date).getTime(),s))-x.offset}var s=(new Date).getTime(),c=t("handle"),f=t(16),u=t("ee"),d=t(15),l=window,p=l.document,h="addEventListener",m="attachEvent",v=l.XMLHttpRequest,w=v&&v.prototype;NREUM.o={ST:setTimeout,SI:l.setImmediate,CT:clearTimeout,XHR:v,REQ:l.Request,EV:l.Event,PR:l.Promise,MO:l.MutationObserver};var y=""+location,g={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-1118.min.js"},b=v&&w&&w[h]&&!/CriOS/.test(navigator.userAgent),x=n.exports={offset:s,now:a,origin:y,features:{},xhrWrappable:b,userAgent:d};t(12),p[h]?(p[h]("DOMContentLoaded",i,!1),l[h]("load",r,!1)):(p[m]("onreadystatechange",o),l[m]("onload",r)),c("mark",["firstbyte",s],null,"api");var E=0,O=t(18)},{}]},{},["loader",2,10,4,3]);</script>
		<!--@@TELERIK_RAD_CODE_BLOCK_START@@-->
		

        <!-- Important: include as high up as possible, but after sensitive tags such as X-UA-Compatible -->
        <title>Eye on Psi Chi: Winter 2001 - Psi Chi, The International Honor Society in Psychology</title>

        <link rel="stylesheet" type="text/css" href="https://cdn.ymaws.com/psichi.site-ym.com/css/20180829/sp/combined_v358.css">
		<link rel="stylesheet" type="text/css" href="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/container/assets/skins/sam/container.css">
		<link rel="stylesheet" type="text/css" href="/global_graphics/skins/MemberCustomPageMenu/yuimenu.css">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css">
        <!--[if IE]><link rel="stylesheet" type="text/css" href="/global_inc/site_templates/YM-IM-04/ie.css">
		<style type="text/css">
			#CustomPageBody,
			div.ContributedContent {
				padding-bottom: expression(this.scrollWidth > this.offsetWidth ? 17 : 0); }
		</style><![endif]-->
		
		<!--@@DG_PRINT_BASE_URL@@
			IMPORTANT! DO NOT MOVE OR MODIFY -->

		

		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/yahoo-dom-event/yahoo-dom-event.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/dragdrop/dragdrop-min.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/container/container-min.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/menu/menu-min.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/yui/2.9.0/build/json/json-min.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.8.18/jquery-ui.min.js"></script>
        <script type="text/javascript" src="https://cdn.ymaws.com/global/js/20180829/frontend/combined.js"></script>

		<script type='text/javascript'>
			var _gaq = _gaq || [];_gaq.push(['_setAccount', 'UA-12891745-1'], ['_setDomainName', 'none'], ['_setAllowLinker', true], ['_trackPageview']);_gaq.push(['YM._setAccount', 'UA-2449742-47'], ['YM._setDomainName', 'none'], ['YM._setAllowLinker', true], ['YM._trackPageview']);
			(function() {
		        var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
		        ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
		        var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
	            })();
			</script>
	
		<script type="text/javascript">
			addEventHandler_OnLoad(function(){CheckMultipartForms(true)});
		
			var m_pulse = new Pulse('');
			m_pulse.Start();
		</script>
	
		
		<!--@@TELERIK_RAD_CODE_BLOCK_END@@-->
	</head>


				<!-- Copyright (c) OpenGlobal. GNU/GPL licence. You may copy and modify this, providing the link to http://www.openglobal.co.uk remains intact. -->
				<div id="openglobal_privacy_widget" class="privacy-widget">
                This website uses cookies to store information on your computer. Some of these cookies are used for visitor analysis, others are essential to making our site function properly and improve the user experience. By using this site, you consent to the placement of these cookies. Click Accept to consent and dismiss this message or Deny to leave this website. Read our <a href="/Privacy_Statement.aspx" target="_blank">Privacy Statement</a> for more.
                <div style="margin-top:15px;">
                <button id="openglobal_privacy_accept" class="formbutton btn btn-primary" onclick="openglobal_privacy_accept();return false;">Accept</button>
                <button id="openglobal_privacy_leave" class="formbutton btn btn-default" style="margin-left:10px;" onclick="window.location='https://www.google.com';">Deny</button>
                </div>
                </div>
				<script type="text/javascript">
				//<![CDATA[
				var openglobal_privacy_timeout = 0;
				var openglobal_privacy_functions = [];

				var openglobal_privacy_widget = document.getElementById('openglobal_privacy_widget');
				var results = document.cookie.match ( '(^|;) ?openglobal_privacy_widget=([^;]*)(;|$)' );
				if (results) {
				  if (1 == unescape(results[2])) {
					openglobal_privacy_accept();
				  }
				}

				function openglobal_privacy_accept() {
				  document.cookie = 'openglobal_privacy_widget=1; path=/; expires=Mon, 18 Jan 2038 03:14:00 GMT';
				  openglobal_privacy_widget.parentNode.removeChild(openglobal_privacy_widget);
				  for (var i = 0; i < openglobal_privacy_functions.length; i++) {
					openglobal_privacy_functions[i]();
				  }
				}
				//]]>
				</script>

<!--<link rel="stylesheet" type="text/css" href="http://yui.yahooapis.com/3.3.0/build/cssreset/reset-min.css">-->



<body id="PageBody" onunload="try{if(m_blnDoBodyUnload) Body_OnUnload();}catch(e){}">
	<div id="icontainer">
		<div id="icontent">
            <div id="LeaderContentArea">
                <!--YMPSTITLE=TgBBAA==/YMPSTITLE--><div id="iheader"><a class="logo" href="/" target="_parent" style="color:#000;"></a></div>
            </div>
			<div id="topbar">
				<div id="inavigation"><div id="FrontendMainMenu" class="radmenu RadMenu_YMPublic ">
	<!-- 4.3.2 --><script type="text/javascript" src="/global_inc/RadControls/Menu/Scripts/4_3_2/RadMenu.js"></script><span id="FrontendMainMenuStyleSheetHolder" style="display:none;"></span><script type="text/javascript">RadControlsNamespace.AppendStyleSheet(false, 'FrontendMainMenu', '/global_inc/RadControls/Menu/Scripts/4_3_2/menu.css');</script><script type="text/javascript">RadControlsNamespace.AppendStyleSheet(false, 'FrontendMainMenu', '/global_inc/RadControls/Menu/Skins/YMPublic/styles.css');</script><ul class="horizontal rootGroup">
		<li class="item first"><a href="/?page=about" id="FrontendMainMenu_m0" class="link"><span class="text">About</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=welcome" id="FrontendMainMenu_m0_m0" class="link"><span class="text">Welcome to Psi Chi</span></a></li><li class="item"><a href="/?page=purpose" id="FrontendMainMenu_m0_m1" class="link"><span class="text">Mission & Purpose</span></a></li><li class="item"><a href="/?page=manchap_constitution" id="FrontendMainMenu_m0_m2" class="link"><span class="text">Constitution</span></a></li><li class="item"><a href="/?page=timeline" id="FrontendMainMenu_m0_m3" class="link"><span class="text">History Timeline</span></a></li><li class="item"><a href="/?page=board" id="FrontendMainMenu_m0_m4" class="link"><span class="text">Board of Directors</span></a></li><li class="item"><a href="/?page=staff" id="FrontendMainMenu_m0_m5" class="link"><span class="text">Central Office Staff</span></a></li><li class="item"><a href="#" target="_blank" id="FrontendMainMenu_m0_m6" class="link"><span class="text">Committees</span></a><div class="slide">
					<ul class="vertical group level2">
						<li class="item first"><a href="/?page=Diversity" id="FrontendMainMenu_m0_m6_m0" class="link"><span class="text">Diversity Committee</span></a></li><li class="item"><a href="/?page=international_news " id="FrontendMainMenu_m0_m6_m1" class="link"><span class="text">International Committee</span></a></li><li class="item last"><a href="/?ResearchAdvisory" id="FrontendMainMenu_m0_m6_m2" class="link"><span class="text">Research Committee</span></a></li>
					</ul>
				</div></li><li class="item"><a href="/?page=Partnerships" id="FrontendMainMenu_m0_m7" class="link"><span class="text">Sponsors</span></a></li><li class="item last"><a href="https://donate.psichi.org/campaign/give-back-to-psi-chi/c187764" id="FrontendMainMenu_m0_m8" class="link"><span class="text">Donations</span></a><div class="slide">
					<ul class="vertical group level2">
						<li class="item first"><a href="https://donate.psichi.org/campaign/give-back-to-psi-chi/c187764" target="_blank" id="FrontendMainMenu_m0_m8_m0" class="link"><span class="text">Donate Now</span></a></li><li class="item"><a href="/page/LegacyGiving" id="FrontendMainMenu_m0_m8_m1" class="link"><span class="text">Legacy Giving</span></a></li><li class="item last"><a href="resource/resmgr/pdfs/waystogive-final.pdf" target="_blank" id="FrontendMainMenu_m0_m8_m2" class="link"><span class="text">Ways to Give</span></a></li>
					</ul>
				</div></li>
			</ul>
		</div></li><li class="item"><a href="/?page=join" id="FrontendMainMenu_m1" class="link"><span class="text">Member</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=member_benefits" id="FrontendMainMenu_m1_m0" class="link"><span class="text">Benefits of Membership</span></a></li><li class="item"><a href="/?page=become_member" id="FrontendMainMenu_m1_m1" class="link"><span class="text">Become a Member</span></a></li><li class="item"><a href="/?page=undergraduate" id="FrontendMainMenu_m1_m2" class="link"><span class="text">Undergraduate</span></a></li><li class="item"><a href="/?page=graduate" id="FrontendMainMenu_m1_m3" class="link"><span class="text">Graduate</span></a></li><li class="item"><a href="/?page=faculty" id="FrontendMainMenu_m1_m4" class="link"><span class="text">Faculty</span></a></li><li class="item"><a href="/?page=alumni" id="FrontendMainMenu_m1_m5" class="link"><span class="text">Alumni</span></a></li><li class="item"><a href="/?Dist_Members" id="FrontendMainMenu_m1_m6" class="link"><span class="text">Distinguished Member</span></a></li><li class="item last"><a href="/search/custom.asp?id=2163" id="FrontendMainMenu_m1_m7" class="link"><span class="text">Member Search</span></a></li>
			</ul>
		</div></li><li class="item"><a href="/?page=memberchapter_main" id="FrontendMainMenu_m2" class="link"><span class="text">Chapter</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=start_chapter" id="FrontendMainMenu_m2_m0" class="link"><span class="text">Start a Chapter</span></a></li><li class="item"><a href="/?page=chapter_search" id="FrontendMainMenu_m2_m1" class="link"><span class="text">Chapter Directory Search</span></a></li><li class="item"><a href="/?page=chapter_leader" id="FrontendMainMenu_m2_m2" class="link"><span class="text">Chapter Leadership</span></a></li><li class="item"><a href="/?page=chapter_service" id="FrontendMainMenu_m2_m3" class="link"><span class="text">Chapter Service Projects</span></a></li><li class="item last"><a href="/?page=ConductingResearch" id="FrontendMainMenu_m2_m4" class="link"><span class="text">Conducting Research</span></a></li>
			</ul>
		</div></li><li class="item"><a href="/?page=regions_main" id="FrontendMainMenu_m3" class="link"><span class="text">Conventions</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=reg_east_letter" id="FrontendMainMenu_m3_m0" class="link"><span class="text">Eastern</span></a></li><li class="item"><a href="/?page=reg_midwest_letter" id="FrontendMainMenu_m3_m1" class="link"><span class="text">Midwestern</span></a></li><li class="item"><a href="/?page=reg_rckymtn_letter" id="FrontendMainMenu_m3_m2" class="link"><span class="text">Rocky Mountain</span></a></li><li class="item"><a href="/?page=reg_southeast_letter" id="FrontendMainMenu_m3_m3" class="link"><span class="text">Southeastern</span></a></li><li class="item"><a href="/?page=reg_southwest_letter" id="FrontendMainMenu_m3_m4" class="link"><span class="text">Southwestern</span></a></li><li class="item"><a href="/?page=reg_west_letter" id="FrontendMainMenu_m3_m5" class="link"><span class="text">Western</span></a></li><li class="item"><a href="/?page=APS_APA" id="FrontendMainMenu_m3_m6" class="link"><span class="text">National</span></a></li><li class="item last"><a href="/?page=international_news" id="FrontendMainMenu_m3_m7" class="link"><span class="text">International</span></a></li>
			</ul>
		</div></li><li class="item"><a href="/?page=awards" id="FrontendMainMenu_m4" class="link"><span class="text">Awards/Grants</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=1_undergrad_main" id="FrontendMainMenu_m4_m0" class="link"><span class="text">Undergraduate</span></a></li><li class="item"><a href="/?page=2_graduate_main" id="FrontendMainMenu_m4_m1" class="link"><span class="text">Graduate </span></a></li><li class="item"><a href="/?page=3_chapter_main" id="FrontendMainMenu_m4_m2" class="link"><span class="text">Chapter</span></a></li><li class="item"><a href="/?page=4_faculty_main" id="FrontendMainMenu_m4_m3" class="link"><span class="text">Faculty</span></a></li><li class="item last"><a href="/?page=CopyofA_IndvAwardT" id="FrontendMainMenu_m4_m4" class="link"><span class="text">Reviewers</span></a></li>
			</ul>
		</div></li><li class="item"><a href="/?page=news" id="FrontendMainMenu_m5" class="link"><span class="text">Publications/News</span></a><div class="slide">
			<ul class="vertical group level1">
				<li class="item first"><a href="/?page=journal_main" id="FrontendMainMenu_m5_m0" class="link"><span class="text">Journal</span></a></li><li class="item"><a href="/?page=eye_main" id="FrontendMainMenu_m5_m1" class="link"><span class="text">Magazine</span></a></li><li class="item"><a href="/page/Ology_0101_Intro#.WJo-mn-0koV" id="FrontendMainMenu_m5_m2" class="link"><span class="text">Blog</span></a></li><li class="item"><a href="/?page=digest" id="FrontendMainMenu_m5_m3" class="link"><span class="text">News/Digest</span></a></li><li class="item last"><a href="/?page=Advertise" id="FrontendMainMenu_m5_m4" class="link"><span class="text">Advertise</span></a></li>
			</ul>
		</div></li><li class="item last"><a href="/page/Merch_ITM_Grad" id="FrontendMainMenu_m6" class="link"><span class="text">Store</span></a></li>
	</ul><input type="hidden" id="FrontendMainMenu_Hidden" name="FrontendMainMenu" /><script type="text/javascript">window["FrontendMainMenu"] = RadMenu.Create("FrontendMainMenu");window["FrontendMainMenu"].Initialize({"EnableAutoScroll":true,"Skin":"YMPublic","Enabled":true},{"FrontendMainMenu_m0_m6":{"NavigateAfterClick":false}});</script>
</div><link rel="stylesheet" type="text/css" href="/global_inc/RadControls/Menu/Scripts/4_3_2/menu.css"/><link rel="stylesheet" type="text/css" href="/global_inc/RadControls/Menu/Skins/YMPublic/styles.css"/></div>
				
					<div id="isearch"><form id="QuickSearchForm" name="QuickSearchForm" action="/search/all.asp">
		<div id="QuickSearchFormInner1" class="ui-widget">
			<input id="QuickSearchForm_bst" name="bst" maxlength='50' value='Enter search criteria...'@"onfocus='QuickSearchForm_OnFocus();'/>
		</div>
		<div id='QuickSearchFormInner2'><a href='#' id='QuickSearchSubmit' onclick='return QuickSearchForm_DoSubmit();'>Search&nbsp;&raquo;</a></div>
</form><script type="text/javascript">
function QuickSearchForm_DoSubmit()
{
		var QuickSearchForm = document.QuickSearchForm;
     if(QuickSearchForm)
     {
			ClearDefaultValue(QuickSearchForm.bst);
         QuickSearchForm.submit();
     }
		return false;
}
$(document).ready(function ()
{
		$("#QuickSearchForm_bst").click(function()
		{
			if ($("#QuickSearchForm_bst").val() == "Enter search criteria...")
				$("#QuickSearchForm_bst").val('');
			});
			$("#QuickSearchForm_bst").blur(function ()
			{
				if ($("#QuickSearchForm_bst").val() == '')
					$("#QuickSearchForm_bst").val('Enter search criteria...');
			});
	});
</script></div>
				
			</div>

			<div id="iheader"><script type="text/javascript">
  WebFontConfig = {
    google: { families: [ 'Roboto:400,500,700:latin', 'Roboto+Condensed:400,700:latin', 'Roboto+Slab:400,700:latin' ] }
  };
  (function() {
    var wf = document.createElement('script');
    wf.src = ('https:' == document.location.protocol ? 'https' : 'http') +
      '://ajax.googleapis.com/ajax/libs/webfont/1/webfont.js';
    wf.type = 'text/javascript';
    wf.async = 'true';
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(wf, s);
  })(); </script>
<div id="header">
	<a href="/" id="logo"></a>
</div>
<style type='text/css'>#Head{background-image:url('https://cdn.ymaws.com/psichi.site-ym.com/graphics/bg_top.gif');}</style></div>
			
			<div id="itoolbar_bg">
				<div id="itoolbar"><a id="PrintPage" href="#" onclick="return false;" title="Print view will be available once the page has finished loading."><img src="/global_graphics/icons/print_bw.gif" border="0" height="16" width="16" style="margin:5px 5px 0 0;valign:bottom;" />Print Page</a><script type='text/javascript'>function PrintPageClickHandler(){this.handleEvent = createPrintPagePopup }PrintPage_OnClick = new PrintPageClickHandler(); addEventHandler_OnLoad(function(){ var element = document.getElementById("PrintPage"); if(element) { element.onclick = PrintPage_OnClick.handleEvent; element.title = "Print Page";} });</script> &nbsp; | &nbsp; <a href='/general/?type=CONTACT'>Contact Us</a> &nbsp; | &nbsp; <a href='/login.aspx'>Sign In</a> &nbsp; | &nbsp; <a href='/general/register_start.asp'>Register</a></div>
			</div>
	
		<div id="sp-content">
			<div id="left">
				<!--@@DG_PRINT_PAGE_BEGIN@@
					IMPORTANT! DO NOT MOVE OR MODIFY -->
				
  <script type="text/javascript">var blnUseEngagement = false; </script> 
  
<script type="text/javascript" src="/global_inc/js/favorite.js"></script>


<style type="text/css">
	#tat_table {
		z-index:99;
	}
	#FavoriteEditorTitle {
		margin: 0;
	}
</style>
<div class="yui-skin-sam">
<div id="FavoriteOptsPanel" style="visibility:hidden;">
	<div id="FavoriteOptsPanelBody" class="bd">
		<div id="FormErrors" style="display:none">
			<div class="infobox">
				<ul id="FormErrorList" class="redalert"></ul>
			</div><br>
		</div>
			<form id="FavoriteEditor" name="FavoriteEditor" onsubmit="return FavoriteEditor_Submit(this)" style="display:none; margin: 0 10px 0 10px;">
			<input type="hidden" id="FavoriteID" name="FavoriteID" value="">
			<input type="hidden" id="strFavoriteTypeID_FK" name="strFavoriteTypeID_FK" value="">
			<input type="hidden" id="strFavoriteParameters" name="strFavoriteParameters" value="">
			<input type="hidden" name="strCommand" value="">
			<input type="hidden" id="blnFavoriteReload" value="">
			<table border="0" cellspacing="12" cellpadding="0">
				<tr>
					<td align="center">
            
               <img src="/global_graphics/icons/star_32x32.gif" border="0" width="32" height="32">
            
              </td>
					<td><h2 id="FavoriteEditorTitle">
            
               Edit This Favorite
            
              </h2></td>
				</tr>
				<tr>
					<td>Name:</td>
					<td><input type="text" id="strTitle" name="strTitle" value="" size="40" maxlength="100" />
					<INPUT TYPE="hidden" NAME="ERR_strTitle" VALUE="strTitle|Name|20|1||100">
					</td>
				</tr>
				<tr>
					<td>Category:</td>
					<td>
						<input type="text" id="strCategory" name="strCategory" value="" size="40" autocomplete="off" maxlength="100" />
						<INPUT TYPE="hidden" NAME="ERR_strCategory" VALUE="strCategory|Category|20|0||100">
					</td>
				</tr>
				<tr>
					<td>Share:</td>
					<td>
						<input id="blnIsPrivate0" type="radio" value="0" name="blnIsPrivate"/><label for="blnIsPrivate0">Yes</label>
						<input id="blnIsPrivate1" type="radio" value="1" name="blnIsPrivate"/><label for="blnIsPrivate1">No, Keep Private</label>
						<INPUT TYPE="hidden" NAME="ERR_blnIsPrivate" VALUE="blnIsPrivate|Share -- Yes/No, Keep Private|20|1||0">
					</td>
				</tr>
				<tr>
					<td colspan="2" align="center" style="padding-top:10px;">
						<input type="submit" id="FavoriteEditor_btnSubmit" value="Submit" class="formbutton"
							onclick="return FavoriteEditor_btnSubmit_OnClick(this);">
						<input type="button" value="Cancel" class="formbutton" 
							onclick="YAHOO.container.FavoriteOpts.hide();">
						<input type="submit" id="FavoriteEditor_btnDelete" value="Delete" class="formbutton" style="display:none;"
							onclick="return FavoriteEditor_btnDelete_OnClick(this);">
					</td>
				</tr>
			</table>
			<input type="hidden" name="__ASPVIEWSTATE" value="80e9e640e39fcac5d0ee585160149c83b6d5b7c056b5b0e0702cc7efad12a6145ffb88205c33d9396ab497e12c2c82931214b6f3326d12d42ef1cae7549469c84617f815e0ea43165caeb93f52c25f1e9e7781bba9e0d2c763b5bd9be1a7593a30b6d88d4803c2d9cecb8a0caad64063f53d435618d9d0ec4b15e507a2c8c07facd0af46">
			</form>
	</div>
</div></div>



<script type="text/javascript" src="/global_inc/js/hit_highlighter.js"></script>
<script type="text/javascript">

    function Window_OnLoad() {
		highlightDtSearchTerms('CustomPageBody');
		highlightDtSearchTerms('ResourceCollection');
	}

	addEventHandler_OnLoad(Window_OnLoad);
</script>

<style type="text/css">

.ScoreControl
{
	display:block;
	float:left;
}
</style>

<table id="SpSubHead" border="0" cellpadding="0" cellspacing="0">
<tr>
	<td id="SpTitleBar">
Eye on Psi Chi: Winter 2001
	</td>
</tr>


</table>

<table id="SpContent" border="0" cellpadding="0" cellspacing="0">
<tr>
	<td id="SpContent_Container">

		<script type="text/javascript" src="/global_inc/js/ContentScores.js"></script>
	
	<div id="CustomPageBody"><style type="text/css">
#right-col { width:172px; height: auto; float:right; vertical-align:top; margin-right:22px !important; clear:both;}
#SpContent_Container {background-image:url(/graphics/right-col-bg.jpg); background-repeat:repeat-y; background-size:222px; background-position:right; padding: 0px 0px 16px 0px !important;}
.pg-content {float:left; margin-top: -2px; padding:0px 0px 10px 0px; margin-right:30px; margin-left:29px; width:474px; vertical-align:top;}
.right-top {background-image:url(/graphics/right-col-bg-top.jpg); background-repeat:no-repeat; background-position:top left; }
#CustomPageBody {overflow:hidden !important;}
#SpNavBar {float:left !important; width:200px !important;}
#right-col-top {background-image:url(/graphics/right-col-bg-top.jpg); background-repeat:no-repeat; background-position:top; width:222px; height:25px; float:right; margin-top: -5px;} 
.calloutbox {display: none;}
</style>


<div id="right-col-top"></div><table>
<tbody>
<tr>
<td valign="top">
<div class="pg-content"></div><div style="line-height: 22px;" class="pg-content"><img style="" src="/resource/resmgr/Eye_Images3/5_2matlin474s.jpg"><table style="width: 100%; border-collapse: collapse;"><tbody><tr align="center"><td style="border-top: 5px solid rgb(82, 97, 172); letter-spacing: 0px; word-spacing: 0px; padding-bottom: 20px; font-family: Georgia; font-size: 24pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(0, 0, 0); text-align: center; padding-top: 20px; line-height: 32px;"><span style="color: rgb(82, 97, 172);"><span style="font-family: Georgia; font-size: 24pt; font-weight: normal; font-style: normal; text-decoration: none;">Demystifying the GRE Psychology Test: <br>A Brief Guide for Students </span></span><br></td></tr><tr align="center"><td style="border-top: 1px solid rgb(105, 105, 105); font-size: 10pt; font-style: normal; font-weight: bold; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; padding-top: 5px; text-align: center; padding-bottom: 5px;">Margaret W. Matlin State University of New York at Geneseo<br>James W. Kalat, North Carolina State University <br></td></tr><tr><td style="border-top: 1px solid rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; padding-top: 10px;"><br></td></tr></tbody></table><span style="color: rgb(105, 105, 105);"><p></p><p align="left">In the United States, about half of doctoral-level psychology programs and a third of master's-level programs require applicants to submit scores from the Graduate Records Examination (GRE) Psychology Test. Still other programs recommend the GRE Psychology Test, but they do not require it (Norcross, Hanych, &amp; Terranova, 1996).</p><p align="left">Undergraduate students typically find that psychology professors do not have much information about the GRE Psychology Test. Most of the information we'll discuss in this article is available in free but seldom-read publications from Educational Testing Service<sup>1</sup> (P.O. Box 6000, Princeton, NJ 08541-0001). The rest comes from our combined experience in serving on the committee that guides the development of the GRE Psychology Test. (James Kalat served as the committee chair from 1990 to 1998, and Margaret Matlin became the committee chair in 1998.)</p><p align="left">The GRE Psychology Test is a paper-based test in a multiple-choice format, with five choices per item. The test includes about 215 items; students are allotted 2 hours and 50 minutes to complete the test. The GRE Psychology Test is administered on three dates each year, at test locations throughout the world. In the present article, we will discuss how the GRE Psychology Test is scored and how the test is developed, as well as information on the test's usefulness.</p><p align="left"><span style="font-weight: bold; color: rgb(82, 97, 172);">The Scoring System for the GRE Psychology Test</span><br>The GRE Psychology Test is designed to be challenging. You may be accustomed to earning scores in the neighborhood of 90% on the examinations in your psychology courses. As a result, you may worry about the large number of items that you cannot answer. Here's some reassuring information: You can earn a score of 500 on the GRE Psychology Test by answering 43% of the questions correctly, answering 25% of the questions incorrectly, and leaving 32% of the questions unanswered (Graduate Records Examination Board, 1999b, p. 7). Remember, too, that students who take the GRE Psychology Test constitute a selected sample of all psychology undergraduates. Keep in mind, then, that a score of 90% correct on this exam would be extremely unusual!</p><p align="left">The mean score on the GRE Psychology Test is 554, with a standard deviation of 99, based on the performance of all examinees who took the test between October 1, 1995, and September 30, 1998 (Graduate Records Examinations Programs, 1999a, p. 15). The reliability of the test is .95, as estimated in an analysis of a sample of 4,130 scores (Graduate Record Examinations Board, 1999a, p. 22). The 99th percentile on this test starts at 770; a score of 340 is in the first percentile.</p><p align="left">Your score on the GRE Psychology Test will be based on the number of questions you answered correctly, minus one fourth of the questions you answered incorrectly (Graduate Records Examination Board, 1999b, p. 4). The question often arises: Should you guess when you do not know the answer? This question has a complex answer. Many students believe that this formula will hurt them if they guess, rather than omitting an answer. Across all examinees who take the test, the mean score of the whole population will not be affected by random guessing. That is, the number of points gained by guessing will be balanced by the correction factor for incorrect answers. However, by chance, some <span style="font-style: italic;">individual</span> students will lose points by guessing (and other students will gain points by guessing).</p><p align="left">What should you do if you can eliminate one or more of the five possible answers, or if one answer seems like a slightly better guess than the others. Here, your chances of answering correctly are improved. In these cases, you should certainly fill in an answer, because this type of "strategic guessing" may indeed improve your score.</p><p align="left"><span style="font-weight: bold; color: rgb(82, 97, 172);">Who Prepares the GRE Psychology Test, and How</span><br>Most psychology faculty members do not know how the GRE Psychology Test is prepared. In fact, neither of us knew about the procedures when we were initially asked to serve on the committee. The GRE Program of the Educational Testing Service (ETS) appoints a committee of six psychology faculty members from U.S. colleges and universities. The committee members are selected to be diverse in terms of their research specialties, the geographic location of their universities, and so forth. Furthermore, they must have a broad background in psychology as a whole, in addition to expertise in just a single area.</p><p align="left">Each committee member writes about 15 potential test questions per year. The ETS test developers also invite other faculty members to write additional questions. The committee members individually review the hundreds of questions that are submitted each year. Then they meet for a three-day session once a year to discuss each question. During this session, they review whether the question addresses an important issue, whether it is clearly stated, and whether the question has only one correct answer.</p><p align="left">On the GRE Psychology Test, 40% of the questions deal with material in cognition, sensation and perception, learning, and biological psychology; another 43% deal with social psychology, personality, development, and abnormal behavior. The remaining 17% cover material such as research methods, history of psychology, and applied psychology. On the actual test, however, the three types of questions are distributed throughout, rather than appearing in three separate sections. Your overall score for the GRE Psychology Test is based on questions from all three of these areas. </p><p align="left">After each administration of the test<span style="font-size: 11pt; font-family: Times New Roman;">—</span>and before scores are reported at ETS<span style="font-size: 11pt; font-family: Times New Roman;">—</span>statisticians at ETS calculate extensive statistics on each question. The information includes the percent of students who answered each question correctly, the point biserial (that is, the correlation between performance on that question and performance on the test as a whole), and information on how well the students who selected each choice for a given item performed on the rest of the test. For example, the results might indicate that the students who chose answer "B"<span style="font-size: 11pt; font-family: Times New Roman;">—</span>the correct answer<span style="font-size: 11pt; font-family: Times New Roman;">—</span>had the highest overall scores on the test, whereas those who answered "D" had the worst. These statistics call attention to items with possible problems, and almost any test has a small number of these items. Mostly, these are cases in which the point biserial is less than .30, and a large percentage of the best students had marked a choice other than the intended correct answer.</p><p align="left">The staff then consults with committee members to decide whether the item might have a second acceptable answer. Questions that are judged to be problematic are not used in computing scores. The staff at ETS continually reviews the performance of test questions. If performance patterns on a specific question change, they will stop considering that question in the scores. Furthermore, they will not use that question in future tests. A change in performance patterns may occur for many reasons. However, the most common problem occurs when new research either disproves an old theory or supports a new explanation of behavior. Thus, the GRE Psychology Test is updated to reflect changes in our knowledge about psychological phenomena.</p><p align="left"><span style="font-weight: bold; color: rgb(82, 97, 172);">How Useful is the GRE Psychology Test?</span><br>Psychology departments consider many kinds of information when they evaluate applicants for admission to graduate school. They generally emphasize grade point average (GPA), GRE General Test scores, GRE Psychology Test scores, and letters of recommendation. They may also examine information such as the student's research experience, the prestige of the student's undergraduate institution, and the match between student and faculty interests (Keith-Spiegel, Tabachnick, &amp; Spiegel, 1994).</p><p align="left">The GRE Board (1999a) decided to investigate the correlation between several quantitative measures and a student's first year grades in graduate school. The Board collected quantitative data from 110 graduate departments of psychology for the years 1986 through 1990; the study was based on 1,151 students who had pursued graduate work. The data included the student's undergraduate GPA, GRE General Test scores (verbal, quantitative, and analytical), and scores on the GRE Psychology Test. Of these measures, which one would you guess correlates best with first-year grades in graduate school?</p><p align="left">As Table 1 shows, both the GRE Psychology Test and the undergraduate GPA are correlated .37 with first-year graduate grades. This equivalence is especially interesting, because the Psychology Test is based on students' performance on just one examination, whereas the undergraduate GPA is established over four years of college courses. Table 1 also shows that scores on the GRE Psychology Test are more highly correlated with first-year graduate grades than are any of the GRE General Test measures, alone or in combination.</p><p align="left">Some researchers have argued that first-year grades may not be an appropriate measure of success in graduate school (Sternberg &amp; Williams, 1997). However, we have no evidence that other measures of success<span style="font-size: 11pt; font-family: Times New Roman;">—</span>such as faculty evaluations of graduate students<span style="font-size: 11pt; font-family: Times New Roman;">—</span>are reliable or valid (Thayer &amp; Kalat, 1998). Also, first-year grades are important because they can determine a graduate student's future. At many universities, graduate students who fail to reach some minimum criterion in their first-year grades, such as a B average, are dismissed from the program or denied financial aid.</p><p align="left">Kuncel, Hezlett, and Ones (1998) examined data on graduate students in all academic fields, not just psychology. In their meta-analysis of 201 studies of 27,039 graduate students, the GRE Subject Test was correlated .46 with first-year graduate GPA, .48 with scores on comprehensive examinations in graduate school, .53 with faculty ratings, and .21 with completion of a graduate degree. With the exception of degree completion, the GRE Subject Tests correlated more strongly with these measures than either the GRE General Test or the undergraduate GPA.</p><p align="left"><span style="font-weight: bold; color: rgb(82, 97, 172);">Future Directions of the GRE Psychology Test</span><br>Several years ago the GRE Board considered offering the Subject Tests in a computer-based format, consistent with the current GRE General Test. However, constructing the computer-based GRE General Test required adding an enormous number of new items to the test pool. The cost of constructing a similar number of new items for the Psychology Test pool would be prohibitively expensive. In other words, you can count on the paper-and-pencil format for the foreseeable future!</p><p align="left">The GRE Psychology Committee has been more concerned about another issue, the nature of the test questions. Many people<span style="font-size: 11pt; font-family: Times New Roman;">—</span>both students taking the GRE Psychology Test and the committee members themselves<span style="font-size: 11pt; font-family: Times New Roman;">—</span>have complained that the test may overemphasize rote recall of facts, some of them not especially interesting or important. Items of that kind are the easiest to write, and they usually produce decent item statistics. However, they do not reflect what most psychologists consider the best side of psychology.</p><p align="left">In recent years, the GRE Psychology Committee has tried to reduce the number of items that require simple recognition of terms or psychologists' names. We have replaced these items with more conceptual questions. However, students often obtain commercially available preparation books for the Subject Test. Some of these books contain numerous "name that psychologist" items as well as outdated "factual" questions. Students may be misled by their scores on the practice tests in these books. The books will also encourage students to use inappropriate review strategies in preparing for the GRE Psychology Test. These strategies will be especially counterproductive as the GRE Psychology Committee increases the number of conceptual questions.</p><p align="left">The official guide<span style="font-size: 11pt; font-family: Times New Roman;">—</span><span style="font-style: italic;">GRE: Practicing to Take the Psychology Test</span><span style="font-size: 11pt; font-family: Times New Roman;">—</span>will give you better information and more realistic practice items. You can order this resource from the GRE website at <a href="http://www.gre.org/" target="_blank">www.gre.org</a> or by calling 1-800-537-3160 or (609) 771-7243.</p><p align="left">Since the mid-1990s, new editions of the test have included some "analysis-of-evidence sets" among the methods items. For these questions, you will read a paragraph describing a hypothetical research study and its results. Then you'll answer two to five questions about proper conclusions to be drawn, potential weaknesses of the study as described, and ways to improve the research design or to follow up with additional research. So far, students' performance on these item sets has correlated well with the rest of the test. Future forms of the GRE Psychology Test will continue to use such items. These analysis-of-evidence items attempt to assess critical thinking, consistent with the increasing emphasis on critical thinking in psychology (e.g., Nunmedal &amp; Halpern, 1995).</p><p align="left">In summary, the GRE Psychology Test continues to evolve. With fewer factual items and a larger number of conceptual and critical-thinking items, the test will have greater content validity. As a result, the test will assess more completely those skills that psychologists value most highly in their graduate students.</p><p align="left"><span style="font-weight: bold; color: rgb(82, 97, 172);">References</span><br>Graduate Record Examinations Board. (1999a). <span style="font-style: italic;">Guide to the use of scores: Graduate Records Examinations, 1999-2000.</span> Princeton, NJ: Educational Testing Service.</p><p align="left">Graduate Record Examinations Board. (1999b). <span style="font-style: italic;">Psychology Test descriptive booklet, 1999-2001.</span> Princeton, NJ: Educational Testing Service.</p><p align="left">TKalat, J. W., &amp; Matlin, M. W. (2000). The GRE Psychology Test: A useful but poorly understood test. <span style="font-style: italic;">Teaching of Psychology, 27,</span> 23-26.</p><p align="left">Keith-Spiegel, P., Tabachnick, B. G., &amp; Spiegel, G. B. (1994). When demand exceeds supply: Second-order criteria used by graduate school selection committees. <span style="font-style: italic;">Teaching of Psychology, 21, </span>79-81.</p><p align="left">Kuncel, N. R., Hezlett, S. A., &amp; Ones, D. S. (1998, April). The predictive validity of the Graduate Record Examination: A meta-analysis. In J. P. Campbell &amp; D. S. Ones (Chairs), <span style="font-style: italic;">Selection Into I-O programs: Focus on GRE validity.</span> Symposium conducted at the 13th annual conference of the Society for Industrial and Organizational Psychology, Dallas, TX.</p><p align="left">Norcross, J. C., Hanych, J. M., &amp; Terranova, R. D. (1996). Graduate study in psychology: 1992-1993. <span style="font-style: italic;">American Psychologist, 51,</span> 631-643.</p><p align="left">Nummedal, S. G., &amp; Halpern, D. F. (1995). Introduction: Making the case for "psychologists teach critical thinking." <span style="font-style: italic;">Teaching of Psychology, 22,</span> 4-5.</p><p align="left">Sternberg, R. J., &amp; Williams, W. M. (1997). Does the Graduate Record Examination predict meaningful success in the graduate training of psychologists? A case study. <span style="font-style: italic;">American Psychologist, 52, </span>630-641.</p><p align="left">Thayer, P. W., &amp; Kalat, J. W. (1998). Questionable criteria. <span style="font-style: italic;">American Psychologist, 53,</span> 566.</p><p align="left"><a name="1"><sup>1</sup></a> The sidebar on page 25 lists Educational Testing Service publications available online at <a href="http://www.gre.org/codelst.html#reginfo" target="_blank">www.gre.org/codelst.html#sidata</a>.</p><span style="color: rgb(105, 105, 105); font-family: Arial;"></span><p></p></span></div><br><div style="line-height: 22px;" class="pg-content"><table style="width: 100%; margin-top: 20px; border-collapse: collapse;" align="" width=""><tbody><tr><td style="padding-top: 15px; padding-bottom: 15px; border-top: 1px solid rgb(105, 105, 105); font-size: 9pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; line-height: 17px;"><span style="font-family: Arial;"><span style="font-weight: bold;"><span style="font-weight: bold;"><p style="font-weight: normal; font-style: normal; text-decoration: none; letter-spacing: 0pt;"><span style="font-weight: bold;">Margaret W. Matlin</span> received her bachelor's degree from Stanford University and her PhD from the University of Michigan. She currently holds the title of Distinguished Teaching Professor of Psychology at SUNY Geneseo, where she has taught for 29 years.<br><br>M<span style="font-weight: normal;">argaret Matlin is the author of four current textbooks, </span><span style="font-style: italic; font-weight: normal;">Psychology</span><span style="font-weight: normal;"> (third edition), </span><span style="font-style: italic; font-weight: normal;">Psychology of Women</span><span style="font-weight: normal;"> (fourth edition), </span><span style="font-style: italic; font-weight: normal;">Cognition</span><span style="font-weight: normal;"> (fifth edition in press), and </span><span style="font-style: italic; font-weight: normal;">Sensation and Perception</span><span style="font-weight: normal;"> (with coauthor Hugh J. Foley, fourth edition). Dr. Matlin has also won several teaching awards, including the American Psychological Association Teaching of Psychology Award for Four-Year Institutions (1985), and the American Psychological Foundation's Distinguished Teaching in Psychology Award (1995).</span><br style="font-weight: normal;"><span style="font-weight: normal;"><br>Among Margaret Matlin's interests are travel, foreign films, and 19th-century British novels. In 1990, she and her husband, Dr. Arnold Matlin, founded a preschool educational and nutritional program in El Sauce, Nicaragua; about 300 children have subsequently attended the program.</span></p></span></span><span style="font-weight: bold;"><span style="font-weight: bold;"><p align="left"><span style="font-weight: bold;">James W. Kalat</span>,<span style="font-weight: normal;"> professor of psychology at North Carolina State University, received his PhD from the University of Pennsylvania in 1971. After a few years of doing research on taste-aversion learning in rats, he shifted his focus to textbook writing. He has written </span><span style="font-style: italic; font-weight: normal;">Biological Psychology,</span><span style="font-weight: normal;"> currently in its seventh edition, and </span><span style="font-style: italic; font-weight: normal;">Introduction to Psychology,</span><span style="font-weight: normal;"> with the sixth edition scheduled for summer 2001. Both reflect his experience in teaching both courses every semester for many years. He has served on the GRE Psychology Committee and the Convention Program Committee of the American Psychological Society. His nonacademic interests include his children, grandchildren, and birdwatching.</span></p><p align="left"></p></span></span>Authors' note.
 We thank Walter Emmerich, Robin Durso, and Judson Sheridan for their 
comments on an earlier version of this article. We also thank Heather L.
 Gitlin, Susan A. Obetz, and Dawn Robinson for their comments on this 
current article.<br><br>Send correspondence to Margaret W. Matlin, Department of Psychology, SUNY Geneseo, Geneseo, NY 14454; e-mail: <a href="mailto:matlin@geneseo.edu">matlin@geneseo.edu</a>, or to James W. Kalat, Department of Psychology, Box 7801, North Carolina State University, Raleigh, NC 27695-7801; e-mail: <a href="mailto:james_kalat@ncsu.edu">james_kalat@ncsu.edu</a>.<br><br>For
 more details on the scoring system and the test preparation, consult 
our article in the journal Teaching of Psychology (Kalat &amp; Matlin, 
2000).</span><br></td></tr><tr><td style="padding-top: 5px; border-top: 1px solid rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; font-family: Arial; font-size: 8pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); text-indent: 0px; line-height: 14px; padding-bottom: 5px;"><p>Copyright 2001 (Volume 5, Issue 2) by Psi Chi, the
International Honor Society in Psychology</p>

</td></tr><tr><td colspan="1" style="padding-top: 2px; border-top: 1px solid rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; font-family: Arial; font-size: 8pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105);"><br></td></tr></tbody></table></div><div style="line-height: 22px;" class="pg-content">&nbsp;</div><div style="line-height: 22px;" class="pg-content"><br><span style="color: rgb(105, 105, 105);"></span>



</div>

</td>


<td float="right" valign="top" width="222px">

<span style="color: rgb(105, 105, 105);">
</span><span style="color: rgb(105, 105, 105);">
</span><span style="color: rgb(105, 105, 105);">
</span><table style="width:180px; height: auto; float:right; vertical-align:top; margin-right:17px; clear:both;">
<tbody>
<tr>
<td style="line-height: 17px; font-weight: normal; font-style: normal; text-decoration: none; letter-spacing: 0px;">



<table height="130" align="left" cellspacing="0" width="170"><tbody><tr><td style="padding-left: 10px; padding-top: 6px; padding-bottom: 6px; background-color: rgb(255, 153, 51); border-bottom: 2px solid rgb(255, 220, 184); font-size: 11pt; font-style: normal; font-weight: bold; text-decoration: none; color: rgb(255, 255, 255); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial Narrow; width: 172px;"><span style="font-family: Arial; font-size: 9pt;">EYE ON PSI CHI</span><br>
                        </td></tr><tr><td style="padding-left: 10px; padding-top: 3px; padding-bottom: 3px; background-color: rgb(255, 255, 255); border-bottom: 2px solid rgb(255, 220, 184); font-size: 10pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial; width: 172px;"><span style="font-weight: bold;"><a href="/?eye_main"><span style="font-family: Arial; font-size: 9pt;"><span style="font-size: 9pt; font-family: Arial;">VIEW THIS ISSUE</span></span></a></span><br>
                        </td></tr><tr><td colspan="1" style="padding-left: 10px; padding-top: 3px; padding-bottom: 3px; background-color: rgb(255, 234, 213); border-bottom: 2px solid rgb(255, 220, 184); font-size: 10pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial; width: 172px;"><span style="font-family: Arial; font-size: 9pt; font-weight: bold; font-style: normal; text-decoration: none; vertical-align: middle; color: rgb(105, 105, 105); background-color: rgb(255, 234, 213); letter-spacing: 0px;"><span style="background-color: rgb(255, 255, 255); font-weight: normal; font-style: normal; text-decoration: none; letter-spacing: 0px;"><span style="font-weight: bold;"></span><span style="background-color: rgb(255, 234, 213);"><a href="/?page=Eye_past" target="_self">PAST ISSUES</a></span></span><br></span></td></tr><tr><td style="padding-left: 10px; padding-top: 3px; padding-bottom: 3px; background-color: rgb(255, 234, 213); border-bottom: 2px solid rgb(255, 220, 184); font-size: 9pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial; width: 172px;">SUBMISSIONS<br>
                        </td></tr><tr><td colspan="1" style="padding-left: 10px; padding-top: 3px; padding-bottom: 3px; background-color: rgb(255, 234, 213); border-bottom: 2px solid rgb(255, 220, 184); font-size: 9pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial; width: 172px;"><span style="font-family: Arial; font-size: 9pt;">» <a href="/?eye_activity" target="_self">CHAPTER ACTIVITY</a><br></span></td></tr><tr><td colspan="1" style="padding-left: 10px; padding-top: 3px; padding-bottom: 3px; background-color: rgb(255, 234, 213); border-bottom: 2px solid rgb(255, 220, 184); font-size: 9pt; font-style: normal; font-weight: normal; text-decoration: none; color: rgb(105, 105, 105); letter-spacing: 0px; word-spacing: 0px; vertical-align: middle; font-family: Arial; width: 172px;"><span style="font-family: Arial; font-size: 9pt;">» </span><a href="/?eye_feature" target="_self">FEATURE ARTICLES</a><br></td></tr></tbody></table><p><span style="font-family: Arial; font-size: 9pt; color: rgb(105, 105, 105);"></span></p><p><img alt="" title="" src="/resource/resmgr/eye_covers/5_2_winter.jpg"><span style="font-family: Arial; font-size: 9pt; color: rgb(105, 105, 105);"><span style="font-family: Arial; font-size: 9pt;"><span style="font-family: Arial; font-size: 9pt; font-style: italic; color: rgb(0, 102, 164);">Eye on Psi Chi</span> is a magazine designed to keep members
and alumni up-to-date with all the latest information about Psi Chi’s programs,
awards, and chapter activities. It features informative articles about careers,
graduate school admission, chapter ideas, personal development, the various
fields of psychology, and important issues related to our discipline.</span><span style="font-family: Arial; font-size: 9pt;">

</span></span></p><p><span style="font-family: Arial; font-size: 9pt; color: rgb(105, 105, 105);"><span style="font-family: Arial; font-size: 9pt; font-style: italic; color: rgb(0, 102, 164);">Eye on Psi Chi</span> is published quarterly:<br><span style="color: rgb(0, 102, 164);">Spring</span> (February)<br><span style="color: rgb(0, 102, 164);">Summer</span> (April)<br><span style="color: rgb(0, 102, 164);">Fall</span>
(September)<br><span style="color: rgb(0, 102, 164);">Winter</span> (November)</span></p><p></p><p><span style="font-family: Arial; font-size: 9pt; color: rgb(105, 105, 105);"><br></span></p><p>&nbsp;</p><p>&nbsp;</p><p>&nbsp;</p><p>&nbsp;</p><p><span style="font-family: Arial; font-size: 9pt; color: rgb(105, 105, 105);">



</span></p></td></tr></tbody></table><span style="color: rgb(105, 105, 105);">

</span></td>

</tr>
</tbody>
</table></div>

	<div id="ResourceCollection">
		
	
	<script type="text/javascript">
	function LaunchThis(sender, strURL)
	{
		window.open (strURL);	
		return false;
	}
	
	function NewCollection(Collection)
	{
		window.location = "/members/resource_collection_item_edit.asp?id=" + Collection + "&groupID=";
		return false;
	}
	
	function ModifyThis(Collection, ItemID)
	{
		window.location = "/members/resource_collection_item_edit.asp?id=" + Collection + "&groupID=&itemID=" + ItemID;
		return false;
	}
	</script>

	</div></td>
</tr>
</table><!--END SpContent-->


<div id="PageBase_RaiseAlert" class="yui-skin-sam"></div>


<div class="yui-skin-sam">
<div id="ContextualHelp" style="visibility:hidden">
	<div id="ContextualHelpHead" class="hd"></div>
	<div id="ContextualHelpBody" class="bd"></div>
</div>
<div id="SpNavBarSub" style="visibility:hidden">
	<div id="SpNavBarSubBody" class="bd"></div>
</div></div>

					<!--@@DG_PRINT_PAGE_END@@
						IMPORTANT! DO NOT MOVE OR MODIFY -->
				</div> <!-- Close left div --></td>
				<div id="right">
				<div id="RightRailTopContentArea"><!--YMPSTITLE=TgBBAA==/YMPSTITLE--><!-- AddThis Button BEGIN --><br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.addthis.com/bookmark.php?v=300&amp;pubid=ra-51b72e6f1fdb42e1" class="addthis_button"><img style="border:0;" alt="Bookmark and Share" src="https://s7.addthis.com/static/btn/v2/lg-share-en.gif" width="125" height="16" /></a>
<script type="text/javascript">var addthis_config = {"data_track_addressbar":true};</script>
<script src="//s7.addthis.com/js/300/addthis_widget.js#pubid=ra-51b72e6f1fdb42e1" type="text/javascript"></script>
<!-- AddThis Button END --></div>
									
					<div id="login" class="zone">
						<div class="irailhead">Sign In</div>
						<div class="irailcontent"><script language="javascript" type="text/javascript" src="/global_inc/js/jquery.data.js"></script><script language="javascript" type="text/javascript" src="/global_inc/js/jquery.watermark.min.js"></script><script type="text/javascript">
                             $(document).ready(function () {
                             $('.loginuser').watermark('Username');
                             $('.loginpass').watermark('Password');});</script><form id='LoginForm' action='https://www.psichi.org/Login.aspx?returl=' method='post'><INPUT TYPE='hidden' NAME='ERR_u' VALUE='u|Username|20|1||0'><INPUT TYPE='hidden' NAME='ERR_p' VALUE='p|Password|20|1||0'><p><div id="LoginUserName"><input class="small loginuser" type="text" name="u" size="20" maxlength="255" value=""/></div><div id="LoginPassword"> <br/>
                        <input class="small loginpass" type="password" name="p" size="20" maxlength="64" autocomplete="off"></div></p>
                        <p id="RememberMe"><input id="FrontendControls_RememberMe"
                            type="checkbox" name="rememberme" value="true" checked><label
                            for="FrontendControls_RememberMe">Remember Me</label></p>
                        <p id="LoginSubmit"><input type="submit" name="btn_submitLogin" value="Sign In" class="formbutton">
							<img class="securesubmit" src="/global_graphics/icons/securesubmit.png" title="Secured with SSL encryption." /></p></form><div id="LoginForgot"><a href='/general/email_pass.asp'>Forgot your password?</a></div><div id="LoginRegister"><a href='/general/register_start.asp'>Apply for Membership!</a></div></div>
					</div>
					
           			<div id="events" class="zone" style="display:;">
                		<div class="irailhead"><a href="/events/event_list.asp">more</a>Calendar</div>
						<div class="irailcontent"><div id="tt-container" class="yui-skin-sam"></div><div class='UpcomingEvents UpcomingEvents_1'><p id="EventPnl359321">1/31/2019<br clear=all><a href='/events/EventDetails.aspx?id=359321'>APS Poster Submission Deadline</a></p></div><div class='UpcomingEvents UpcomingEvents_2'><p id="EventPnl592464">2/1/2019 &raquo; 3/15/2019<br clear=all><a href='/events/EventDetails.aspx?id=592464'>Voting Open for Psi Chi Board of Directors</a></p></div><div class='UpcomingEvents UpcomingEvents_1'><p id="EventPnl762465">2/1/2019<br clear=all><a href='/events/EventDetails.aspx?id=762465'>APS Albert Bandura Graduate Research Award</a></p></div><div class='UpcomingEvents UpcomingEvents_2'><p id="EventPnl889467">2/1/2019<br clear=all><a href='/events/EventDetails.aspx?id=889467'>APS Society Convention Research Awards</a></p></div></div>
					</div>
					
					<div id="news" class="zone" style="display:none;">
						<div class="irailhead"><a href="/news/">more</a>Latest News</div>
						<div class="irailcontent">There are currently no news items posted.</div>
					</div>				
					
					<div id="surveys" class="zone" style="display:none;">
						<div class="irailhead">Online Surveys</div>
						<div class="irailcontent"><table border='0' cellpadding='0' cellspacing='0'></table></div>
					</div>
					
					<div id="featuredmembers" class="zone" style="display:none;">
						<div class="irailhead">Featured Members</div>
						<div class="irailcontent"><p></p></div>
					</div>
					
					
								<div id="railbottom"><!--YMPSTITLE=TgBBAA==/YMPSTITLE--></div>
						</div><!-- end div right -->
						
				<div class="clear"></div>				
		
			</div> <!-- Close sp-content div -->
			<div id="BottomContentArea"><!--YMPSTITLE=TgBBAA==/YMPSTITLE--></div>
			</div> <!-- Close icontent div -->

		    <div id="FooterContentArea">
			    <!--YMPSTITLE=TgBBAA==/YMPSTITLE--><a href="/">PSICHI.ORG</a> | <a href="https://www.psichi.org/?page=PrivacyPolicy">PRIVACY POLICY</a> | <a href="http://psichi.site-ym.com/?page=legal">LEGAL</a> | <a href="http://www.psichi.org/general/?type=contact">CONTACT US</a> | <a href="http://www.psichi.org/?page=JoinToday">JOIN</a> | <a href="https://donate.psichi.org/campaign/give-back-to-psi-chi/c187764" target="_blank">DONATE</a> | <a href="http://www.psichi.org/?page=Advertise">ADVERTISE</a> | <a href="/?page=faq_main">FAQ</a><br />
<br />
&nbsp;© 2017 | PSI CHI, THE INTERNATIONAL HONOR SOCIETY IN PSYCHOLOGY<br />
Phone: (423) 756-2044 | Fax: (423) 265-1529 | <a target="_blank" href="http://www.achsnatl.org/">Certified member of the <span style="font-weight: bold; color: #ffdcb8;">Association of College Honor Societies</span></a><span style="color: #696969;"></span>
		    </div>

		    <div id="Foot"><!-- FOOTER --> </div>

		    <div id="icopyright">Membership Software Powered by <a href='http://www.yourmembership.com/'>YourMembership</a> &nbsp;::&nbsp; <a href='/ams/legal-privacy.htm'>Legal</a><!-- Copyright (c) 1998-2019 YourMembership.com Inc. All Rights Reserved. Copyright: Certain elements of this website are: Copyright (c) 1998-2019, YourMembership.com, Incorporated. YourMembership.com, Incorporated provides a limited license to use its Copyrights to the entity from whose web page you are viewing. Certain elements of this website may also be copyrighted by that entity; please see its Terms of Use or contact the organization for more information. General information about copyright laws can be found at: http://www.copyright.gov/. For more specific information, please consult an attorney. --></div>
</body>


</html>
<!--END_OF_FILE-->
