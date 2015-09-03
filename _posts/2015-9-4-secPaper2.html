<html>
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
  <title>渗透中寻找突破口的那些事 | WooYun知识库</title>
  <base href="/">
  <meta name="fragment" content="!">
  <meta name="description" content="渗透中寻找突破口的那些事">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">
  <script>document.documentElement.className += ('ontouchstart' in window) ? ' touch' : ' no-touch'</script>
  <script src="http://wooyun.b0.upaiyun.com/static/js/jquery.min.js"></script>
  <script src="http://wooyun.b0.upaiyun.com/static/js/bootstrap.min.js"></script>
  <link rel="stylesheet" href="http://wooyun.b0.upaiyun.com/static/css/95e46879.main.css">
  <link rel="stylesheet" href="http://wooyun.b0.upaiyun.com/static/css/bootstrap.min.css">
  <style type="text/css" id="syntaxhighlighteranchor"></style>

</head>
<body ng-app="columnWebApp" ng-controller="AppCtrl" ng-class="pageClass">

  <div class="navbar-wooyun">
    <div class="home-author-wooyun">
      <a href="/" data-toggle="popover" data-placement="right" data-content="首页" data-trigger="hover" data-original-title="" title="">
        <span class="glyphicon glyphicon-home"></span>
      </a>
    </div>
    <div class="home-author-wooyun">
      <a href="/newsend" data-toggle="popover" data-placement="right" data-content="投稿" data-trigger="hover" data-original-title="" title="">
        <span class="glyphicon glyphicon-pencil"></span>
      </a>
    </div>
    <div class="bottom-author-wooyun">
      <a href="/wp-login.php?action=logout&amp;redirect_to=http%3A%2F%2Fdrops.wooyun.org" data-toggle="popover" data-placement="right" data-content="登出" data-trigger="hover" data-original-title="" title="">
        <span class="glyphicon glyphicon-log-out"></span>
      </a>
    </div>
  </div>

<main class="main-container ng-scope" ng-view="">
<div class="main receptacle post-view ng-scope">

  <article class="entry ng-scope" ng-controller="EntryCtrl" ui-lightbox="">
    <header>
      <h1 class="entry-title ng-binding">渗透中寻找突破口的那些事</h1>

      <div class="entry-meta">
        <a target="_blank" href="/author/HRay" class="author name ng-binding">
          HRay</a>
        <span class="bull">·</span>
        <time title="2014/09/02 10:28" ui-time="" datetime="2014/09/02 10:28" class="published ng-binding ng-isolate-scope">2014/09/02 10:28</time>
      </div>
    </header>

    <!-- ngIf: isCensoring -->

    <section class="entry-content ng-binding" ng-bind-html="postContentTrustedHtml">
      <p>
        <h2>0x00 寻找目标</h2>

<hr />

<p>在自己日常检测中以及观察他人检测思路发现前期收集信息具有很关键的作用，很多时候不需要对某种漏洞有很深的研究，如果前期收集了足够多的目标，只需要检测一些常见的高危漏洞即可有收获</p>

<p>常用思路</p>

<h3>1.网段信息</h3>

<p>1）通过子域名</p>

<p>如果存在域传送这种漏洞是最好的，没有的话一般就要暴破子域名了</p>

<p>我常用的软件为dnsmap，基本用法</p>

<pre><code>./dnsmap target-domain.com -w 你的域名字典 -r 要保存结果文件的绝对路径
</code></pre>

<p>针对做了泛解析的域名可以使用-i 需忽略ip来避免误报，如对域名xxx.com的暴破过程中不存在域名都解析到1.1.1.1上，则使用命令为</p>

<pre><code>./dnsmap xxx.com -w domain.txt -i 1.1.1.1 -r /tmp/result.txt 
</code></pre>

<!--more-->

<p>结果为如下格式:</p>

