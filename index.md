<!DOCTYPE html>
<html xmlns = "http://www.w3.org/1999/xhtml" xml:lang = "en" lang = "en">
    <!--
        index.html
        Mockingbird
        Copyright 2009-2018 Some Character LLC. All rights reserved.
    -->
    <head><base href="/version/LYE0YVILUS/" />
        <!-- TypeKit Fonts -->
        <script src="//use.typekit.net/rvq3ubp.js"></script>
        <script>try{Typekit.load();}catch(e){}</script>
        <!-- End TypeKit Fonts -->

  
  
<script type="text/javascript" charset="UTF-8">
(function(_,e,rr,s){_errs=[s];var c=_.onerror;_.onerror=function(){var a=arguments;_errs.push(a);
    c&&c.apply(this,a)};var b=function(){var c=e.createElement(rr),b=e.getElementsByTagName(rr)[0];
    c.src="//beacon.errorception.com/"+s+".js";c.async=!0;b.parentNode.insertBefore(c,b)};
    _.addEventListener?_.addEventListener("load",b,!1):_.attachEvent("onload",b)})
    (window,document,"script","553ebf82a1b3d51609002a6c");
var oldOnError = window.onerror;
window.onerror = function() {
    if(oldOnError)
        oldOnError.apply(this, arguments);
    // FIXME someday
    // layoutSubviews doesn't seem to work past this point,
    // even if manually trying to pump the run loop?
    setTimeout(function() {
        alert("Whoops! Something went wrong. We're looking into it, but in the meantime please refresh your browser.");
        document.location.reload(true);
    }, 1000);
}
</script>

        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=Edge">
        <meta name="apple-mobile-web-app-capable" content="yes">

        <link rel="shortcut icon" href="/static/images/favicon.ico" />

        <title>Mockingbird</title>

        <script type="text/javascript" src="static.js"></script>
        <script type = "text/javascript">
            if(typeof(console) === 'undefined') {
                var console = {}
                console.log = console.error = console.info = console.debug = console.warn = console.trace = console.dir = console.dirxml = console.group = console.groupEnd = console.time = console.timeEnd = console.assert = console.profile = function() {};
            }
        </script>

        <script type="text/javascript">
            OBJJ_INCLUDE_PATHS = ["Frameworks/Release"]
        </script>
            
        <script src="Frameworks/Release/Objective-J/Objective-J.js" type = "text/javascript"></script>

        

        <style type = "text/css">
    html, body, h1, p {
        margin: 0;
        padding: 0;
    }
    /* We need a body wrapper because Cappuccino is unhappy if we change the body element */
    #cappuccino-body {
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        /* Position it absolutely so it will fill the height without content */
        position: absolute;
        top: 0;
        bottom: 0;
        width: 100%;
        /* Put it at the bottom of the stack so it doesn't interfere with UI */
        z-index: 0;
    }
