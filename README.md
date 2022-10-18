# history
&lt;!DOCTYPE html> &lt;!-- Copyright 2016 Google Inc. All Rights Reserved.  Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at    http://www.apache.org/licenses/LICENSE-2.0  Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License. --> &lt;html> &lt;head> &lt;meta charset="utf-8"> &lt;title>Chrome Platform Status&lt;/title> &lt;meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">  &lt;link rel="manifest" href="/static/manifest.json">  &lt;meta name="theme-color" content="#366597"> &lt;link rel="icon" sizes="192x192" href="/static/img/crstatus_192.png">  &lt;!-- iOS: run in full-screen mode and display upper status bar as translucent --> &lt;meta name="apple-mobile-web-app-capable" content="yes"> &lt;meta name="mobile-web-app-capable" content="yes"> &lt;meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">  &lt;link rel="apple-touch-icon" href="/static/img/crstatus_128.png"> &lt;link rel="apple-touch-icon-precomposed" href="/static/img/crstatus_128.png"> &lt;link rel="shortcut icon" href="/static/img/crstatus_128.png">  &lt;link rel="preconnect" href="https://www.google-analytics.com" crossorigin> &lt;!-- &lt;link rel="dns-prefetch" href="https://fonts.googleapis.com"> --> &lt;!-- &lt;link rel="preconnect" href="https://fonts.gstatic.com" crossorigin> -->    &lt;!-- &lt;link rel="stylesheet"       href="https://fonts.googleapis.com/css?family=Roboto:300,400"       media="none" onload="this.media='all'"> -->  &lt;!-- &lt;link rel="stylesheet" href="/static/css/main.css"> --> &lt;style>html,body{margin:0;padding:0;border:0;font-weight:inherit;font-style:inherit;font-size:100%;font-family:inherit;vertical-align:baseline}div,span,object,iframe,h1,h2,h3,h4,h5,h6,p,pre,a,abbr,acronym,address,code,del,dfn,em,img,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,caption,tbody,tfoot,thead,tr{margin:0;padding:0;border:0;font-weight:inherit;font-style:inherit;font-size:100%;font-family:inherit;vertical-align:baseline}blockquote,q{margin:0;padding:0;border:0;font-weight:inherit;font-style:inherit;font-size:100%;font-family:inherit;vertical-align:baseline;quotes:"" ""}blockquote:before,q:before,blockquote:after,q:after{content:""}th,td,caption{margin:0;padding:0;border:0;font-weight:inherit;font-style:inherit;font-size:100%;font-family:inherit;vertical-align:baseline;text-align:left;font-weight:normal;vertical-align:middle}table{margin:0;padding:0;border:0;font-weight:inherit;font-style:inherit;font-size:100%;font-family:inherit;vertical-align:baseline;border-collapse:separate;border-spacing:0;vertical-align:middle}a img{border:none}*{box-sizing:border-box}*{-webkit-tap-highlight-color:transparent}h1,h2,h3,h4{font-weight:300}h1{font-size:30px}h2,h3,h4{color:#444}h2{font-size:25px}h3{font-size:20px}a{text-decoration:none;color:#4580c0}a:hover{text-decoration:underline;color:#366597}b{font-weight:600}input:not([type="submit"]),textarea{border:1px solid #D4D4D4}input:not([type="submit"])[disabled],textarea[disabled]{opacity:0.5}button,.button{display:inline-block;background:linear-gradient(#F9F9F9 40%, #E3E3E3 70%);border:1px solid #a9a9a9;border-radius:3px;padding:5px 8px;outline:none;white-space:nowrap;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;text-shadow:1px 1px #fff;font-size:10pt}button:not(:disabled):hover{border-color:#515151}button:not(:disabled):active{background:linear-gradient(#E3E3E3 40%, #F9F9F9 70%)}.comma::after{content:',\00a0'}html,body{height:100%}body{color:#666;font:14px "Roboto", sans-serif;font-weight:400;-webkit-font-smoothing:antialiased;background-color:#eee}body.loading #spinner{display:flex}body.loading chromedash-toast{visibility:hidden}#spinner{display:none;align-items:center;justify-content:center;position:fixed;height:calc(100% - 54px - $header-height);max-width:768px;width:100%}#site-banner{display:none;background:#4580c0;color:#fff;position:fixed;z-index:1;-webkit-tap-highlight-color:transparent;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;text-transform:capitalize;text-align:center;transform:rotate(35deg);right:-40px;top:20px;padding:10px 40px 8px 60px;box-shadow:inset 0px 5px 6px -3px rgba(0,0,0,0.4)}#site-banner iron-icon{margin-right:4px;height:20px;width:20px}#site-banner a{color:currentcolor;text-decoration:none}app-drawer{font-size:14px}app-drawer .drawer-content-wrapper{height:100%;overflow:auto;padding:16px}app-drawer paper-listbox{background-color:inherit !important}app-drawer paper-listbox paper-item{font-size:inherit !important}app-drawer h3{margin-bottom:16px;text-transform:uppercase;font-weight:500;font-size:14px;color:inherit}app-header{background-color:#eee;right:0;top:0;left:0;z-index:1}app-header[fixed]{position:fixed}.main-toolbar{display:flex;position:relative;padding:0 16px}header,footer{display:flex;align-items:center;text-shadow:0 1px 0 white}header{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}header a{text-decoration:none !important}header nav{display:flex;align-items:center;margin-left:16px}header nav a{background-color:#FAFAFA;background:linear-gradient(to bottom, white, #F2F2F2);padding:0.75em 1em;box-shadow:1px 1px 4px rgba(0,0,0,0.065);cursor:pointer;font-size:16px;text-align:center;border-radius:3px;border-bottom:1px solid #D4D4D4;border-right:1px solid #D4D4D4;white-space:nowrap}header nav a:active{position:relative;top:1px;left:1px;box-shadow:3px 3px 4px rgba(0,0,0,0.065)}header nav a.disabled{opacity:0.5;pointer-events:none}header nav paper-menu-button{margin:0 !important;padding:0 !important;line-height:1}header nav paper-menu-button .dropdown-content{display:flex;flex-direction:column;contain:content}header aside{background-color:#FAFAFA;background:linear-gradient(to bottom, white, #F2F2F2);padding:0.75em 1em;box-shadow:1px 1px 4px rgba(0,0,0,0.065);border-bottom-left-radius:5px;border-bottom-right-radius:5px;border-bottom:1px solid #D4D4D4;border-right:1px solid #D4D4D4;background:url(/static/img/chrome_logo.svg) no-repeat 16px 50%;background-size:48px;background-color:#fafafa;padding-left:72px}header aside hgroup a{color:currentcolor}header aside h1{line-height:1}header aside img{height:45px;width:45px;margin-right:7px}footer{background-color:#FAFAFA;background:linear-gradient(to bottom, white, #F2F2F2);padding:0.75em 1em;box-shadow:1px 1px 4px rgba(0,0,0,0.065);font-size:12px;box-shadow:0 -2px 5px rgba(0,0,0,0.065);display:flex;flex-direction:column;justify-content:center;text-align:center;position:fixed;bottom:0;left:0;right:0;z-index:3}footer div{margin-top:4px}.description{line-height:1.4}#subheader,.subheader{display:flex;align-items:center;margin:16px 0;max-width:768px}#subheader .num-features,.subheader .num-features{font-weight:400}#subheader div.search input,.subheader div.search input{width:200px;outline:none;padding:10px 7px}#subheader div.actionlinks,.subheader div.actionlinks{display:flex;justify-content:flex-end;flex:1 0 auto;margin-left:16px}#subheader div.actionlinks .blue-button,.subheader div.actionlinks .blue-button{background:#366597;color:#fff;display:inline-flex;align-items:center;justify-content:center;max-height:35px;min-width:5.14em;-webkit-tap-highlight-color:transparent;-webkit-tap-highlight-color:transparent;text-transform:uppercase;text-decoration:none;border-radius:3px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;padding:0.7em 0.57em}#subheader div.actionlinks .blue-button iron-icon,.subheader div.actionlinks .blue-button iron-icon{margin-right:8px;height:24px;width:24px}#subheader div.actionlinks .legend,.subheader div.actionlinks .legend{font-size:18px;cursor:pointer;text-decoration:none}#container{display:flex;flex-direction:column;height:100%;width:100%}#content{margin:16px;position:relative;height:100%}#panels{display:flex;width:100%;overflow:hidden}@media only screen and (min-width: 701px){.main-toolbar .toolbar-content{max-width:768px}app-header{padding-left:200px;left:0 !important}}@media only screen and (max-width: 700px){h1{font-size:24px}h2{font-size:20px}h3{font-size:15px}app-header .main-toolbar{padding:0;display:block}app-header .main-toolbar iron-icon{width:24px}app-drawer{z-index:2}#content{margin-left:0;margin-right:0}header{margin:0;display:block}header aside{display:flex;padding:8px;border-radius:0;background-size:24px;background-position:48px 50%}header aside hgroup{padding-left:48px}header aside hgroup span{display:none}header nav{margin:0;justify-content:center;flex-wrap:wrap}header nav a{padding:5px 10px;margin:0;border-radius:0;flex:1 0 auto}#panels{display:block}#panels nav{display:none}.subheader .description{margin:0 16px}#subheader div:not(.search){display:none}#subheader div.search{text-align:center;flex:1 0 0;margin:0}chromedash-toast{width:100%;left:0;margin:0}}@media only screen and (min-width: 1100px){#site-banner{display:block}}body.loading chromedash-legend{display:none}body.loading chromedash-featurelist{visibility:hidden}body.loading .main-toolbar .dropdown-content{display:none} &lt;/style>   &lt;!-- &lt;link rel="stylesheet" href="/static/css/metrics/metrics.css"> --> &lt;style>#content h3{margin-bottom:16px}.data-panel{max-width:768px}.data-panel .description{margin-bottom:1em}.metric-nav{list-style-type:none}.metric-nav h3:not(:first-of-type){margin-top:32px}.metric-nav li{text-align:center;border-top-left-radius:3px;border-top-right-radius:3px;background:linear-gradient(to bottom, white, #F2F2F2);box-shadow:1px 1px 4px rgba(0,0,0,0.065);padding:0.5em;margin-bottom:10px}@media only screen and (max-width: 700px){#subheader{margin:16px 0;text-align:center}.data-panel{margin:0 10px}} &lt;/style>     &lt;script> window.Polymer = window.Polymer || {   dom: 'shadow', // Use native shadow dom.   lazyRegister: 'max',   useNativeCSSProperties: true,   suppressTemplateNotifications: true, // Don't fire dom-change on dom-if, dom-bind, etc.   suppressBindingNotifications: true   // disableUpgradeEnabled: true // Works with `disable-upgrade` attr. When removed, upgrades element. };  var $ = function(selector) {   return document.querySelector(selector); };  var $$ = function(selector) {   return document.querySelectorAll(selector); }; &lt;/script>  &lt;style is="custom-style">   app-drawer {     --app-drawer-width: 200px;     --app-drawer-content-container: {       background: #eee;     };   }   paper-item {     --paper-item: {       cursor: pointer;     };   } &lt;/style>     &lt;link rel="import" href="/static/elements/metrics-imports.vulcanize.html">    &lt;/head> &lt;body class="loading">  &lt;!--&lt;div id="site-banner">   &lt;a href="https://www.youtube.com/watch?v=Rd0plknSPYU" target="_blank">   &lt;iron-icon icon="chromestatus:ondemand-video">&lt;/iron-icon> How we built it&lt;/a> &lt;/div>-->  &lt;app-drawer-layout fullbleed>   &lt;app-drawer swipe-open>     &lt;div class="drawer-content-wrapper">          &lt;ul class="metric-nav">   &lt;h3>All properties&lt;/h3>   &lt;li>&lt;a href="/metrics/css/popularity">Stack rank&lt;/a>&lt;/li>   &lt;li>&lt;a href="/metrics/css/timeline/popularity">Timeline&lt;/a>&lt;/li>   &lt;h3>Animated properties&lt;/h3>   &lt;li>&lt;a href="/metrics/css/animated">Stack rank&lt;/a>&lt;/li>   &lt;li>&lt;a href="/metrics/css/timeline/animated">Timeline&lt;/a>&lt;/li> &lt;/ul>       &lt;/div>   &lt;/app-drawer>   &lt;app-header-layout>     &lt;app-header reveals fixed effects="waterfall">       &lt;div class="main-toolbar">         &lt;div class="toolbar-content">           &lt;header>   &lt;aside>     &lt;iron-icon icon="chromestatus:menu" drawer-toggle>&lt;/iron-icon>     &lt;hgroup>       &lt;a href="/features" target="_top">&lt;h1>Chrome Platform Status&lt;/h1>&lt;/a>       &lt;span>feature support &amp;amp; usage metrics&lt;/span>     &lt;/hgroup>   &lt;/aside>   &lt;nav>     &lt;a href="/features">Features&lt;/a>     &lt;a href="/samples" class="features">Samples&lt;/a>     &lt;paper-menu-button vertical-align="top" horizontal-align="right">       &lt;a href="javascript:void(0)" class="dropdown-trigger">Usage Metrics&lt;/a>       &lt;div class="dropdown-content" hidden> &lt;!-- hidden removed by lazy load code. -->         &lt;a href="/metrics/css/popularity" class="metrics">CSS&lt;/a>         &lt;a href="/metrics/feature/popularity" class="metrics">JS/HTML&lt;/a>       &lt;/div>     &lt;/paper-menu-button>   &lt;/nav> &lt;/header>             &lt;div id="subheader">   &lt;h2>CSS usage metrics &amp;gt; animated properties > timeline&lt;/h2> &lt;/div>          &lt;/div>       &lt;/div>     &lt;/app-header>      &lt;div id="content">       &lt;div id="spinner">&lt;img src="/static/img/ring.svg">&lt;/div>        &lt;div class="data-panel">   &lt;p class="description">Percentages are the number of times (as the fraction of all animated properties) this property is animated.&lt;/p>   &lt;chromedash-feature-timeline       type="css" view="animated"       title="Percentage of times (as the fraction of all animated properties) this property is animated."       >&lt;/chromedash-feature-timeline> &lt;/div>      &lt;/div>    &lt;/app-header-layout>    &lt;footer>   &lt;p>Except as otherwise noted, the content of this page under &lt;a href="https://creativecommons.org/licenses/by/2.5/">CC Attribution 2.5&lt;/a> license. Code examples are &lt;a href="https://github.com/GoogleChrome/samples/blob/gh-pages/LICENSE">Apache-2.0&lt;/a>.&lt;/p>   &lt;div>&lt;a href="https://groups.google.com/a/chromium.org/forum/#!newtopic/blink-dev">File content issue&lt;/a> | &lt;a href="https://docs.google.com/a/chromium.org/forms/d/1djZD0COt4NgRwDYesNLkYAb_O8YL39eEvF78vk06R9c/viewform">Request "edit" access&lt;/a> | &lt;a href="https://github.com/GoogleChrome/chromium-dashboard/issues">File site bug&lt;/a> | &lt;a href="https://docs.google.com/document/d/1jrSlM4Yhae7XCJ8BuasWx71CvDEMMbSKbXwx7hoh1Co/edit?pli=1" target="_blank">About&lt;/a> |       &lt;a href="https://www.google.com/accounts/ServiceLogin?service=ah&amp;amp;passive=true&amp;amp;continue=https://appengine.google.com/_ah/conflogin%3Fcontinue%3Dhttps://www.chromestatus.com/metrics/css/timeline/animated">Login&lt;/a>   &lt;/div> &lt;/footer>  &lt;/app-drawer-layout>  &lt;chromedash-toast msg="Welcome to chromestatus.com!">&lt;/chromedash-toast>     &lt;script> /*! (c) 2017 Copyright (c) 2016 The Google Inc. All rights reserved. (Apache2) */ "use strict";function _classCallCheck(e,r){if(!(e instanceof r))throw new TypeError("Cannot call a class as a function")}var _createClass=function(){function e(e,r){for(var n=0;n&lt;r.length;n++){var t=r[n];t.enumerable=t.enumerable||!1,t.configurable=!0,"value"in t&amp;&amp;(t.writable=!0),Object.defineProperty(e,t.key,t)}}return function(r,n,t){return n&amp;&amp;e(r.prototype,n),t&amp;&amp;e(r,t),r}}(),Metric=function(){function e(r){if(_classCallCheck(this,e),!r)throw Error("Please provide a metric name");if(!e.supportsPerfMark&amp;&amp;(console.warn("Timeline won't be marked for \""+r+'".'),!e.supportsPerfNow))throw Error("This library cannot be used in this browser.");this.name=r}return _createClass(e,[{key:"duration",get:function(){var r=this._end-this._start;if(e.supportsPerfMark){var n=performance.getEntriesByName(this.name)[0];n&amp;&amp;"measure"!==n.entryType&amp;&amp;(r=n.duration)}return r||-1}}],[{key:"supportsPerfNow",get:function(){return performance&amp;&amp;performance.now}},{key:"supportsPerfMark",get:function(){return performance&amp;&amp;performance.mark}}]),_createClass(e,[{key:"log",value:function(){return console.info(this.name,this.duration,"ms"),this}},{key:"logAll",value:function(){var r=arguments.length>0&amp;&amp;void 0!==arguments[0]?arguments[0]:this.name;if(e.supportsPerfNow)for(var n=window.performance.getEntriesByName(r),t=0;t&lt;n.length;++t){var a=n[t];console.info(r,a.duration,"ms")}return this}},{key:"start",value:function(){return this._start?(console.warn("Recording already started."),this):(this._start=performance.now(),e.supportsPerfMark&amp;&amp;performance.mark("mark_"+this.name+"_start"),this)}},{key:"end",value:function(){if(this._end)return console.warn("Recording already stopped."),this;if(this._end=performance.now(),e.supportsPerfMark){var r="mark_"+this.name+"_start",n="mark_"+this.name+"_end";performance.mark(n),performance.measure(this.name,r,n)}return this}},{key:"sendToAnalytics",value:function(e){var r=arguments.length>1&amp;&amp;void 0!==arguments[1]?arguments[1]:this.name,n=arguments.length>2&amp;&amp;void 0!==arguments[2]?arguments[2]:this.duration;return window.ga?n>=0&amp;&amp;ga("send","timing",e,r,n):console.warn("Google Analytics has not been loaded"),this}}]),e}(); &lt;/script>   &lt;script> document.addEventListener('WebComponentsReady', function(e) {   var timeline = $('chromedash-feature-timeline');   timeline.props = [[469,"alias-epub-caption-side"],[470,"alias-epub-text-combine"],[471,"alias-epub-text-emphasis"],[472,"alias-epub-text-emphasis-color"],[473,"alias-epub-text-emphasis-style"],[474,"alias-epub-text-orientation"],[475,"alias-epub-text-transform"],[476,"alias-epub-word-break"],[477,"alias-epub-writing-mode"],[478,"alias-webkit-align-content"],[479,"alias-webkit-align-items"],[480,"alias-webkit-align-self"],[166,"alias-webkit-animation"],[167,"alias-webkit-animation-delay"],[169,"alias-webkit-animation-duration"],[170,"alias-webkit-animation-fill-mode"],[171,"alias-webkit-animation-iteration-count"],[172,"alias-webkit-animation-name"],[173,"alias-webkit-animation-play-state"],[174,"alias-webkit-animation-timing-function"],[177,"alias-webkit-backface-visibility"],[181,"alias-webkit-background-size"],[481,"alias-webkit-border-bottom-left-radius"],[482,"alias-webkit-border-bottom-right-radius"],[197,"alias-webkit-border-radius"],[483,"alias-webkit-border-top-left-radius"],[484,"alias-webkit-border-top-right-radius"],[212,"alias-webkit-box-shadow"],[485,"alias-webkit-box-sizing"],[218,"alias-webkit-column-count"],[219,"alias-webkit-column-gap"],[221,"alias-webkit-column-rule"],[222,"alias-webkit-column-rule-color"],[223,"alias-webkit-column-rule-style"],[224,"alias-webkit-column-rule-width"],[225,"alias-webkit-column-span"],[226,"alias-webkit-column-width"],[227,"alias-webkit-columns"],[486,"alias-webkit-flex"],[487,"alias-webkit-flex-basis"],[488,"alias-webkit-flex-direction"],[489,"alias-webkit-flex-flow"],[490,"alias-webkit-flex-grow"],[491,"alias-webkit-flex-shrink"],[492,"alias-webkit-flex-wrap"],[493,"alias-webkit-justify-content"],[494,"alias-webkit-opacity"],[495,"alias-webkit-order"],[308,"alias-webkit-perspective"],[309,"alias-webkit-perspective-origin"],[496,"alias-webkit-shape-image-threshold"],[497,"alias-webkit-shape-margin"],[498,"alias-webkit-shape-outside"],[537,"alias-webkit-text-size-adjust"],[326,"alias-webkit-transform"],[327,"alias-webkit-transform-origin"],[331,"alias-webkit-transform-style"],[332,"alias-webkit-transition"],[333,"alias-webkit-transition-delay"],[334,"alias-webkit-transition-duration"],[335,"alias-webkit-transition-property"],[336,"alias-webkit-transition-timing-function"],[230,"align-content"],[231,"align-items"],[232,"align-self"],[386,"alignment-baseline"],[454,"all"],[424,"animation"],[425,"animation-delay"],[426,"animation-direction"],[427,"animation-duration"],[428,"animation-fill-mode"],[429,"animation-iteration-count"],[430,"animation-name"],[431,"animation-play-state"],[432,"animation-timing-function"],[532,"apply-at-rule"],[508,"backdrop-filter"],[451,"backface-visibility"],[21,"background"],[22,"background-attachment"],[419,"background-blend-mode"],[23,"background-clip"],[24,"background-color"],[25,"background-image"],[26,"background-origin"],[27,"background-position"],[28,"background-position-x"],[29,"background-position-y"],[30,"background-repeat"],[31,"background-repeat-x"],[32,"background-repeat-y"],[33,"background-size"],[387,"baseline-shift"],[551,"block-size"],[34,"border"],[35,"border-bottom"],[36,"border-bottom-color"],[37,"border-bottom-left-radius"],[38,"border-bottom-right-radius"],[39,"border-bottom-style"],[40,"border-bottom-width"],[41,"border-collapse"],[42,"border-color"],[43,"border-image"],[44,"border-image-outset"],[45,"border-image-repeat"],[46,"border-image-slice"],[47,"border-image-source"],[48,"border-image-width"],[49,"border-left"],[50,"border-left-color"],[51,"border-left-style"],[52,"border-left-width"],[53,"border-radius"],[54,"border-right"],[55,"border-right-color"],[56,"border-right-style"],[57,"border-right-width"],[58,"border-spacing"],[59,"border-style"],[60,"border-top"],[61,"border-top-color"],[62,"border-top-left-radius"],[63,"border-top-right-radius"],[64,"border-top-style"],[65,"border-top-width"],[66,"border-width"],[67,"bottom"],[68,"box-shadow"],[69,"box-sizing"],[520,"break-after"],[521,"break-before"],[522,"break-inside"],[416,"buffered-rendering"],[70,"caption-side"],[547,"caret-color"],[71,"clear"],[72,"clip"],[355,"clip-path"],[356,"clip-rule"],[2,"color"],[365,"color-interpolation"],[366,"color-interpolation-filters"],[367,"color-profile"],[368,"color-rendering"],[523,"column-count"],[440,"column-fill"],[524,"column-gap"],[525,"column-rule"],[526,"column-rule-color"],[527,"column-rule-style"],[528,"column-rule-width"],[529,"column-span"],[530,"column-width"],[531,"columns"],[517,"contain"],[74,"content"],[75,"counter-increment"],[76,"counter-reset"],[77,"cursor"],[466,"cx"],[467,"cy"],[518,"d"],[3,"direction"],[4,"display"],[388,"dominant-baseline"],[78,"empty-cells"],[358,"enable-background"],[369,"fill"],[370,"fill-opacity"],[371,"fill-rule"],[359,"filter"],[233,"flex"],[234,"flex-basis"],[235,"flex-direction"],[236,"flex-flow"],[237,"flex-grow"],[238,"flex-shrink"],[239,"flex-wrap"],[79,"float"],[360,"flood-color"],[361,"flood-opacity"],[5,"font"],[516,"font-display"],[6,"font-family"],[514,"font-feature-settings"],[13,"font-kerning"],[7,"font-size"],[465,"font-size-adjust"],[80,"font-stretch"],[8,"font-style"],[9,"font-variant"],[533,"font-variant-caps"],[15,"font-variant-ligatures"],[535,"font-variant-numeric"],[549,"font-variation-settings"],[10,"font-weight"],[389,"glyph-orientation-horizontal"],[390,"glyph-orientation-vertical"],[453,"grid"],[422,"grid-area"],[418,"grid-auto-columns"],[250,"grid-auto-flow"],[417,"grid-auto-rows"],[248,"grid-column"],[245,"grid-column-end"],[511,"grid-column-gap"],[244,"grid-column-start"],[513,"grid-gap"],[249,"grid-row"],[247,"grid-row-end"],[512,"grid-row-gap"],[246,"grid-row-start"],[452,"grid-template"],[423,"grid-template-areas"],[242,"grid-template-columns"],[243,"grid-template-rows"],[81,"height"],[534,"hyphens"],[397,"image-orientation"],[507,"image-orientation"],[82,"image-rendering"],[398,"image-resolution"],[550,"inline-size"],[438,"internal-callback"],[436,"isolation"],[240,"justify-content"],[455,"justify-items"],[443,"justify-self"],[391,"kerning"],[83,"left"],[84,"letter-spacing"],[362,"lighting-color"],[556,"line-break"],[20,"line-height"],[85,"list-style"],[86,"list-style-image"],[87,"list-style-position"],[88,"list-style-type"],[89,"margin"],[90,"margin-bottom"],[91,"margin-left"],[92,"margin-right"],[93,"margin-top"],[372,"marker"],[373,"marker-end"],[374,"marker-mid"],[375,"marker-start"],[357,"mask"],[435,"mask-source-type"],[376,"mask-type"],[555,"max-block-size"],[94,"max-height"],[554,"max-inline-size"],[95,"max-width"],[406,"max-zoom"],[553,"min-block-size"],[96,"min-height"],[552,"min-inline-size"],[97,"min-width"],[407,"min-zoom"],[420,"mix-blend-mode"],[460,"motion"],[458,"motion-offset"],[457,"motion-path"],[459,"motion-rotation"],[433,"object-fit"],[437,"object-position"],[543,"offset"],[544,"offset-anchor"],[540,"offset-distance"],[541,"offset-path"],[545,"offset-position"],[548,"offset-rotate"],[542,"offset-rotation"],[98,"opacity"],[303,"order"],[408,"orientation"],[99,"orphans"],[100,"outline"],[101,"outline-color"],[102,"outline-offset"],[103,"outline-style"],[104,"outline-width"],[105,"overflow"],[538,"overflow-anchor"],[106,"overflow-wrap"],[107,"overflow-x"],[108,"overflow-y"],[109,"padding"],[110,"padding-bottom"],[111,"padding-left"],[112,"padding-right"],[113,"padding-top"],[114,"page"],[115,"page-break-after"],[116,"page-break-before"],[117,"page-break-inside"],[434,"paint-order"],[449,"perspective"],[450,"perspective-origin"],[557,"place-content"],[558,"place-items"],[118,"pointer-events"],[119,"position"],[120,"quotes"],[468,"r"],[121,"resize"],[122,"right"],[505,"rotate"],[463,"rx"],[464,"ry"],[506,"scale"],[444,"scroll-behavior"],[456,"scroll-blocks-on"],[502,"scroll-snap-coordinate"],[503,"scroll-snap-destination"],[500,"scroll-snap-points-x"],[501,"scroll-snap-points-y"],[499,"scroll-snap-type"],[439,"shape-image-threshold"],[346,"shape-inside"],[348,"shape-margin"],[347,"shape-outside"],[349,"shape-padding"],[377,"shape-rendering"],[123,"size"],[519,"snap-height"],[125,"speak"],[124,"src"],[363,"stop-color"],[364,"stop-opacity"],[378,"stroke"],[379,"stroke-dasharray"],[380,"stroke-dashoffset"],[381,"stroke-linecap"],[382,"stroke-linejoin"],[383,"stroke-miterlimit"],[384,"stroke-opacity"],[385,"stroke-width"],[127,"tab-size"],[126,"table-layout"],[128,"text-align"],[404,"text-align-last"],[392,"text-anchor"],[509,"text-combine-upright"],[129,"text-decoration"],[403,"text-decoration-color"],[401,"text-decoration-line"],[546,"text-decoration-skip"],[402,"text-decoration-style"],[130,"text-indent"],[441,"text-justify"],[131,"text-line-through"],[132,"text-line-through-color"],[133,"text-line-through-mode"],[134,"text-line-through-style"],[135,"text-line-through-width"],[510,"text-orientation"],[136,"text-overflow"],[137,"text-overline"],[138,"text-overline-color"],[139,"text-overline-mode"],[140,"text-overline-style"],[141,"text-overline-width"],[11,"text-rendering"],[142,"text-shadow"],[536,"text-size-adjust"],[143,"text-transform"],[144,"text-underline"],[145,"text-underline-color"],[146,"text-underline-mode"],[405,"text-underline-position"],[147,"text-underline-style"],[148,"text-underline-width"],[149,"top"],[421,"touch-action"],[442,"touch-action-delay"],[446,"transform"],[559,"transform-box"],[447,"transform-origin"],[448,"transform-style"],[150,"transition"],[151,"transition-delay"],[152,"transition-duration"],[153,"transition-property"],[154,"transition-timing-function"],[504,"translate"],[155,"unicode-bidi"],[156,"unicode-range"],[539,"user-select"],[409,"user-zoom"],[515,"variable"],[393,"vector-effect"],[157,"vertical-align"],[158,"visibility"],[168,"webkit-animation-direction"],[354,"webkit-app-region"],[412,"webkit-app-region"],[175,"webkit-appearance"],[176,"webkit-aspect-ratio"],[400,"webkit-background-blend-mode"],[178,"webkit-background-clip"],[179,"webkit-background-composite"],[180,"webkit-background-origin"],[399,"webkit-blend-mode"],[182,"webkit-border-after"],[183,"webkit-border-after-color"],[184,"webkit-border-after-style"],[185,"webkit-border-after-width"],[186,"webkit-border-before"],[187,"webkit-border-before-color"],[188,"webkit-border-before-style"],[189,"webkit-border-before-width"],[190,"webkit-border-end"],[191,"webkit-border-end-color"],[192,"webkit-border-end-style"],[193,"webkit-border-end-width"],[194,"webkit-border-fit"],[195,"webkit-border-horizontal-spacing"],[196,"webkit-border-image"],[198,"webkit-border-start"],[199,"webkit-border-start-color"],[200,"webkit-border-start-style"],[201,"webkit-border-start-width"],[202,"webkit-border-vertical-spacing"],[203,"webkit-box-align"],[228,"webkit-box-decoration-break"],[414,"webkit-box-decoration-break"],[204,"webkit-box-direction"],[205,"webkit-box-flex"],[206,"webkit-box-flex-group"],[207,"webkit-box-lines"],[208,"webkit-box-ordinal-group"],[209,"webkit-box-orient"],[210,"webkit-box-pack"],[211,"webkit-box-reflect"],[73,"webkit-clip-path"],[213,"webkit-color-correction"],[214,"webkit-column-axis"],[215,"webkit-column-break-after"],[216,"webkit-column-break-before"],[217,"webkit-column-break-inside"],[220,"webkit-column-progression"],[396,"webkit-cursor-visibility"],[410,"webkit-dashboard-region"],[229,"webkit-filter"],[413,"webkit-filter"],[341,"webkit-flow-from"],[340,"webkit-flow-into"],[12,"webkit-font-feature-settings"],[241,"webkit-font-size-delta"],[14,"webkit-font-smoothing"],[251,"webkit-highlight"],[252,"webkit-hyphenate-character"],[253,"webkit-hyphenate-limit-after"],[254,"webkit-hyphenate-limit-before"],[255,"webkit-hyphenate-limit-lines"],[256,"webkit-hyphens"],[258,"webkit-line-align"],[257,"webkit-line-box-contain"],[259,"webkit-line-break"],[260,"webkit-line-clamp"],[261,"webkit-line-grid"],[262,"webkit-line-snap"],[16,"webkit-locale"],[264,"webkit-logical-height"],[263,"webkit-logical-width"],[270,"webkit-margin-after"],[265,"webkit-margin-after-collapse"],[271,"webkit-margin-before"],[266,"webkit-margin-before-collapse"],[267,"webkit-margin-bottom-collapse"],[269,"webkit-margin-collapse"],[272,"webkit-margin-end"],[273,"webkit-margin-start"],[268,"webkit-margin-top-collapse"],[274,"webkit-marquee"],[275,"webkit-marquee-direction"],[276,"webkit-marquee-increment"],[277,"webkit-marquee-repetition"],[278,"webkit-marquee-speed"],[279,"webkit-marquee-style"],[280,"webkit-mask"],[281,"webkit-mask-box-image"],[282,"webkit-mask-box-image-outset"],[283,"webkit-mask-box-image-repeat"],[284,"webkit-mask-box-image-slice"],[285,"webkit-mask-box-image-source"],[286,"webkit-mask-box-image-width"],[287,"webkit-mask-clip"],[288,"webkit-mask-composite"],[289,"webkit-mask-image"],[290,"webkit-mask-origin"],[291,"webkit-mask-position"],[292,"webkit-mask-position-x"],[293,"webkit-mask-position-y"],[294,"webkit-mask-repeat"],[295,"webkit-mask-repeat-x"],[296,"webkit-mask-repeat-y"],[297,"webkit-mask-size"],[299,"webkit-max-logical-height"],[298,"webkit-max-logical-width"],[301,"webkit-min-logical-height"],[300,"webkit-min-logical-width"],[302,"webkit-nbsp-mode"],[411,"webkit-overflow-scrolling"],[304,"webkit-padding-after"],[305,"webkit-padding-before"],[306,"webkit-padding-end"],[307,"webkit-padding-start"],[310,"webkit-perspective-origin-x"],[311,"webkit-perspective-origin-y"],[312,"webkit-print-color-adjust"],[343,"webkit-region-break-after"],[344,"webkit-region-break-before"],[345,"webkit-region-break-inside"],[342,"webkit-region-fragment"],[313,"webkit-rtl-ordering"],[314,"webkit-ruby-position"],[395,"webkit-svg-shadow"],[353,"webkit-tap-highlight-color"],[415,"webkit-tap-highlight-color"],[315,"webkit-text-combine"],[316,"webkit-text-decorations-in-effect"],[317,"webkit-text-emphasis"],[318,"webkit-text-emphasis-color"],[319,"webkit-text-emphasis-position"],[320,"webkit-text-emphasis-style"],[321,"webkit-text-fill-color"],[17,"webkit-text-orientation"],[322,"webkit-text-security"],[323,"webkit-text-stroke"],[324,"webkit-text-stroke-color"],[325,"webkit-text-stroke-width"],[328,"webkit-transform-origin-x"],[329,"webkit-transform-origin-y"],[330,"webkit-transform-origin-z"],[337,"webkit-user-drag"],[338,"webkit-user-modify"],[339,"webkit-user-select"],[352,"webkit-wrap"],[350,"webkit-wrap-flow"],[351,"webkit-wrap-through"],[18,"webkit-writing-mode"],[159,"white-space"],[160,"widows"],[161,"width"],[445,"will-change"],[162,"word-break"],[163,"word-spacing"],[164,"word-wrap"],[394,"writing-mode"],[461,"x"],[462,"y"],[165,"z-index"],[19,"zoom"]];    document.body.classList.remove('loading');    window.addEventListener('popstate', function(e) {     if (e.state) {       timeline.selectedBucketId = e.state.id;     }   }); }); &lt;/script>   &lt;script> /*! (c) 2017 Copyright (c) 2016 The Google Inc. All rights reserved. (Apache2) */ "use strict";!function(e){function r(){return caches.keys().then(function(e){var r=0;return Promise.all(e.map(function(e){if(e.includes("sw-precache"))return caches.open(e).then(function(e){return e.keys().then(function(n){return Promise.all(n.map(function(n){return e.match(n).then(function(e){return e.arrayBuffer()}).then(function(e){r+=e.byteLength})}))})})})).then(function(){return r})["catch"](function(){})})}function n(){"serviceWorker"in navigator&amp;&amp;navigator.serviceWorker.register("/service-worker.js").then(function(e){e.onupdatefound=function(){var n=e.installing;n.onstatechange=function(){switch(n.state){case"installed":t&amp;&amp;!navigator.serviceWorker.controller&amp;&amp;o.then(r().then(function(e){var r=Math.round(e/1e3);console.info("[ServiceWorker] precached",r,"KB");var n=new Metric("sw_precache");n.sendToAnalytics("service worker","precache size",e),t.showMessage("This site is cached ("+r+"KB). Ready to use offline!")}));break;case"redundant":throw Error("The installing service worker became redundant.")}}}})["catch"](function(e){console.error("Error during service worker registration:",e)})}var t=document.querySelector("chromedash-toast"),o=new Promise(function(e,r){return window.asyncImportsLoadPromise?window.asyncImportsLoadPromise.then(e,r):void e()});window.asyncImportsLoadPromise||n(),navigator.serviceWorker&amp;&amp;navigator.serviceWorker.controller&amp;&amp;(navigator.serviceWorker.controller.onstatechange=function(e){if("redundant"===e.target.state){var r=function(){window.location.reload()};t?o.then(function(){t.showMessage("A new version of this app is available.","Refresh",r,-1)}):r()}}),e.registerServiceWorker=n}(window);  // https://gist.github.com/ebidel/1d5ede1e35b6f426a2a7 function lazyLoadWCPolyfillsIfNecessary() {   function onload() {     // For native Imports, manually fire WCR so user code     // can use the same code path for native and polyfill'd imports.     if (!('HTMLImports' in window)) {       document.body.dispatchEvent(           new CustomEvent('WebComponentsReady', {bubbles: true}));     }   }    var webComponentsSupported = ('registerElement' in document       &amp;&amp; 'import' in document.createElement('link')       &amp;&amp; 'content' in document.createElement('template'));   if (!webComponentsSupported) {     var script = document.createElement('script');     script.async = true;     script.src = '/static/bower_components/webcomponentsjs/webcomponents-lite.min.js';     script.onload = onload;     document.head.appendChild(script);   } else {     onload();   } }  var button = document.querySelector('app-header paper-menu-button'); button.addEventListener('click', function lazyHandler(e) {   this.removeEventListener('click', lazyHandler);       var url = '/static/elements/paper-menu-button.vulcanize.html';       Polymer.Base.importHref(url, function() {     button.contentElement.hidden = false;     button.open();   }, null, true); });  // Google Analytics (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){ (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o), m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m) })(window,document,'script','//www.google-analytics.com/analytics.js','ga');  ga('create', 'UA-39048143-1', 'auto'); ga('send', 'pageview'); // End Google Analytics  lazyLoadWCPolyfillsIfNecessary(); &lt;/script> &lt;/body> &lt;/html>