<p><img src="http://static.wooyun.org/201408/2014083012324194719.png" alt="2014083012324194719.png" /> </p>

<p>其中默认编译的dnsmap存在一个问题，解决方法与其他使用方法请参考</p>

<p><a href="http://pan.baidu.com/s/1nt5HMw5">http://pan.baidu.com/s/1nt5HMw5</a></p>

<p>大家可以在默认字典的基础上加一些如oa、zabbix、nagios、cacti、erp、sap、crm等等，不少企业都是这种命名方式</p>

<p>渗透的话一般会从oa，mail等重要业务网段寻找目标，如果发现有些管理后台的域名为</p>

<p>xx.admin.xxx.com这种，则可继续扩展，寻找admin.xxx.com下的三级域名</p>

<p>曾检测某站时无意发现一个ntp.nb.xxx.com的域名，进而暴破nb.xxx.com这个域名，结果如下</p>

<p><img src="http://static.wooyun.org/201408/2014083012332478937.jpg" alt="2014083012332478937.jpg" /> </p>

<p>其中zabbix.nb.xxx.com这个站点暴露到了外网，版本较低，使用zabbix的注入漏洞成功获取权限</p>

<p><img src="http://static.wooyun.org/201408/2014083012334836324.jpg" alt="2014083012334836324.jpg" /> </p>

<p>同时子域名也可通过搜索引擎语法site:xxx.com收集(不断增加条件，可获取的更多，如inurl,intitle等等)</p>

<p>2）AS号</p>

<p>Jwhois使用方法</p>

<pre><code>yum install -y jwhois
</code></pre>

<p>执行</p>

<pre><code>whois -h asn.shadowserver.org origin 1.1.1.1
</code></pre>

<p>可获得ip所在企业的AS号</p>

<p>继续执行</p>

<pre><code>whois -h asn.shadowserver.org prefix as号
</code></pre>

<p>即可获得该as号对应网段</p>

<p>注：一般只有大企业才会有as号，并且一个企业可能会有多个as号</p>

<p>3）DNS <img src="http://static.wooyun.org/201408/2014083012343269530.jpg" alt="2014083012343269530.jpg" /> </p>

<p>4）spf记录</p>

<p><img src="http://static.wooyun.org/201408/2014083012350888436.jpg" alt="2014083012350888436.jpg" /> </p>

<p>如何判断cdn？</p>

<p>如果误把cdn的ip加到目标里会影响一些人工时间，如何判断cdn？最简单的方法是用多地ping功能</p>

<p><a href="http://ping.chinaz.com/">http://ping.chinaz.com/</a></p>

<p><img src="http://static.wooyun.org/201408/2014083012353084184.jpg" alt="2014083012353084184.jpg" /> </p>

<h3>2.利用whatweb寻找web入口</h3>

<p>使用方法</p>

<pre><code>./whatweb 1.1.1.1/24 --log-brief=output_file（详细使用参考使用说明） 
</code></pre>

<p>默认的话只识别80端口的，如果此时我们想识别下8080端口，再加上--url-suffix=”:8080”即可</p>

<p>可根据title，cms等信息寻找目标，一般把后台或者存在已知漏洞的系统作为目标，同时可寻找nginx低版本存在解析漏洞的站点，受影响版本为0.5全版本，0.6全版本，0.7&lt;=0.7.65，0.8&lt;=0.8.37</p>

<p>附上一则实例：</p>

<p>在检测某企业时，whatweb批量识别指纹发现存在一台nginx版本比较低且存在解析漏洞的站点，首页为空白页，对目录结构暴破发现.bash_history文件</p>

<p><img src="http://static.wooyun.org/201408/2014083012360122353.jpg" alt="2014083012360122353.jpg" /> </p>

<p>操作历史中发现有打包文件且放在web目录下</p>

<p><img src="http://static.wooyun.org/201408/2014083012364544754.jpg" alt="2014083012364544754.jpg" /> </p>