</style>

        <script type="text/javascript">
            (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
            (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
            m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
            })(window,document,'script','//www.google-analytics.com/analytics.js','ga');
            ga('create', 'UA-8797847-1', 'auto');
            if (typeof window.onerror == "object")
            {
                window.onerror = function (err, url, line)
                {
                    ga('send', 'exception', {
                        'exDescription': line + " " + err
                    });
                };
            }
        </script>
    </head>

    <body>
        <div id="cappuccino-body">
            <style type="text/css">
    .fadeOut
    {
        -webkit-animation: fadeout 1s;
           -moz-animation: fadeout 1s;
            -ms-animation: fadeout 1s;
             -o-animation: fadeout 1s;
                animation: fadeout 1s;
    }
    .fadeIn
    {
        -webkit-animation: fadein 1s;
           -moz-animation: fadein 1s;
            -ms-animation: fadein 1s;
             -o-animation: fadein 1s;
                animation: fadein 1s;
    }
    @keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
    @keyframes fadeout { from { opacity: 1; } to { opacity: 0; } }
    @-moz-keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
    @-moz-keyframes fadeout { from { opacity: 1; } to { opacity: 0; } }
    @-webkit-keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
    @-webkit-keyframes fadeout { from { opacity: 1; } to { opacity: 0; } }
    @-ms-keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
    @-ms-keyframes fadein { from { opacity: 1; } to { opacity: 0; } }
    @-o-keyframes fadein { from { opacity: 0; } to { opacity: 1; } }
    @-o-keyframes fadeout { from { opacity: 1; } to { opacity: 0; } }
    #grid-background-container {
        height: 100%;
        background-color: #F5F5F5;
    }
    #horizontal-grid {
        margin: 0;
        -webkit-background-size: 24px 24px;
        -moz-background-size: 24px 24px;
        background-size: 24px 24px;
        height: 100%;
        background-image: linear-gradient(top, transparent 23px, #f5eae6 1px);
        background-image: -webkit-linear-gradient(top, transparent 23px, #f5eae6 1px);
        background-image: -moz-linear-gradient(top, transparent 23px, #f5eae6 1px);
        background-image: -ms-linear-gradient(top, transparent 23px, #f5eae6 1px);
        background-image: -o-linear-gradient(top, transparent 23px, #f5eae6 1px);
    }
    #vertical-grid {
        background-size: 78px;
        width: 916px;
        height: 100%;
        margin: 0 auto;
        position: relative;
        padding-top:168px;
        background-image: linear-gradient(0deg, transparent 58px, #e7e7e7 58px, #e7e7e7 59px, transparent 59px, transparent 77px, #e7e7e7 77px, #e7e7e7 78px);
        background-image: -webkit-linear-gradient(0deg, transparent 58px, #e7e7e7 58px, #e7e7e7 59px, transparent 59px, transparent 77px, #e7e7e7 77px, #e7e7e7 78px);
        background-image: -moz-linear-gradient(0deg, transparent 58px, #e7e7e7 58px, #e7e7e7 59px, transparent 59px, transparent 77px, #e7e7e7 77px, #e7e7e7 78px);
        background-image: -ms-linear-gradient(0deg, transparent 58px, #e7e7e7 58px, #e7e7e7 59px, transparent 59px, transparent 77px, #e7e7e7 77px, #e7e7e7 78px);
        background-image: -o-linear-gradient(0deg, transparent 58px, #e7e7e7 58px, #e7e7e7 59px, transparent 59px, transparent 77px, #e7e7e7 77px, #e7e7e7 78px);
        border-left: 1px solid #d0d0d0;
        border-right: 1px solid #d0d0d0;
        /*vertical grid container */
    }
    #loading-container {
        font-family: "ff-tisa-sans-web-pro";
        margin: auto;
        background-color: white;
        padding: 45px 38px 50px 38px;
        max-width: 507px;
        box-shadow: 0px 2px 6px 0px rgba(0, 0, 0, 0.14);
        border-radius: 4px;
    }
    #loading-container h1 {
        padding: 0px;
        margin: 0;
        font-weight: normal;
        opacity: 0.8;
        font-family: "crete-round";
        font-size: 16px;
        color: #c1c1c1;
        margin-bottom: 16px;
    }
    #loading-container .loading-messages {
        font-family: "ff-tisa-sans-web-pro";
        font-weight: bold;
        font-size: 24px;
        height:40px;
        color: #FD3A40;
    }
    .loading-messages span{
        position: absolute;
        opacity: 0;
        -webkit-transform-origin: 10% 75%;
        transform-origin: 10% 75%;
        -webkit-animation: fadeInAndOut 12s linear infinite 0s;
        -ms-animation: fadeInAndOut 12s linear infinite 0s;
        animation: fadeInAndOut 12s linear infinite 0s;
    }
    .loading-messages span:nth-child(2) {
        -webkit-animation-delay: 3s;
        -ms-animation-delay: 3s;
        animation-delay: 3s;
    }
    .loading-messages span:nth-child(3) {
        -webkit-animation-delay: 6s;
        -ms-animation-delay: 6s;
        animation-delay: 6s;
    }
    .loading-messages span:nth-child(4) {
        -webkit-animation-delay: 9s;
        -ms-animation-delay: 9s;
        animation-delay: 9s;
    }
    @-webkit-keyframes fadeInAndOut {
        0% { opacity: 0; }
        5% { opacity: 0; }
        17% { opacity: 1;}
        19% { opacity: 1;}
        21% { opacity: 1;}
        23% { opacity: 0;}
        25% { opacity: 0;}
        80% { opacity: 0; }
        100% { opacity: 0; }
    }
    @-ms-keyframes fadeInAndOut {
        0% { opacity: 0; }
        5% { opacity: 0; }
        17% { opacity: 1; }
        19% { opacity: 1; }
        21% { opacity: 1; }
        23% { opacity: 0; }
        25% { opacity: 0; }
        80% { opacity: 0; }
        100% { opacity: 0; }
    }
    @keyframes fadeInAndOut {
        0% { opacity: 0; }
        5% { opacity: 0; }
        17% { opacity: 1;}
        19% { opacity: 1;}
        21% { opacity: 1;}
        23% { opacity: 0;}
        25% { opacity: 0;}
        80% { opacity: 0; }
        100% { opacity: 0; }
    }
</style>


            <!-- JAVASCRIPT MISSING -->
            
<noscript>
  <div id="container">
    <div style="width: 440px; padding: 10px 25px 20px 25px; font-family: sans-serif; background-color: #ffffff; position: relative; left: -245px; top: -120px; text-align: center; -moz-border-radius: 20px; -webkit-border-radius: 20px; color: #555555">
      <p style="line-height: 1.4em;">JavaScript is required for this site to work correctly but is either disabled or not supported by your browser.</p>
      <p style="font-size:120%; padding:10px;"><a href="http://cappuccino.org/noscript">Show me how to enable JavaScript</a></p>
      <p style="font-size:80%;">You may want to upgrade to a newer browser while you're at it:</p>
      <ul style="margin:0;padding:0; text-align: center; font-size:80%;" >
        <li style="display: inline;"><a href="http://www.apple.com/safari/download/">Safari</a></li>
        <li style="display: inline;"><a href="http://www.mozilla.com/en-US/firefox/">Firefox</a></li>
        <li style="display: inline;"><a href="http://www.google.com/chrome/">Chrome</a></li>
      </ul>
    </div>
  </div>
</noscript>
        </div>
    </body>
</html>
