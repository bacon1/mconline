<html lang="en" class="no-js">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">

        <title>Minecraft</title>
        <meta name="description" content="Minecraft is a game about placing blocks to build anything you can imagine. At night monsters come out, make sure to build a shelter before that happens.">
        <meta name="author" content="Mojang AB">

        <meta name="viewport" content="width=device-width, initial-scale=1.0">

        <link rel="shortcut icon" href="/favicon.png">
        <link rel="apple-touch-icon" href="/apple-touch-icon.png">
        <link rel="stylesheet" href="/stylesheets/style.css?b=b_672">
        <link rel="stylesheet" media="handheld" href="/stylesheets/handheld.css?b=b_672">
                <!--[if !IE 7]>
        <style type="text/css">
        #wrap {display:table;height:100%}
        </style>
        <![endif]-->
        <script src="/javascripts/libs/modernizr.min.js"></script>
        <script>
            function recordOutboundLink(link, category, action, label, value) {
                try {
                    _gaq.push(['_trackEvent', category, action, label, value]);
                    setTimeout('document.location = "' + link.href + '"', 100);
                }catch(err){}
            }
            
            var _gaq = _gaq || [];
            _gaq.push(['_setAccount', 'UA-9482675-1']);
            _gaq.push(['_trackPageview']);

            (function() {
            var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
            ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
            var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
            })();
        </script>
    </head>
    <body>
        <div id="wrap">
            <header>
                <div id="header_container" class="clearfix">
                    <a id="logo" href="/">Minecraft</a>
                    <ul id="menu">
                        <li><a href="/">Home</a></li>
                        <li>
                            <a href="/game">Game</a>
                            <ul>
                                <li><a href="/game">What is Minecraft?</a></li>
                                <li><a href="/game/howtoplay">Getting started</a></li>
                                <li><a href="/game/credits">Credits</a></li>
                            </ul>
                        </li>
                        <li><a href="/community">Community</a></li>
                        <li><a href="/store">Store</a></li>
                        <li><a href="/profile">Profile</a></li>
                        <li><a href="https://help.mojang.com">Help</a></li>
                    </ul>
                    <div id="userbox">
                                                <span class="logged-in">Logged in as jacksoncooley | <a href="/logout" id="logout-link">Log out</a></span>
                                                                    </div>
                </div>
            </header>

            <noscript>
            <div id="javascript-warning" class="warning warning-yellow">
                Please, please enable JavaScript to use this site.
            </div>
            </noscript>

            <div id="main" role="main" class="clearfix controller-Minecraft action-play">
                
<section class="left">
    <h1>Minecraft</h1>
                <p>
        You are currently playing an older version of Minecraft. In order to play the latest version you need to <a href="/download">download the game</a>.
    </p>
            <br/><br/><br/>
    <applet code="net.minecraft.Launcher" archive="https://s3.amazonaws.com/MinecraftDownload/launcher/MinecraftLauncher.jar?v=1374223516000" codebase="/game/" width="854" height="480">
        <param name="separate_jvm" value="true">
        <param name="java_arguments" value="-Xmx1024M -Xms1024M -Dsun.java2d.noddraw=true -Dsun.awt.noerasebackground=true -Dsun.java2d.d3d=false -Dsun.java2d.opengl=false -Dsun.java2d.pmoffscreen=false">
        <param name="userName" value="jacksoncooley">
        <param name="latestVersion" value="1374223516000">
        <param name="sessionId" value="1f9059fd3af395119f5973e598d596eff152ece3">
                        <param name="downloadTicket" value="6254b0df4b52ef4ed6e1b40e502510ca">
            </applet>
        </section>            </div>
        </div>

        <footer>
            Mojang &copy; 2009-2013. "Minecraft" is a trademark of Notch Development AB &mdash; <a href="/terms">Terms of Use</a> &mdash; b_672 r_705b0ac31512f223441a74d03ca257ff7f9dfb89
        </footer>

        <script src="/javascripts/libs/json2.js"></script>
        <script src="//ajax.googleapis.com/ajax/libs/jquery/1.5.1/jquery.min.js"></script>
        <script>!window.jQuery && document.write(unescape('%3Cscript src="/javascripts/libs/jquery-1.5.1.min.js"%3E%3C/script%3E'))</script>
        <script src="/javascripts/libs/jquery.dataTables.min.js"></script>
        <script src="/javascripts/libs/jquery.timeago.js"></script>
        <script src="/javascripts/libs/sammy.js"></script>
        <script type="text/javascript">
            var app = $.sammy('#main', function() {

                this.debug = true;

                this.get('/', function() {
                    var action = function(options) {var pattern = '/'; for(var key in options) { pattern = pattern.replace(':'+key, options[key] || ''); } return pattern }
                    this.partial(action());
                });

                this.get('/game', function() {
                    var action = function(options) {var pattern = '/game'; for(var key in options) { pattern = pattern.replace(':'+key, options[key] || ''); } return pattern }
                    this.partial(action());
                });

                this.get('/login', function() {
                    var action = function(options) {var pattern = '/login'; for(var key in options) { pattern = pattern.replace(':'+key, options[key] || ''); } return pattern }
                    this.partial(action());
                });

                this.get('/register', function() {
                    var action = function(options) {var pattern = '/register'; for(var key in options) { pattern = pattern.replace(':'+key, options[key] || ''); } return pattern }
                    this.partial(action());
                });

            });

            $(document).ready(function() {
                if ($('html').is('.history') && false) {
                    app.run(window.location.pathname);
                } else {
                    $(document).trigger('changed');
                }
            });
        </script>
        <script src="/javascripts/plugins.js?b=b_672"></script>
        <script src="/javascripts/main.js?b=b_672"></script>
            </body>
</html>