<p>下载打包文件，内容如下</p>

<p><img src="http://static.wooyun.org/201408/2014083012371464932.jpg" alt="2014083012371464932.jpg" /> </p>

<p>其中发现有log文件，且log文件会记录user-agent信息</p>

<p><img src="http://static.wooyun.org/201408/2014083012373986307.jpg" alt="2014083012373986307.jpg" /> </p>

<p>使用firefox插件User Agent Switcher更改user-agent信息</p>

<p> <img src="http://static.wooyun.org/201408/2014083012375814489.jpg" alt="2014083012375814489.jpg" /></p>

<p>一句话代码写入log文件后利用解析漏洞直接获取webshell</p>

<p><img src="http://static.wooyun.org/201408/2014083012381959967.jpg" alt="2014083012381959967.jpg" /> </p>

<h3>3.利用nmap寻找可利用服务</h3>

<p>详细用法参考使用手册，个人常用命令为（-P0参数视情况添加，如果没有禁ping可以不加，提升速度）</p>

<pre><code>./nmap -sT -sV 1.1.1.1/24 -P0 -oN /tmp/port_result.txt --open 
</code></pre>

<p>Ip较少的情况下可以扫全端口以及一些基本信息</p>

<pre><code>./nmap -sT -sV -p 1-65535 1.1.1.1 -P0 -A
</code></pre>

<p>利用nmap可以发现一些非80/443/8080这种常见端口上的web以及一些容易出问题的端口如</p>

<p>873(rsync无验证)/21(ftp匿名账户)/11211(memcache无验证)/27017（mongodb无验证）等，碰到不认识的服务别急着放弃，去exploit-db等站点搜一下是否存在已知漏洞吧，说不准直接找到个RCE呢(很多时候我也会在乌云search一下，搜到的话就是实际例子，看着更直白)</p>

<h3>4.利用搜索引擎寻找后台或重要系统</h3>

<p>常用搜索语法为site:xxx.com inurl:login</p>

<p>Inurl的值可以自由变换，常用的包括admin、manage或者使用intitle:找管理、登录之类的关键字，有些站点出来的结果可能多数为同一站点下的误报，比如博客类的，问问类的，可使用-来减少误报，比如google中搜索site:baidu.com inurl:login -zhidao就可以在结果中去除zhidao相关的结果，百度可输入</p>

<pre><code>site:baidu.com inurl:login -site:zhidao.baidu.com
</code></pre>

<p>实例参考: <a target="_blank" href="http://www.wooyun.org/bugs/wooyun-2013-026581">WooYun: 对苏宁易购一次完整的web检测过程（多图）</a> </p>

<h3>5.搞一个精简的路径字典</h3>

<p>我们可以把容易出问题且危害比较高的常见路径做成一个精简的小字典，针对之前收集的域名去遍历，比如/invoker/JMXInvokerServlet、wwwroot.zip这种，发现的话很大几率可以搞到权限</p>

<h2>0x01 利用</h2>

<hr />

<p>这里列出几个常见的系统利用方法</p>

<h3>1. 后台</h3>

<p>当前面的过程中发现后台或者重要系统时，一般会进行如下几种检测</p>

<p>1）awvs综合扫描（经常有意外发现） 2）目录结构暴破 3）口令暴破（admin不行的时候，不一定是密码不对，很多时候是用户名不对，尝试想到的可获取用户名的一切方法，如翻翻js、css文件，html源码注释内容，或者.svn目录下的信息泄露等，密码可针对系统名称及域名等信息做一些变形加到字典中） 4）Html源码、js等文件获取信息（有些开发者会把一些管理地址以注释形式放到html源码中，管理的接口地址写在js中，运气好的话可以直接越权访问） 5）参数值暴破（一些框架写的后台登陆页面可能是这种格式xx.com/?c=login,日常可以收集一些常见的参数值，如index、main、upload、edit、adduser等、运气好的话可以直接越权操作）</p>

<h3>2. axis2</h3>

<p>文件包含：</p>

<p><a href="http://www.xxx.com/axis2/services/listServices">www.xxx.com/axis2/services/listServices</a> 查看所有services</p>

<p><a href="http://www.xxx.com/axis2/services/xxxxx?xsd=../conf/axis2.xml">www.xxx.com/axis2/services/xxxxx?xsd=../conf/axis2.xml</a> xxxxx替换任意服务均可，读取axis2配置文件获取后台账户</p>

<p><img src="http://static.wooyun.org/201408/2014083012385029649.jpg" alt="2014083012385029649.jpg" /></p>

<p><a href="http://www.xxx.com/axis2/axis2-admin/">www.xxx.com/axis2/axis2-admin/</a> 登陆管理后台</p>

<p>后台部署文件代码执行：</p>

<p>使用metasploit</p>

<p><img src="http://static.wooyun.org/201408/2014083012392773538.jpg" alt="2014083012392773538.jpg" /> </p>

<p>Resin</p>

<p>文件读取：</p>

<p><a href="http://www.xxx.com/resin-doc/resource/tutorial/jndi-appconfig/test?inputFile=/etc/passwd">http://www.xxx.com/resin-doc/resource/tutorial/jndi-appconfig/test?inputFile=/etc/passwd</a></p>

<p><img src="http://static.wooyun.org/201408/2014083012401614058.png" alt="2014083012401614058.png" /> </p>

<p>也可以通过</p>

<p>http://www.xxx.com/resin-doc/resource/tutorial/jndi-appconfig/test?inputFile=http://1.1.1.1</p>

<p>实现SSRF</p>

<p>solr敏感信息泄漏</p>

<p>http://xxx.org:8080/solr/admin/file/?file=solrconfig.xml</p>

<p>搜索xml文件，找到data-import.xml</p>

<p><img src="http://static.wooyun.org/201408/2014083012404391496.jpg" alt="2014083012404391496.jpg" /> </p>

<p>访问<a href="http://xxx.org:8080/solr/admin/file/?file=data-import.xml">http://xxx.org:8080/solr/admin/file/?file=data-import.xml</a>获取数据库密码</p>

<p><img src="http://static.wooyun.org/201408/2014083012411280552.jpg" alt="2014083012411280552.jpg" /> </p>

<p>Hudson（jenkins类似）</p>

<p>参考 <a target="_blank" href="http://www.wooyun.org/bugs/wooyun-2013-018339">WooYun: 搜狐某应用远程Groovy代码执行！</a> </p>

<p>Zenoss</p>

<p>Google关键字：intitle:"Zenoss Login"</p>

<p>默认口令admin/zenoss</p>

<p>利用方法参考</p>

<p> <a target="_blank" href="http://www.wooyun.org/bugs/wooyun-2013-019917">WooYun:  从一个默认口令到youku和tudou内网（危害较大请尽快修复）</a> </p>

<p>Zabbix</p>

<p>后台:http://www.xxx.com/zabbix</p>

<p>默认密码:admin/zabbix</p>

<p>Google:inurl:zabbix/dashboard.php</p>

<p>利用方法参考 <a target="_blank" href="http://www.wooyun.org/bugs/wooyun-2013-036277">WooYun: 应用汇zabbix运维不当导致任意命令执行。</a> </p>

<p>另外这个zabbix注入的也很多都存在http://drops.wooyun.org/papers/680</p>

<p>Cacti</p>

<p>默认登陆路径www.xxx.com/cacti/index.php</p>

<p>默认密码admin/admin</p>

<p>利用方法参考 <a target="_blank" href="http://www.wooyun.org/bugs/wooyun-2011-02674">WooYun: cacti后台登陆命令执行漏洞</a> </p>

<p>Splunk</p>

<p>默认后台地址:</p>

<p><a href="http://xxx.com:8000/zh-CN/account/login?return_to=/zh-CN/">http://xxx.com:8000/zh-CN/account/login?return_to=%2Fzh-CN%2F</a></p>

<p><img src="http://static.wooyun.org/201408/2014083012413824936.jpg" alt="2014083012413824936.jpg" /> </p>

<p>默认账户admin/changeme  默认端口8000</p>

<p><img src="http://static.wooyun.org/201408/2014083012415718222.jpg" alt="2014083012415718222.jpg" /> </p>

<p>管理器-应用-从文件安装应用处可获得shell</p>

<p><img src="http://static.wooyun.org/201408/2014083012421664684.jpg" alt="2014083012421664684.jpg" /> </p>

<p>msf有利用模块</p>

<p>exploit/multi/http/splunk&#95;upload&#95;app_exec</p>

<p><img src="http://static.wooyun.org/201408/2014083012423574417.jpg" alt="2014083012423574417.jpg" /> </p>

<h2>0x02 结尾</h2>

<hr />

<p>推荐两篇乌云综合性介绍文章</p>

<p>1.从乌云看运维安全那点事儿</p>

<p>http://drops.wooyun.org/papers/410</p>

<p>2.攻击JavaWeb应用<a href="http://ping.chinaz.com/">7</a>-Server篇<a href="http://static.wooyun.org/201408/2014083012324194719.png">1</a></p>

<p>http://drops.wooyun.org/tips/604</p>      </p>
    </section>
  </article>
  <!-- collect -->
  <div class="entry-controls clearfix">
        <div class="right-section">
          <!-- <span class="control-item read-counts">
            <i class="icon icon-eye"></i>13 人读过
          </span> -->
          <!-- ngIf: ownPost(post) -->
          <a href="javascript:void(0)" name="colloct-button" class="control-item report ng-scope fav-add">
            <i class="glyphicon glyphicon-star-empty"></i><span>收藏</span>
          </a><!-- end ngIf: !ownPost(post) && !isCensoring -->
          <!-- ngIf: !isCensoring --><div ng-transclude="" class="post-share-button post-menu-button ui-menu-button ng-scope" ng-class="{ true: 'open', false: 'close' }[open]" ui-menu-button="" onbeforeopen="beforeShareMenuOpen()" ng-if="!isCensoring">
            <a href="javascript:void(0)" class="menu-button control-item share ng-scope"><i class="icon icon-share"></i>分享</a>
            <menu class="menu ng-scope" tabindex="0">
              <!-- ngRepeat: item in shareMenuItems --><div class="menu-item ng-binding ng-scope share-weibo" tabindex="0">
              <a class="share-sina-weibo">
                <i class="icon icon-share-sina"></i>新浪微博
              </a>
              </div><!-- end ngRepeat: item in shareMenuItems -->
            </menu>
          </div><!-- end ngIf: !isCensoring -->

        </div>

      </div>

          
  <!-- collect end -->
  <!-- comment -->
  <div id="comments" class="comment-list clearfix">
            <div  class="new_comment" data-remote="true" id="new_comment">
              <div class="comment-head">
              <input type="hidden" name="comment_post_ID" value="2915"/>
                            <input type="hidden" name="nickname" value="panda">
                            <input type="input" placeholder="验证码" name="captcha"> <img id="captcha_img"  align="center" src="/wooyun/captcha.php" style="border:none; cursor:pointer" onclick="this.src='/wooyun/captcha.php?'+Math.random()"><br />
            </div>
      <div class="comment-text">
        <textarea class="mousetrap" id="comment_content" maxlength="2000" placeholder="写下你的评论…"></textarea>
        <div>
          <input class="btn btn-info" data-disable-with="提交中..." name="commit" type="submit" value="发 表">
          <span class="warning" style="display: none"><i class="fa fa-exclamation-circle"></i><span class="warning-text"></span></span>
        </div>
      </div>
  </div>
