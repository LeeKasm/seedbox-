<html>
 <head></head> 
 <body> 
  <div class="leftWrap"> 
   <div class="poster-wraper"> 
    <div itemprop="image" itemscope="" itemtype="https://schema.org/ImageObject" class="detailed_banner"> 
     <img src="https://qna.smzdm.com/201801/22/5a65b201ee06e6555.png_fo710.jpg" /> 
     <meta itemprop="url" content="https://qna.smzdm.com/201801/22/5a65b201ee06e6555.png_fo710.jpg" /> 
     <meta itemprop="width" content="710" /> 
     <meta itemprop="height" content="300" /> 
    </div> 
   </div> 
   <article> 
    <h1 itemprop="headline" class="item-name">家庭影音之路 篇一：#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程</h1> 
    <div itemprop="description"> 
     <h2 id="cl_0">开篇简介：</h2> 
     <p itemprop="description">本人最近迷恋上了PT下载，不知不觉已经摸索了近2个月了。相信各位值友们肯定好奇，一个PT有什么好摸索的？恩～正所谓内行看门道，外行看热闹。有需求的同学肯定能在我的文章中找到一些对你有用的信息。生命在于折腾！那么在定义这个系列标题的时候，我一直在思考，到底以何种形式去做1个简单明了概括？ 思来想去，还是以“家庭影音之路”为系列比较合适，因为所有的需求以及教学都是建立在这个基础之上的。日后所有关于这方面的文章都会记录在这个系列里面。</p> 
     <p itemprop="description">那么，先分析下需求，我需要什么？ 很简单，就三个字“看电影”，那么怎么才能好好的看电影呢？牵扯的东西无非就2个“硬件”“软件”。硬件方面包含的就太多了，门道也太多了，比如用什么音箱啊，用什么投影等等，太多也太复杂。但是，俗话说的好，好马配好鞍，所以给你4K屏幕，但你却拿去看720p的电影，是否太浪费了？这下“软件”的重要性就不言而喻了吧。</p> 
     <p itemprop="description"><strong>开篇废话有点多了，总的来说就是我想以一种文字的形式，记录我是如何好好“看电影”的。本系列准备告诉大家我是如何搭建线上以及线下的观影系统（包含线上seedbox的搭建，以及本地NAS的搭建，以及在线观影等等各种和“看电影”有关的小科技、小技巧、小知识）</strong></p> 
     <h2 id="cl_1">1、挑选一台线上<a class="seo_link" href="https://www.smzdm.com/fenlei/fuwuqi/" target="_blank">服务器</a>：</h2> 
     <p itemprop="description">什么是服务器？你可以理解为就是1台电脑，比如张大妈就是放在这台电脑上，然后广大值友就能愉快的交流了！</p> 
     <p itemprop="description">租用服务器的原因很简单，家里网速上传速率惨不忍睹。混1个PT站没问题，但同时混10个就有点乏力了。所以租用1台大带宽的服务器，既能满足我混PT站的需求，也能给我提供不错的线上观影体验。毕竟每次下载到本地实在太耗时了，不如在线直接看的好。</p> 
     <p itemprop="description">恩，聪明的小伙伴肯定会说了，这不就是离线下载吗？YES，没错。所以我们物尽其用！当然是需要花成本的！至于成本的多少，取决你的需求。不想折腾的小伙伴也可以iqiyi，2个月前我一直在用- -，后来被我果断放弃了，现在就老婆1个人在用了。</p> 
     <p itemprop="description">正如上文所说我的需求是混PT，以及在线观影，那么服务器的带宽是不能少的，而且<a class="seo_link" href="https://www.smzdm.com/fenlei/yingpan/" target="_blank">硬盘</a>得大，毕竟一部影片小的几个G，大的几十G，一部蓝光怎么也得50G吧。而且，最重要的1点价格得便宜啊。资金有限。我们要充分的发挥“值”这个字的魅力才行。</p> 
     <p itemprop="description">那么国内的是不用考虑了，因为硬盘和带宽的价格实在感人。1个月怎么也得4位数。所以我们吧目标放在了国外，那国外便宜的服务器其实也很多，但是大部分都限制流量。当然这些流量如果你不混PT站的话，肯定是用不完的。所以无需担心，但是我的需求是要混PT。所以肯定得无限流量了。最后锁定了oneprovider法国的服务器。优点：硬盘大，带宽大，混PT完美 &nbsp; 缺点：连通过内速度较慢 Ping值有300+ &nbsp;不过无所谓了后面会单独开一篇文章教大家如何使用加速。（当然也可以选择其它连通性好的地区，具体这里我就不详细说了，国外服务器连国内，主要看地理位置，要么就是CN2的线路）还是那句话，根据你的需求来的。</p> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_2/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65919cdc96c4260.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">最终选择了这台，15欧元，折合成RMB约120元吧，比起国内动辄4位数的独服，简直美的不要不要的了。从配置上可以看出1G的带宽，2TB的硬盘，I3-530的U，双核四线程。中规中矩。当然选择第一个也可以，只不过CPU实在惨不忍睹。我直接给PASS了。至于怎么购买，只要你有paypay就可以了，没有？也没关系，注册1个，绑定国内银联卡付款的。看不懂英文？没关系，装个浏览器插件，翻译当前网页，就这么嗨皮。（我就是这么干的，哈哈）</p> 
     <h2 id="cl_2">2.在线重装服务器系统</h2> 
     <p itemprop="description">网站后台是可以直接通过控制面板重新装系统的，当然你也可以自己通过DD的方式重新装，网上各位大牛写了不少一键脚本，特别方便。建议别用windows，国外的这个连通性，能卡成翔，而且关键是服务器预装windows系统需要收费啊，那价格够你在买几个月的了。我一般都用linux，系统选 Debian 或&nbsp;Ubuntu 。除非国内的服务器或者亚洲的服务器我才会用 windows的系统。linux也没有想象中的那么难，最起码我接触到稍微了解，也就花了2天的时间。说白了就是不用图形界面，全部靠命令执行，当然也可用界面，问题是，那我干嘛不直接用Windows？</p> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_3/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a6596041ebc46068.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">上面这张图是预装的系统，Debian7 64位。至于为啥要重新装？因为服务商给你装的系统肯定是定制过的，所以我们要装1个原汁原味的才行。下面开始通过DD的方式重新装Ubuntu16.04 系统（不想重新安装系统的同学可以直接跳过这一步）。</p> 
     <p itemprop="description">首先先下载1个工具 &nbsp;PuTTY &nbsp;并打开它，再根据服商给你提供的 &nbsp;IP address、Username、Password &nbsp;连接我们的服务器。就像下面一样图一样，输入好IP之后然后点击Open 就连上去了。然后分别输入账号和密码（密码输入的时候是不会显示字符的，所以不要怀疑你的<a class="seo_link" href="https://www.smzdm.com/fenlei/jianpan/" target="_blank">键盘</a>是否坏了）</p> 
     <h3>输入IP地址，点击Open</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_4/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://am.zdmimg.com/201801/22/5a6597c8e30c66446.png_e600.jpg" title="" /></a></p> 
     <h3>输入UserName 然后回车</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_5/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a6597caecb4a289.png_e600.jpg" title="" /></a></p> 
     <h3>输入Password 然后回车</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_6/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a6597cd2a4476374.png_e600.jpg" title="" /></a></p> 
     <h3>OK，出现如下界面就代表登录成功了！<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_7/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a6598864dc4f2428.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">下面我们将用国内某大神写的一键DD脚本进行重装系统，流程就是复制粘贴复制粘贴。（复制后对着Putty窗口<a class="seo_link" href="https://www.smzdm.com/fenlei/shubiao/" target="_blank">鼠标</a>右键就能粘贴进去了，这个小技巧一定要知道噢，千万别手打，不仅容易错还累人。。）以下的输入命令直接复制就行了，复制完记得敲回车。一定要复制完全！而且等一条命令执行完毕之后在执行下1条命令。不要着急，面对未知你是焦躁的，但是我们一定要有耐心。</p> 
     <h3>输入命令：&nbsp;apt-get install -y gawk sed grep &nbsp; &nbsp;</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_8/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659a115241385.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：wget --no-check-certificate -qO DebianNET.sh 'https://moeclub.org/attachment/LinuxShell/DebianNET.sh' &amp;&amp; chmod -x DebianNET.sh</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_9/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659bda7eb4d1338.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：bash DebianNET.sh -u xenial -v 64</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_10/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659c26d8f838812.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：n<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_11/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659c94b400e198.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">到这里服务器就开始重装了！你会看到窗口在不停的跳出命令，最终命令卡在“170511 blockss”这里不动了。那是因为服务器重启了，开始重新装系统了！这时你就可以关闭putty这个窗口了。因为已经断开了连接，</p> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_12/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659d428c7fc1584.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">我们只需要等待服务器重装完毕即可再次登录，那么如何检测是否安装完呢？很简单能ping通就没问题了</p> 
     <h3>按 Win+R ，然后出入cmd<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_13/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://am.zdmimg.com/201801/22/5a659e0685a029370.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：Ping xx.xx.xx.xx &nbsp;-t &nbsp; ( xx.xx.xx.xx 是你的IP地址)</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_14/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659eb6e79ae7916.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">如图所示，能Ping通了，就代表服务器重装好了。安装速度取决于你的服务器配置，如果你用的和我一模样的服务器，那么几分钟搞定。这里有一点要提示一下，重装有风险的，如果你没有把握，我建议你还是别装。当然万一出错了，服务器打不开了。进入网站后台面板，重新安装服务商提供的系统就行了。</p> 
     <h3>重新装过之后，我们再次登录服务器，新的账号是 root &nbsp;密码是 Vicer &nbsp;，我们用这个账号密码登入服务器。</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_15/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a659fd488c975590.png_e600.jpg" title="" /></a></p> 
     <h3>至此系统已经重装好了，可以看到版本是 Ubuntu 16.04 ，下面我把初始密码改一下。<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_16/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a02f521de8405.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：passwd root<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_17/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a07c624918292.png_e600.jpg" title="" /></a></p> 
     <h3>然后出入两边密码，最后提示 successfully 就代表修改成功，以后登录就用root 和你的新密码即可。</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_18/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a0b9f27bf9967.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">至此，服务器重装的部分就结束了，恭喜你拥有了1个干净完整的Linux系统。你可以尽情的折腾了。这里有一点要说一下，如果你有的服务商提供了VNC，那么你可以通过VNC登录，观看重装过程。当然没有也没关系，脚本是自动安装的。不过不保证所有机器都能适用。我试了2台服务器都完美重装，所以应该没什么大问题吧。下面将给大家带来的是Rutorrent的安装说明。<br /></p> 
     <h2 id="cl_3">3.安装Rutorrent （种子专用下载工具）</h2> 
     <p itemprop="description">为了篇幅的大小，这里我采用的也是一键脚本，毕竟手工安装实在是太费篇幅了，光截图估计就能让我吐血。哈哈，所以这里主要是给大家演示下如何用 一键脚本安装Rutorrent<br /></p> 
     <h3>输入命令：bash -c &quot;$(wget --no-check-certificate -qO - https://raw.githubusercontent.com/arakasi72/rtinst/master/rtsetup)&quot;</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_19/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a637cfce67067.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：rtinst -t<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_20/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a649b48362939.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description">然后会有各种提示的信息，看不懂没关系，跟着截图一步一步走就好了。一会输入的账号密码，不要填写你服务器的登录账号密码，这个新的账号密码，是用于网页后台登录管理用的。你可以自定义1个账号 1个密码。最终安装完毕后，我们登录网页客户端时会用到这个创建好的账号密码。OK，下面开始一步一步截图输入命令。</p> 
     <h3>输入命令：y &nbsp; &nbsp;（这个是向你确认你的服务器IP对不对，直接输入y，然后回车就行）</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_21/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a9a820f711970.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：这里输入你需要创建的网页管理账号就行了，自定义的，比如：xiazai</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_22/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65a9e6d98063377.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：y &nbsp;（确认用的）<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_23/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65aa2de836f1589.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：需要创建的密码，也是自定义，需要输入两边，密码输入不显示字符，输入好，直接回车即可</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_24/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65aa867f62b143.png_e600.jpg" title="" /></a></p> 
     <h3>输入命令：把上面输入过的密码，再次输入两边，同样不显示字符，输入好，直接回车即可</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_25/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://am.zdmimg.com/201801/22/5a65aae4484a95900.png_e600.jpg" title="" /></a></p> 
     <h3>OK，出现这个提示就代表正在安装了，安装速度取决你服务器配置，目测10分钟不到全部装完。<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_26/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://qnam.smzdm.com/201801/22/5a65ab17e1efc7162.png_e600.jpg" title="" /></a></p> 
     <h3>出现这个界面，就代表了安装成功，上面也提供了网页后台的地址，就是你的http://IP/rutorrent&nbsp; 然后我们可以通过这个后台，用上面创建好的账号密码登录。就行了！</h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_27/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://am.zdmimg.com/201801/22/5a65ab82771784306.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description"><br /></p> 
     <h3>登录后台，开始用的服务器进行下载吧！<br /></h3> 
     <p itemprop="description"><a href="https://post.smzdm.com/p/a767rnl/pic_28/" target="_blank"><img alt="#原创新人#服务器安装Rutorrent（PT盒子）Seedbox教程" src="https://am.zdmimg.com/201801/22/5a65ac915c7e32505.png_e600.jpg" title="" /></a></p> 
     <p itemprop="description"><br /></p> 
     <p itemprop="description">rutorrent到此就算安装完毕了，你可以通过服务器下载种子了，至于怎么在线播放，以及如何把服务器上下好的文件拖回本地。或者是一些服务器速度方面的相关优化。我将会在下一章给大家详细介绍。本教程是基于Linux的，如果你有<a class="seo_link" href="https://pinpai.smzdm.com/2315/" target="_blank">群晖</a>或者装有Transmission的机器，可以直接使用无需在装rutorrent。我用rutorrent的主要原因是，在通过浏览器管理的下载工具中，算是功能强大的了，只不过只能下载种子文件，直链是无法下载的。所以具体怎么选择，需要考虑清楚。根据需求来定夺吧。</p> 
    </div> 
   </article> 
  </div>      
  <article> 
   <h1 itemprop="headline" class="item-name">家庭影音之路 篇二：PT盒子服务器参数优化以及Rutorrent设置调整</h1> 
   <div itemprop="description"> 
    <h2 id="cl_0">开篇简介：</h2> 
    <p itemprop="description">上一篇给大家介绍了如何租用一台法国的大带宽、大硬盘的独立<a class="seo_link" href="https://www.smzdm.com/fenlei/fuwuqi/" target="_blank">服务器</a>，以及如何在线重新安装linux系统和如何安装ruotrrent（种子下载工具）。那在上一篇文章中，有一点忘记和大家说了，<strong>如果你自己租用的是VPS，而非独立服务器，重装系统前必须确认你的服务器虚拟架构是KVM的，而且还要保证是GRUB引导的才行</strong>。如果不是，或者不知道自己的VPS是什么架构，没关系本文将会给大家介绍如何检测自己VPS的虚拟化架构。当然了，做教程肯定是要尽量全面的，如果各位小伙伴觉得实在麻烦，不重新安装系统也是可以的。</p> 
    <h2 id="cl_1">温馨提示：</h2> 
    <p itemprop="description">鉴于很多小伙伴还不理解PT是什么意思，我大概解说下。BT下载相信大家应该都知道的吧，如果不知道的可以百度一下，那么PT其实就是BT的延伸版本。简单点说，PT就是小团体的“私有”下载。BT是大团体的“共有”下载。那既然是“私有”肯定是需要验证的，在你下载的时候PT站会对你的账号进行验证，确定你是他们的成员后才会让你下载他们的种子，而且下载时会记录你的分享率，如果你的分享率过低，那么会封掉你的账号。所以PT站点下载种子的速度基本上都能达到你本地带宽的满速。</p> 
    <p itemprop="description">那么话说回来，我们在“服务器”上下载PT种子到底有没有“事”？有的小伙伴会问了，我们用服务器下载种子，服务商会不会封掉我们的服务器？对于这个问题，我想告诉大家。如果你只是下载PT站点的种子，那么问题就不大了，不过有些服务商给你提供的带宽是共享的，因为PT下载基本接近带宽的满速，你长时间占用人家网速，人家会给你限速，甚至有可能封掉，当然这种情况VPS居多。<strong>所以非独享带宽的服务器请适当限速。非独立服务器的请低调下载。</strong></p> 
    <p itemprop="description">俗话说的好，知己知彼百战不殆，那什么情况下会让服务商封掉你的服务器呢？这里就要说1个关键词了“DMCA”数字千年版权法，想了解的小伙伴可以百度一下。简单点说，如果你下载的是BT种子，也就是所有人都能下这个种子，那么一些坏叔叔也会去下载，然后他们会根据你的IP，投诉到你的服务商那里，然后你的服务商扛不住压力就封了你的服务器。反正总之记住一句话，<strong>如果你是用BT种子的下载，那么请租用 抗“DMCA”的服务器。</strong>PT种子的话基本可以无视这个了。暂时就介绍这么多，再说就跑题了。</p> 
    <p itemprop="description">---------------------------------------------------------------------------------------------------</p> 
    <p itemprop="description">那本节主要是教会大家，如何调整自己服务器的参数，以及如何给rutorrent进行一些优化。本次篇幅比较长，主要是为了照顾第一弄的新手们，所以每个步骤我都给细化了。毕竟光靠三言两语是没有办法让一位萌新学会的。</p> 
    <h2 id="cl_2">一、开启Root登录</h2> 
    <p itemprop="description">上一章通过教程教会了大家如何在线安装Rutorrent，那么已经通过我的教程安装过的小伙伴，相信都出现了1个问题，那就是初始的root账号无法登录了。原因是之前使用的一键脚本，这个脚本为了服务器的安全性，故而关闭了root登录，我们只需要用新创建的账号密码去登录就可以了，然后修改设置再次开启root登录即可。下面就跟着教程来做一遍吧。</p> 
    <p itemprop="description"><strong>打开putty并open你的服务器</strong> （账号密码，就是之前你创建的网页账号密码）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_2/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670a34ad9846943.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>输入命令：sudo su </strong>&nbsp; &nbsp;（这一步是告诉系统我们要进入root模式）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_3/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670ac3546992920.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>输入命令：你的密码</strong> &nbsp; &nbsp;（确认用的，密码输入不可见，输入完直接回车就行）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_4/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670afff05355665.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">然后就会出现下面这张图，有 “root@” 这几个字符就证明你已经在root模式中了，然后就可以继续进行下去了。一定得是在root模式下进行才可以，不然权限不够，我们无法修改某些关键性文件的。（本教程是在Ubuntu系统上进行的，如果你是Debian系统那么进入root的命令 应该是 su ，系统不一样进入的方法也不一样）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_5/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670b7a7fa466494.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>输入命令：vi /etc/ssh/sshd_config</strong> &nbsp; &nbsp; （这步是通过VI命令修改文件，有点类似操作<a class="seo_link" href="https://www.smzdm.com/fenlei/bijiben/" target="_blank">记事本</a>，只不过Linux上面比较麻烦，大家跟着教程做就可以了）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_6/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670d1703c253452.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>输入命令：回车</strong> &nbsp; &nbsp; （如下图所示 按enter 后才可以继续）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_7/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670d81189669290.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">出现下面这个就代表成功进入了我们要修改的文件（切记，<strong>这个时候不要乱动你的键盘</strong>，因为这个模式下代表了修改文件，你的任何小动作，都会导致修改失败。因为某些修改命令就在你的键盘上，所以必须得跟着教程一步一步走。当然如果你知道如何修改，那么可以直接操作，但是没弄过的小伙伴，不知道如何修改的小伙伴，一定一定不要心急，请仔细仔细再仔细跟着教程弄！）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_8/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a670e00bfc304496.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">这里需要给大家简单介绍下，我们需要使用到的按键，这些按键是修改文件用的！大家粗略了解一下，一会跟着教程弄的时候就不会那么蛋疼啦！<strong>命令是分大小写的，请把你的键盘切换成小写模式</strong>（不要在Putty窗口切换噢，随便找个能打字的地方，测试下你的键盘输入模式是不是小写模式）</p> 
    <p itemprop="description"><strong>需要用到的功能按键： &nbsp;ESC &nbsp; &nbsp;i &nbsp; x &nbsp;←↑ ↓→</strong>&nbsp;（ i 和 x 都是小写状态的 ，ESC就是你键盘左上角那个按键，上下左右就是键盘右边的方向键）如下图所示。</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_9/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a6711649cbff9863.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">ESC ：这个按键是切换模式用的，你可以把它理解为还原，做过任何操作后都要按它还原成初始操作状态。</p> 
    <p itemprop="description">方向键：这个是用来移动光标位置的，移动之前请多按几下ESC，避免出错。</p> 
    <p itemprop="description">i ： 小写的 i ，这个按键是告诉系统 在当前光标处插入字符，字符输入是连续的哦，退出时要按ESC</p> 
    <p itemprop="description">x&nbsp;：&nbsp;小写的 x ，这个按键是告诉系统，在当前光标位置删除1个字符。</p> 
    <p itemprop="description">好的，简单了介绍了一下这几个按键的作用，那么下面就跟着教程一步一步的进行操作吧。</p> 
    <p itemprop="description">-------------------------------------------------------------------------------------------</p> 
    <p itemprop="description"><strong>1、对着Putty窗口，先按几下ESC，然后一直按 ↓ 方向键，直至到达 “PermitRootLogin no”这一行。</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_10/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672c6d391191966.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>2、接着按→方向键，把光标移动到 “n”这个字符上。</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_11/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672cd493875186.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>3、接着按 &nbsp;两次“x”</strong>（目的是把no这两个字符给删除了）如下图所示</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_12/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672d1c213f68190.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>4、接着按 &nbsp;一次 “i” </strong>&nbsp;（进入插入字符模式，按1次就可以了！！然后千万别乱按键盘，因为是插入模式，所以你所有的按键操作都会写入到这个文档里面）&nbsp;</p> 
    <p itemprop="description"><strong>5、接着依次按 &nbsp;“空格”“y”“e”“s” ，把这4个字符输入进去。</strong>（输入完后别动键盘！）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_13/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672e22944987725.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>6、接着按几次ESC </strong>（意思是退出插入模式，按完后你会发现绿色光标移动到了s这个字母上了，代表了切换模式成功，这时候你就又可以通过方向键移动光标了）<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_14/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672e964b2218365.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>7、然后再次通过方向键移动光标至“AllowGroups sudo sshuser”这一行，并把绿色的光标移动到最左边“A”这个字符的上面。</strong>（我的这行字是在文档的最后，如果没有这行字的话那可以跳过7、8、9、10这几个步骤！）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_15/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a672f197133b7592.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>8、接着按 一次“i” </strong>（继续进入插入模式）<br /></p> 
    <p itemprop="description"><strong>9、接着按 一次 组合键 &quot;Shift + 3<span style="color:rgb(51,51,51);">&quot; &nbsp;</span></strong><span style="color:rgb(51,51,51);">（也就是把“#”这个字符给输入进去！）</span></p> 
    <p itemprop="description"><strong>10、接着按一次 `ESC。把它弄成和下图一模一样就行了。</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_16/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a6730305eb726961.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>11、按一次组合键 &nbsp;Shift + 冒号键</strong> &nbsp;（就是平时你输入冒号时的按法），这时你会发现光标跳到了最下面，并且前面有1个冒号。（注意这个时候就别乱按键盘了噢！我们还有1个步骤就成功了！）<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_17/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a67310cc0c3e5018.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>12、接着依次按 “w”“q”</strong>（把这两个字符给输入进去！）<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_18/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a67317191c204813.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>13、接着 按回车键，就保存了！</strong>&nbsp; &nbsp;（然后回跳回到一开始输入命令的地方。如下图所示。）<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_19/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a6731f72944d2418.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>14、输入命令：service ssh restart </strong>&nbsp; &nbsp;（这一步是让我们刚才修改的内容生效！）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_20/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a67389c3ed306307.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">至此，我们已经成功的给服务器开启了Root的登录权限，各位小伙伴们可以继续使用之前的 root + 密码 ，来登录服务器了。那么，有的同学可能会问了，我不修改这一步可以吗？ 恩，如果你能root登录，当然可以不用修改，<strong>如果不能用root账号进行登录，那么必须进行修改。因为后面的优化设置，必须要用到root账号的。</strong>所以，我才把开启root登录放在了本章第一节进行讲解。</p> 
    <p itemprop="description">-------------------------------------------------------------------------------------------</p> 
    <h2 id="cl_3">二、去掉“HTTPS”使用“HTTP”进行网页访问<br /></h2> 
    <p itemprop="description">当我们安装好Rutorrent之后，访问我们的WebUI的时候，会发现浏览器提示我们的网页不安全，而且在网址那一栏会有1个大大的X。如下图所示，这时我们就需要开始第一次的小优化了。（当然这个只是1个安全性的提示，对实际功能没有一点影响，不想修改的同学可以跳过）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_21/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a67360b3a6098794.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>1、下载WinScp这个工具安装它然后打开。</strong>（这个工具可以很方便的修改我们服务器上的文件，当然前提是要开启Root登录，不然系统的核心文件是没办法用这个工具修改的）后面的教程都会使用WinScp和Putty这2个工具配合。</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_22/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a67368feba4e6450.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>2、点击新建站点，然后在填入服务器相关信息，并登录到服务器</strong>（如下图所示）<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_23/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a6737996c2ee5965.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">登录进去后就像下面这张图一样，这里面的文件列表都是你服务器上的资源，我们可以用这个软件给服务器上的文件进行编辑，特别方便。也可以进行文件传输等操作。当然你也可以用它把你服务器上下载好的文件给拖回本地，当然这个方法不是最好的，后面会教大家1个更好的办法。那么废话不多说，我们继续进行设置。</p> 
    <p itemprop="description"><strong>3、进入<a class="seo_link" href="https://www.smzdm.com/fenlei/wenjianjia/" target="_blank">文件夹</a>：/etc/nginx/sites-enabled</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_24/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a673b5da916a2367.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>4、对着 “default”这个文件右键，然后点击编辑。</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_25/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/23/5a673bab808671829.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">鼠标点过编辑之后就会出现下面这个界面，是不是有点像记事本。恩，没错，我们后面的修改教程，都是通过这个进行的。有了WinScp这个工具，世界都变得美好了。<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_26/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a681bd48dfb61395.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>5、把这个文件里面所有的信息给删掉，然后替换成下面的文本。</strong>（listen 666 代表了监听的端口号）</p> 
    <blockquote> 
     <p itemprop="description"><strong>server {</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; listen 666;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; root /var/www/rutorrent;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; index index.html index.php index.htm;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; client_max_body_size 40m;</strong></p> 
     <p itemprop="description"><br /></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; location / {</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;client_max_body_size 40m;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;auth_basic &quot;Restricted&quot;;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;auth_basic_user_file /etc/nginx/.htpasswd;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;include /etc/nginx/conf.d/php;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;include /etc/nginx/conf.d/cache;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; }</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; location ~ /.ht {</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; deny all;</strong></p> 
     <p itemprop="description"><strong>&nbsp; &nbsp; &nbsp; &nbsp; }</strong></p> 
     <p itemprop="description"><strong>}</strong></p> 
     <p itemprop="description"><br /></p> 
    </blockquote> 
    <p itemprop="description">就像下面这张图片一样，把上面这段代码给粘贴进去，替换掉原来的代码。<strong>然后CTRL+S （保存）</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_27/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a681e6c74c0c9979.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>6、Putty输入命令：service nginx restart</strong> &nbsp; &nbsp; &nbsp;（这步的意思是重启下我们的网页）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_28/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a681ffe84cbb2270.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">好的，这个时候你在访问我们的网页客户端就没有那个提示了，不过我提供给大家的这串代码，把网址给变动了一下,<strong>变成了IP+端口号的访问</strong>（这步的目的主要是为了配合后面教程），所以这个时候你访问原来的网址是没有效果了。需要用下面新的网址进行访问！</p> 
    <blockquote> 
     <h3>http://你的IP地址:666&nbsp; &nbsp;&nbsp;（例如：http://123.123.123.123:666）&nbsp;&nbsp;&nbsp;前面是 http://&nbsp; 没有S &nbsp;切记！&nbsp;<br /></h3> 
    </blockquote> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_29/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://am.zdmimg.com/201801/24/5a68233aa866d7821.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">-------------------------------------------------------------------------------------------</p> 
    <h2 id="cl_4">三、给服务器跑个分</h2> 
    <p itemprop="description">服务器的性能究竟如何？这是个非常有学问的东西，我们用服务器进行PT下载，最明显的就是下载速度和上传速度了。那么大家肯定想知道服务器的极限在哪里把，知道了极限才能进行相关的优化，不然明明给你1G的带宽，你却跑出了200MB的带宽，岂不是没有把“值”这个字进行到底？</p> 
    <p itemprop="description">影响上传和下载速度的牵扯的东西特别多，但是无外乎就2个字“配置”，首先就是服务器的“带宽”。1GBPS的服务器不一定能跑出100MB/S的速度，所以我们要进行测试，那光检测速度肯定是不够的，影响上传速度的，还有1个参数“硬盘IO”。相信说道这个大家应该能有所共鸣，不然<a class="seo_link" href="https://www.smzdm.com/fenlei/gutaiyingpan/" target="_blank">固态硬盘</a>和<a class="seo_link" href="https://www.smzdm.com/fenlei/putongyingpan/" target="_blank">机械硬盘</a>怎么会是1个天1个地呢？当然了，CPU的好坏也会影响我们的上传和下载速度。因为在高速的上传和下载中，对CPU的依赖也是不小的。当然这也取决于你下载工具的性能。有些工具，下载速度一般，但是贵在稳定，有些工具是速度特别快，但是对CPU特别依赖，经常跑满CPU。最最尴尬的就是卡硬盘IO了。这个是硬瓶颈，我们着重优化的也是这个。但是有一句话，是不会错的，一分价钱一分货，举个例子：昨天刚帮一个朋友安装了1台服务器。他买的是25欧的并且没有做任何优化。结果这台服务器的速度却是我15欧服务器2倍左右。</p> 
    <p itemprop="description">服务器测速也不难，因为网上有很多大神写了不少一键测速脚本。对于我等小白来说，简直就是美滋滋。OK，那我们就选1个脚本，来给服务器跑1个分看看性能就然如何把！</p> 
    <h3>输入命令：wget https://raw.githubusercontent.com/FunctionClub/ZBench/master/ZBench-CN.sh &amp;&amp; bash ZBench-CN.sh</h3> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_30/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://am.zdmimg.com/201801/24/5a682cbedfaa92000.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">然后，就是1次小小的等待，脚本这个时候会先下载所依赖的运行库，然后自动检测服务器的配置，硬盘IO、传输速率，以及全球范围类的上传下载速度、ping值、路由表信息等等。当然了，IO、传输速率这些，我们只需要参考一下就行了。大概知道服务器处于什么样的水平就行。比如参数中的 CacheFly 基本上就是你带宽的总速度了。所以真正的上传+下载的传输速率之和，应该接近这个值才算满速。<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_31/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://am.zdmimg.com/201801/24/5a682e689e18d1011.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">-------------------------------------------------------------------------------------------</p> 
    <h2 id="cl_5">四、优化Linux的参数</h2> 
    <p itemprop="description">Linux这个系统，说心里话我也是个小白，对于服务器如何优化，也是google了一大堆文章，最终实测了一下，发现效果还是不错的，亲身经历，法国这台15欧的服务器，原先只能跑到30mb/s的速度，经过优化之后是真的跑到了80mb/s，基本上达到了这台服务器的满速带宽。不过有一个缺点就是不太稳定，我也在尽力的寻找更加妥善的优化速度的方案。所以，如果你觉得你服务器耐折腾，你觉得目前你的服务器速度让你不是很满意的，或者喜欢专研的小伙伴。可以尝试根据我提供的方法进行一些优化设置。<strong>（</strong><strong>优化有风险，操作需谨慎，重装是常事）</strong><br /></p> 
    <p itemprop="description">特别提醒：如果你正在用rutorrent进行下载，请先停止下载任务。因为优化后需要重启系统。所以会导致正在下载的文件下次启动的时候会重新校验<strong>！强烈建议在优化的时候不要有任何下载行为</strong>，因为不怕一万就怕万一，如果优化出错，导致系统打不开等等之类的就得不偿失了。</p> 
    <p itemprop="description"><strong>1、WinScp编辑文件：/etc/fstab</strong></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_32/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://am.zdmimg.com/201801/24/5a6835661c9f87018.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>2、插入代码 noatime &nbsp;到 errors=remount-ro 的前面 &nbsp;&nbsp;</strong>分隔符为逗号（请参考下图）然后保存！<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_33/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a68375947b71513.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">这一步的目的是，让系统不给文件做时间记录，因为我们在进行PT下载的时候，会有大量的硬盘读写行为，而默认情况下linux会把文件访问的时间atime做记录，比如最近一次的访问时间、最近的一次的修改时间等等。所以这里我们设置为 noatime 将会显著提高磁盘 IO 的效率、提升文件系统的性能。&nbsp;（其实按照google上面的说法 加入data=writeback 也能提高IO，问题是，我加入了这个参数后，部分服务器失败，只有一台成功。因为自己技术有限，也不知道什么原因导致的，所以稳妥起见，还是不要加入这个了，只需要 noatime 这个参数就行。）</p> 
    <p itemprop="description"><strong>3、WinScp编辑文件：/etc/sysctl.conf</strong> &nbsp; &nbsp; （把下面的文本复制到这个文件底部，<strong>注意最后要有1个换行符</strong>）</p> 
    <blockquote> 
     <p itemprop="description">vm.swappiness = 1</p> 
     <p itemprop="description">fs.file-max = 2000000</p> 
     <p itemprop="description">kernel.pid_max = 4194303</p> 
     <p itemprop="description">kernel.sched_migration_cost_ns = 5000000</p> 
     <p itemprop="description">kernel.sched_autogroup_enabled = 0</p> 
     <p itemprop="description">net.ipv4.tcp_slow_start_after_idle = 0</p> 
     <p itemprop="description">net.ipv4.tcp_no_metrics_save = 0</p> 
     <p itemprop="description">net.ipv4.tcp_abort_on_overflow = 0</p> 
     <p itemprop="description">net.ipv4.tcp_window_scaling = 1</p> 
     <p itemprop="description">net.ipv4.tcp_tw_reuse = 1</p> 
     <p itemprop="description">vm.dirty_background_ratio = 20</p> 
     <p itemprop="description">vm.dirty_ratio = 30</p> 
     <p itemprop="description">net.ipv4.tcp_rfc1337 = 1</p> 
     <p itemprop="description">net.ipv4.tcp_sack = 1</p> 
     <p itemprop="description">net.ipv4.tcp_fack = 1</p> 
     <p itemprop="description">net.ipv4.tcp_workaround_signed_windows = 1</p> 
     <p itemprop="description">net.ipv4.tcp_timestamps = 1</p> 
     <p itemprop="description">net.ipv4.tcp_syncookies = 1</p> 
     <p itemprop="description">net.ipv4.tcp_syn_retries = 2</p> 
     <p itemprop="description">net.ipv4.tcp_synack_retries = 2</p> 
     <p itemprop="description">net.ipv4.tcp_orphan_retries = 2</p> 
     <p itemprop="description">net.ipv4.tcp_retries2 = 8</p> 
     <p itemprop="description">net.ipv4.ip_local_port_range = 1024 65535</p> 
     <p itemprop="description">net.core.netdev_max_backlog = 3240000</p> 
     <p itemprop="description">net.core.somaxconn = 50000</p> 
     <p itemprop="description">net.ipv4.tcp_max_tw_buckets = 1440000</p> 
     <p itemprop="description">net.ipv4.tcp_max_syn_backlog = 3240000</p> 
     <p itemprop="description">net.ipv4.tcp_mtu_probing = 1</p> 
     <p itemprop="description">net.ipv4.tcp_fin_timeout = 15</p> 
     <p itemprop="description">net.ipv4.tcp_keepalive_time = 600</p> 
     <p itemprop="description">net.ipv4.tcp_keepalive_intvl = 10</p> 
     <p itemprop="description">net.ipv4.tcp_keepalive_probes = 9</p> 
     <p itemprop="description">net.ipv4.ip_no_pmtu_disc = 0</p> 
     <p itemprop="description">net.core.rmem_default = 16777216</p> 
     <p itemprop="description">net.core.wmem_default = 16777216</p> 
     <p itemprop="description">net.core.optmem_max = 16777216</p> 
     <p itemprop="description">net.core.rmem_max = 16777216</p> 
     <p itemprop="description">net.core.wmem_max = 16777216</p> 
     <p itemprop="description">net.ipv4.tcp_fastopen = 3</p> 
     <p itemprop="description">net.ipv4.tcp_rmem = 4096 87380 16777216</p> 
     <p itemprop="description">net.ipv4.tcp_wmem = 4096 65536 16777216</p> 
     <p itemprop="description">net.ipv4.tcp_adv_win_scale = 2</p> 
     <p itemprop="description"><br /></p> 
    </blockquote> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_34/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a683e8de68a55926.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">这一步的目的是修改Linux的内核参数，主要优化TCP等协议参数，调优网络质量。如果你之前就有过这方面的设置，或者用过别的脚本，比如开启BBR的时候顺带优化了这个参数。可以参考如上配置进行适当的修改即可。（What？啥是BBR？ 好吧，那是下一篇文章主要讲解的内容）</p> 
    <p itemprop="description">值得一提的是 &nbsp;vm.swappiness = 1 &nbsp; 这个参数是告诉服务器对SWAP 分区的依赖程度。这样说很难理解，你可以把它理解为windows的虚拟内存。当物理内存不足时，会调用这个虚拟内存作为补充使用，从而使得系统稳定。那么虚拟内存大家都知道是存放在硬盘上的。所以过多的使用SWAP，也就会造成过多的读写硬盘，那么你的硬盘IO速度就降低了。所以，通过调整vm.swappiness这个参数的值，可以告诉linux系统如何使用SWAP。一般默认情况下他的值是60，如果你内存足够大，比如25欧的那款服务器有16G的内存，完全用不掉啊，就可以设置为1。我这里设置的是0，当然不是禁用了SWAP，而是告诉系统能少用就少用，能不用就不用。具体怎么选择看亲们自己定吧</p> 
    <p itemprop="description"><strong>4、WinScp编辑文件：/etc/security/limits.conf</strong> &nbsp; &nbsp;（把下面这些参数给复制进去）然后保存！</p> 
    <blockquote> 
     <p itemprop="description">* soft nofile 2000000&nbsp;</p> 
     <p itemprop="description">* hard nofile 2000000</p> 
     <p itemprop="description">root soft nofile 2000000&nbsp;</p> 
     <p itemprop="description">root hard nofile 2000000</p> 
    </blockquote> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_35/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/25/5a696169a03db2896.png_e600.jpg" title="" /></a>这一步的目的是，增加最大打开的文件数，对于PT下载这种频繁使用到文件读写的。当然得调整了。</p> 
    <p itemprop="description"><strong>6、WinScp编辑文件：/home/登录账号/.rtorrent.rc</strong> &nbsp; （登录账号就是你网页使用的账号名称）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_36/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a6845d0d176d9659.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>修改：</strong>（寻找下面这些参数名称，并修改它的数值）</p> 
    <blockquote> 
     <p itemprop="description">throttle.max_downloads.global.set = 0</p> 
     <p itemprop="description">throttle.max_uploads.global.set = 0</p> 
     <p itemprop="description">throttle.min_peers.normal.set = 1</p> 
     <p itemprop="description">throttle.max_peers.normal.set = 512</p> 
     <p itemprop="description">network.max_open_files.set = 1024</p> 
     <p itemprop="description">network.max_open_sockets.set = 1024</p> 
     <p itemprop="description">network.http.max_open.set = 512</p> 
     <p itemprop="description">network.send_buffer.size.set = 16M</p> 
     <p itemprop="description">network.receive_buffer.size.set = 16M</p> 
     <p itemprop="description">pieces.memory.max.set = 3500M</p> 
    </blockquote> 
    <p itemprop="description">pieces.memory.max.set 这个参数代表使用多少内存，我的是4G内存，所以我设置为3500M 。建议是你内存的80%～90%，文件读取如果都是在内存中进行的话，那么反之本地读写的次数就越少。所以硬盘IO速度也能相应的提升。大内存的机器就不要吝啬你的内存了。要物尽其用才行！</p> 
    <p itemprop="description"><strong>新增：</strong>（把下面这些参数复制进去，放到文本的最后）</p> 
    <blockquote> 
     <p itemprop="description">max_uploads = 512</p> 
     <p itemprop="description">pieces.preload.min_size.set = 262144</p> 
     <p itemprop="description">pieces.preload.min_rate.set = 5120</p> 
     <p itemprop="description">network.xmlrpc.size_limit.set = 4M</p> 
     <p itemprop="description">system.file_allocate.set = yes</p> 
    </blockquote> 
    <p itemprop="description">最后修改完毕后<strong>记得保存</strong>，它看起来应该像下面这张图一样。<br /></p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_37/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a68524b00be2237.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description"><strong>7、Putty输入命令： reboot</strong> &nbsp; （重启一下服务器，使得我们刚才所有的设置生效）</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_38/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/24/5a6839a6399cd1105.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">等服务器重启完毕，我们的基本优化工作已经完成了。现在就可以来测试一下种子的下载速度，找几个热种试试看吧。不出意外的话，速度应该能有1个明显的提升了。如果你还是对速度不满意。那么本人也尽力了。或许等我再好到新的方法，会再次更新这一篇文章。对了，下载工具也是会影响下载速度的噢，不同的工具写法以及算法都不一样。目前速度最快的应该是“Deluge”吧，“qBittorent”的Windows版我也试过，感觉速度也很暴力，不知道Linux下的表现如何。大家可以测试一下。</p> 
    <p itemprop="description"><a href="https://post.smzdm.com/p/aex7kv3/pic_39/" target="_blank"><img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://qnam.smzdm.com/201801/25/5a68c0de0c0379637.png_e600.jpg" title="" /></a></p> 
    <p itemprop="description">就在刚才我添加了1个新种子，可以看到下载速度已经彪到42mb/S了。在加上目前已有的上传带宽，宽带利用率已经达到了接近60MB/S的速度。而我的服务器最快也就只能跑个80MB/S 左右。相比起我一开始没有优化只有30MB/S的速度已经有了快一倍的提升。（不过最后还是有一点要说明一下，我目前只在自己的服务器上测试过。至于别的服务器有没有什么特别的讲究，我也不清楚，所以大家在看我的教程时，主要是做参考，然后贵在自己调试）</p> 
    <p itemprop="description">---------------------------------------------------------------------------------------------------</p> 
    <p itemprop="description">连续发了两篇的文章，教程写的还真是有点累人。不过总算把这2个月摸索的一点东西给贡献了出来，也算是PT精神吧。人人为我，我为人人。我的这台15欧的服务器还有5天到期，届时会测试下11欧的那一款，看看速度稳定性如何。毕竟我们要把彻底把“值”这个字给发挥出来才是上上策。</p> 
    <p itemprop="description">---------------------------------------------------------------------------------------------------</p> 
    <p itemprop="description">下一篇预告：</p> 
    <p itemprop="description">1、服务器开启直链下载（方便取回本地文件）</p> 
    <p itemprop="description">2、给服务器安装魔改BBR加速，增加TCP传输速度。（加快取回文件速度）</p> 
    <p itemprop="description">3、优化直链下载列表（使其更加美观，更加人性化、支持打包下载、文件搜索、支持简易的在线播放）</p> 
    <p itemprop="description">最后谢谢各位的观看，也感谢各位大佬们的打赏。<img alt="PT盒子服务器参数优化以及Rutorrent设置调整" src="https://res.smzdm.com/images/emotions/180.gif" class="face" />&nbsp;</p> 
   </div> 
   <input type="hidden" id="isDetail" /> 
   <input type="hidden" id="channelID" value="11" /> 
   <input type="hidden" id="articleID" value="654616" />      
   <div class="leftWrap"> 
    <div class="poster-wraper"> 
     <div itemprop="image" itemscope="" itemtype="https://schema.org/ImageObject" class="detailed_banner"> 
      <img src="https://qna.smzdm.com/201801/26/5a6af2c1ca16b6594.jpg_fo710.jpg" /> 
      <meta itemprop="url" content="https://qna.smzdm.com/201801/26/5a6af2c1ca16b6594.jpg_fo710.jpg" /> 
      <meta itemprop="width" content="710" /> 
      <meta itemprop="height" content="300" /> 
     </div> 
    </div> 
    <article> 
     <h1 itemprop="headline" class="item-name">家庭影音之路 篇三：给服务器开启HTTP下载，并高速取回“云上”文件</h1> 
     <div itemprop="description"> 
      <h2 id="cl_0">温馨提示：</h2> 
      <p itemprop="description">亲爱的值友们，大家好，很高兴大家能来看我发布的文章，<strong>今天这篇文章是“家庭影音之路”系列的第3篇</strong>。本文的主要内容是前两篇文章的进阶篇，“主要讲解如何给<a class="seo_link" href="https://www.smzdm.com/fenlei/fuwuqi/" target="_blank">服务器</a>开启HTTP直链下载并进行下载加速”。所以，各位亲们，如果你是第一次看到我的文章，<strong>我建议看大家可以从本系列的第一篇看起</strong>，本系列文章主要是以教学为主，所以文章大量的篇幅都是在教你怎么操作。我相信，如果你有这方面的需求，又想自己动手操作的。肯定能在文章中找到对你有用的信息。<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/177.gif" class="face" />&nbsp;（下面给大家放送前两篇文章的传送门）</p> 
      <p itemprop="description">第一篇 ：&nbsp;</p> 
      <p itemprop="description">（教你挑选1台线上服务器并安装下载工具）<br /></p> 
      <p itemprop="description">第二篇 ：&nbsp;</p> 
      <p itemprop="description">&nbsp; （教你如何优化服务器网络并给下载工具加速）<br /></p> 
      <h2 id="cl_1">本章介绍：</h2> 
      <p itemprop="description">鉴于前两篇文章教给了大家如何搭建线上服务器，以及如何给线上服务器优化网络参数。相信已经动手操作过的小伙伴们应该下了不少资源了。所以，<strong>本章将会重点讲解</strong><strong>“如何取回服务器上的文件”，</strong>毕竟我们利用服务器“高速”下载好的文件，不把它取回本地实在对不起自己花的“票票”呀<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/179.gif" class="face" />&nbsp;本章将会用到的工具有：Putty 、WinScp 、FLASHfxp&nbsp;<strong>（Putty和WinScp这两款软件在前两章有介绍如何使用，本章就不重复介绍了）</strong></p> 
      <h2 id="cl_2">本章目录：</h2> 
      <ol class=" list-paddingleft-2" style="list-style-type: decimal;"> 
       <li><p itemprop="description">利用“WinScp”工具，修改Nginx配置文件，使服务器支持“网页直链”下载。</p></li> 
       <li><p itemprop="description">利用“FTP”工具，取回我们在服务器上面下载好的文件。</p></li> 
       <li><p itemprop="description">优化“网页直链”目录，使其更加的美观、多功能、方便 （支持在线观影、在线搜索、打包下载）</p></li> 
       <li><p itemprop="description">安装“<a class="seo_link" href="https://pinpai.smzdm.com/2047/" target="_blank">谷歌</a>BBR”，让你“高速”取回服务器上下载好的文件。</p></li> 
      </ol> 
      <p itemprop="description">亲们可以根据自行选择观看教程内容（<strong>大章节会用“一”“二”“三”“四”中文数字标记</strong>，方便亲们最快的找到所需信息）。好的，废话不多说，下面就跟着作者一起来“实战”吧！</p> 
      <p itemprop="description">--------------------------------------------------------------------------------------------------</p> 
      <h2 id="cl_3">一、利用“WinScp”工具，修改Nginx配置文件，使服务器支持“网页直链”下载</h2> 
      <p itemprop="description">上一章我们优化过“Nginx”的配置文件并去掉了“网页不安全”的提示，大家还有印象吗？那么本节将会再次给“Nginx”的配置文件进行优化，并且增减几行参数，开启Http直链下载目录。（方便我们浏览并下载服务器上的文件）至于“WinScp”这个软件如何使用，大家可以参考第二篇文章，上面有详细的教学。本节就不在详细阐述了。<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/185.gif" class="face" />&nbsp;</p> 
      <p itemprop="description"><strong>1、“WinScp”工具-编辑文件：/etc/nginx/sites-enabled/default</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_2/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/26/5a6b0de0839907072.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">通过“WinScp”这个工具打开文件后，我们会看到上一篇设置好的参数。之前有跟着操作过的同学，这下应该轻车熟路了吧。下面我只需要复制几行参数进去，就OK了。没错，就是这么简单。因为参数我都给你写好啦，照葫芦画瓢即可！</p> 
      <p itemprop="description"><strong>2、把以下文本复制进去</strong><strong>然后保存！</strong></p> 
      <blockquote> 
       <p itemprop="description">server {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; listen 999;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; root /home/登录账号/rtorrent/download;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; index index.html index.php index.htm;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; client_max_body_size 40m;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;autoindex on;</p> 
       <p itemprop="description"><br /></p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; location / {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;client_max_body_size 40m;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;include /etc/nginx/conf.d/php;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;include /etc/nginx/conf.d/cache;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; }</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; location ~ /.ht {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; deny all;</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; }</p> 
       <p itemprop="description">}</p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_3/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b1049961851253.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">上面这些参数就是我们需要“复制进去”的配置文件了。这里有1个地方是需要修改的请大家注意！“输入账号”请改成你网页登录的账号（不知道网页登录账号？？&nbsp;那么前两章肯定没看）。修改好的同学大家可以对比上面这张图，这张图是我修改好的大家可以参考。只要让他们看起来一模一样就可以了（除了“登录账号”）</p> 
      <p itemprop="description"><strong>3.“Putty”工具-输入命令： &nbsp;service nginx restart</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_4/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2dbb09d3c553.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这一步的目的是告诉服务器，我们要重启Web服务端，你可以理解为刷新网页使其生效！至于“Putty”工具如何使用，前看第一章，第一章详细介绍了这个工具如何使用，上面有传送门，不懂的同学建议回顾一下。</p> 
      <p itemprop="description"><strong>4.通过浏览器访问下载目录</strong></p> 
      <p itemprop="description">通过上面对配置文件的修改操作，我们已经成功的开启目录浏览，并支持“简易”的文件下载了。下面我们<strong>只需要以“IP+端口号”的形式访问</strong>我们的服务器就能看到服务器上的文件了。至于什么是“IP+端口号”，还记得我们第二章讲解的内容吗？当时访问我们的“网页版下载工具”就是利用的IP+端口号。类似“http://12.12.12.12:666”这样，其中“666”就是端口号，“12.12.12.12”就是你服务器的IP地址，他们的分隔符是小写的冒号“:”最后结合即可。那么下载目录的端口是多少呢？&nbsp;答案：“999”</p> 
      <blockquote> 
       <h3>http://IP地址:端口号&nbsp;&nbsp; 例如：http://125.125.125.125:999&nbsp; &nbsp;（端口可自定义，http://&nbsp;没有S !&nbsp;）</h3> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_5/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b1882217393632.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">可以看到，我们已经成功的通过“IP+端口”的形式访问了我们的下载目录，就像上面这张图一样。会显示你下载好的所有文件！如果你成功的看到了上面这张图片显示的内容，那么就证明你就已经成功开启了Http的直链下载。这下就可以把服务器上的资源给通过浏览器给拖回本地了。<strong>需要注意的是，默认的下载目录只支持“直链”，你可以这样理解，它只能下载单个文件，比如一首歌，一张图片等等。不能把整个<a class="seo_link" href="https://www.smzdm.com/fenlei/wenjianjia/" target="_blank">文件夹</a>一起下载！</strong>不过值得一提的是在第一章教大家如何安装“Rutorrent”的同时，其实也默认给服务器上装上了“vsftpd”这个程序。简单点说，我们还可以通过FTP的模式，把服务器上的文件给下载回来。这样就可以把“文件夹”一并下载回来了！下面就开始教大家如何通过FTP，把服务器上的资源给取回。</p> 
      <h2 id="cl_4">二、利用“FTP”工具，取回我们在服务器上面下载好的文件</h2> 
      <p itemprop="description">这一节主要内容是通过&quot;FlashFXP&quot;这个工具连接上我们的服务器并把数据下载回来。至于这个&quot;FlashFXP&quot;工具大家可以百度自行下载，我就不提供链接了，相信能做到这一步的小伙伴，找个工具对你们来说“SO EASY”，当然本节是会教大家如何使用这个工具的，毕竟坑我已经挖好了，不能不跳呀是不是？<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/172.gif" class="face" />&nbsp;</p> 
      <p itemprop="description"><strong>1、Putty输入命令：cat /home/输入账号/rtinst.info</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_6/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b1d802552a5377.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>特别提醒：输入账号=网页账号&nbsp;</strong>我们通过Putty输入的这个命令，就是告诉服务器我们要查看 rtinst.info 这个文件内容。就像上面这张图一样，把这段命令粘贴进“Putty”输入端，然后回车就行了 （不知道Putty如何使用的同学，请回看第一章的内容，这里就不多做介绍啦）</p> 
      <p itemprop="description"><strong>2、查看FTP端口号并记录</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_7/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/26/5a6b1e3b3ea6e6337.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">我们之所以要查看这个文件，是因为这个文件记录着我们FTP的信息。里面有1个很重要的数据就是FTP的端口号，一会我们使用FTP工具的同时，会使用到这个端口号。所以你可以根据上面这张图的提示，把我们查看到的端口给记录下来。</p> 
      <p itemprop="description"><strong>3、下载并打开“FlashFXP”工具</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_8/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b1cab689f1891.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这个工具的界面还是挺简单的，是不是和 “WinScp”这个工具的界面差不多？嗯，殊途同归，都是文件传输工具，所以“长的”肯定像呀。好了，打开这个工具之后，我们就可以开始下一步了！</p> 
      <p itemprop="description"><strong>4、对着“FlashFXP”窗口，按“F8”调出连接界面</strong></p> 
      <p itemprop="description">当按了&quot;F8&quot;这个快捷键之后，就会跳出一个窗口，类似下面这张图。“FlashFxp”和“WinScp”这个软件使用上差不多类似。都是输入服务器的相关信息，然后连接进去。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_9/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b1fae150776968.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">连接类型：选择最后1个 “FTP using Explicit SSL （Auth TLS）”</p> 
      <p itemprop="description">地址：填写你服务器的IP地址</p> 
      <p itemprop="description">端口：填写我们上一步通过“Putty”这工具查看的端口号</p> 
      <p itemprop="description">用户名、密码：填写你的网页登录账号和密码</p> 
      <p itemprop="description">信息输入完毕之后，然后<strong>点击“连接”按钮</strong>，然后会跳出1个对话框，如下图所示，<strong>点击“接受并保存”</strong>！</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_10/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b206388212368.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">OK，不出意外，你已成功的连接进去了服务器。<strong>我们的下载目录在 “/rtorrent/download/”这个文件夹里面</strong>，你可以对着“FlashFXP”这个工具显示的服务器上文件夹，一层一层的进去。就像操作我们的电脑一样方便。如果你需要下载某些文件，可以参考一下下面这张图，只需要对着服务器上的文件右键点击传输就行了。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_11/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/26/5a6b212dac1f27129.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">---------------------------------------------------------------------------------------------------</p> 
      <p itemprop="description">至此，2个简单的取回本地的设置以及用法已经告诉了大家，但是本人还是建议大家只用“直链下载”就行。可能到这里有的同学会说，HTTP直链的目录那么丑，而且还不支持文件夹的下载，太不实用了。是的，默认情况下的“直链下载目录”确实比较丑，不符合现代人的审美，也不实用。但是！网上有一个不错的插件，可以美化它。并且让它的功能增加，比如“打包下载”。有需要的小伙伴可以接着往下看，如果你觉得这些功能已经够用了，那么可以跳过第三节的内容（不过作者还是建议大家看下第三节的内容，如果不实用或者没有意义的话，我也不会写出来告诉大家的<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/177.gif" class="face" />）<br /></p> 
      <h2 id="cl_5">三、优化“网页直链”目录，使其更加的美观、多功能、方便</h2> 
      <p itemprop="description"><strong>这一步不是必须的！</strong>改不改，优化不优化完全取决于各位小伙伴的心情，如果你光是跟着前面的教程做的很幸苦，那么可以稍微休息休息，因为这一步“非常麻烦”不是几个命令就能搞定的事情。<strong>但是我保证，跟着我的节奏做出来之后，效果绝对让大家满意！</strong></p> 
      <p itemprop="description">先做1个简单的介绍，我们“美化直链目录”需要用到“H5AI”这个PHP插件。当然不懂的小伙伴也没关系，我已经把开启这个插件最简单的方法给整理出来了！不过这里有1个前提，<strong>必须之前跟着教程开启了“HTTP直链下载目录”</strong>，如果你没有开启，那么本节的操作方法就对你无效了噢。（不知道如何开启“HTTP直链下载目录”的同学，请回看本章的第一节）</p> 
      <p itemprop="description"><strong>1、Putty输入命令：cd /home/输入账号/rtorrent/download</strong>&nbsp;&nbsp;</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_12/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b26de5e5963721.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这一步的意思是告诉服务器，我们要进入“/home/输入账号/rtorrent/download”这个文件夹，其中的“输入账号”就是你网页登录使用时的账号。当你输入完这个命令之后，就会发现“Putty”工具上你的输入光标前面的路径地址，变成了“root@xxx /home/输入账号/rtorrent/download”。<strong>如果没有看到这个提示，就证明你没有进入该文件夹噢！</strong>请检查你的输入，看看是否有误，因为本节能否操作成功，全看这个。非常重要！</p> 
      <p itemprop="description"><strong>2、putty输入命令：wget https://release.larsjung.de/h5ai/h5ai-0.29.0.zip</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_13/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b271ba9d901299.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这一步的命令是告诉服务器，我们要下载文件。至于文件下载到哪里了？很简单，“wget”这个命令在不指定文件夹的情况下，会默认下载到当前目录，所以我才会让大家在上一步先进入我们需要操作的文件夹的。</p> 
      <p itemprop="description"><strong>3、putty输入命令：unzip h5ai-0.29.0.zip &nbsp; &nbsp;</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_14/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b273ca93aa6455.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这个命令是告诉服务器，把我们刚才下好的文件解压至当前文件夹。当然如完毕之后，你会发现“putty”这工具上面提示了好多文件出来，其实这个就是告诉你服务器一共解压出来了什么文件。</p> 
      <p itemprop="description"><strong>4、putty输入命令：rm h5ai-0.29.0.zip</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_15/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2751bbac8466.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这个命令是告诉服务器，删除我们刚才下载的“压缩包”，因为我们已经通过命令把需要的文件解压出来了。所以刚才这个下载的压缩包已经没用了。当然你不删除也可以，不影响大局。只不过，删了之后更美观而已。</p> 
      <p itemprop="description">把上面4条命令执行完毕后，你可以通过WinScp工具查看你的“下载目录”，这时候你会发现下载目录中多了1个_h5ai的文件夹。这个文件夹就是我们刚才通过命令解压的文件夹了。<strong>有一点需要注意！以后这个文件夹都不可以删除，这是我们美化目录的核心文件！</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_16/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2a2e2f5c9512.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>5、WinScp修改文件：/etc/nginx/sites-enabled/default</strong></p> 
      <blockquote> 
       <h3>在“index index.html index.php index.htm”这些字符的后面加入 &nbsp;/_h5ai/public/index.php&nbsp;</h3> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_17/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2e456e1781347.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">还记得我们在本章第一节时候修改“Nginx”配置文件吗？没错，这次还是来修改这个文件，只不过很简单，只需要复制1个参数进去就行了。大家可以参考一下上面这张图，让他们看起来一模一样即可。有的小伙伴这个时候会问了，这个文件中 有2个配置啊，我应该复制到哪1个后面才对呢？ 我的答案是：2或者都复制。还有修改完毕后记得保存！</p> 
      <p itemprop="description"><strong>6.Purry输入命令： &nbsp;service nginx restart</strong><br /></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_18/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2dbb09d3c553.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">当修改成功之后，保存过后，我们只需要给服务器发送上面这段命令就行了，这一步骤的目的是告诉服务器重启网页端，使得我们刚才的保存配置生效，然后就大功告成了。当然还没有结束，我们往下看！</p> 
      <p itemprop="description"><strong>7.重新访问下载目录 &nbsp;（访问方法还是和之前一样 IP+端口）</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_19/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b2f5425aaa4380.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_20/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/26/5a6b301ae1791698.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这才符合现代人的审美，和一开始的目录相比，简直就是天壤之别啊。不要着急，默认的H5AI的配置还不能满足我们的需求，这么高大上的插件，功能远不止我们看上去的这么简单，下面将会教会大家优化H5AI，让它更加的实用、更加的完美。</p> 
      <p itemprop="description"><strong>8、WinScp编辑文件：/home/输入账号/rtorrent/download/_h5ai/private/conf/options.json</strong></p> 
      <p itemprop="description">这一步看似复杂，其实很简单，总的来说，就是根据我给你提供的配置文件信息，然后修改就行了。再简单点，就是3个步骤 “搜索”“对比”“复制”。大家慢慢跟着操作就可以了。切记不要心急哦～<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/171.gif" class="face" />&nbsp;</p> 
      <blockquote> 
       <p itemprop="description">&nbsp; &nbsp; &quot;download&quot;: {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;enabled&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;php-tar&quot;,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;packageName&quot;: null,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;alwaysVisible&quot;: false</p> 
       <p itemprop="description">&nbsp; &nbsp; },</p> 
       <p itemprop="description">-----------------------------------</p> 
       <p itemprop="description">&nbsp; &nbsp; &quot;info&quot;: {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;enabled&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;show&quot;: false,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;qrcode&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;qrFill&quot;: &quot;#999&quot;,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;qrBack&quot;: &quot;#fff&quot;</p> 
       <p itemprop="description">&nbsp; &nbsp; },</p> 
       <p itemprop="description">-----------------------------------</p> 
       <p itemprop="description">&nbsp; &nbsp; &quot;l10n&quot;: {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;enabled&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;lang&quot;: &quot;zh-cn&quot;,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;useBrowserLang&quot;: true</p> 
       <p itemprop="description">&nbsp; &nbsp; },</p> 
       <p itemprop="description">-----------------------------------</p> 
       <p itemprop="description">&nbsp; &nbsp; &quot;search&quot;: {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;enabled&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;advanced&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;debounceTime&quot;: 300,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;ignorecase&quot;: true</p> 
       <p itemprop="description">&nbsp; &nbsp; },</p> 
       <p itemprop="description">-----------------------------------</p> 
       <p itemprop="description">&nbsp; &nbsp; &quot;select&quot;: {</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;enabled&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;clickndrag&quot;: true,</p> 
       <p itemprop="description">&nbsp; &nbsp; &nbsp; &nbsp; &quot;checkboxes&quot;: true</p> 
       <p itemprop="description">&nbsp; &nbsp; },</p> 
      </blockquote> 
      <p itemprop="description">以上提供给大家的文件参数是我修改过的，大家对照着我修改的文件，搜索关键字，然后替换关键信息就行了。这里我打个比方。比如“download”这个参数值如何修改？ 首先“搜索”-》“download”，然后你会找到“download”这一行，然后对比我给你的配置，看看有哪些变化？ 比如我们发现默认配置上是 enabled: no &nbsp;而我给你提供的是&nbsp;enabled: yes ，那我们只需要 把 “no”这参数改成“yes”就行啦。 我相信大家如果之前跟着教程做到了这一步，处理下这个问题应该不难吧？ &nbsp;我已经尽量的让教程变的通俗易懂了，如果还是不明白我表达的是什么- -，我只能说，大佬们，我尽力了。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_21/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/26/5a6b4e861f4877692.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">当我们把配置文件修改好之后，刷新一下网页，就会发现“下载目录”的功能增加了，这个时候已经支持在线搜索以及打包下载等等非常实用的功能了。大家也可以自己摸索下，看看还有那些变化呢。</p> 
      <p itemprop="description">------------------------------------------------------------------------------------------------</p> 
      <h2 id="cl_6">四、安装“谷歌BBR”，让你“高速”取回服务器上下载好的文件</h2> 
      <p itemprop="description">和第三节一样，这一步也不是必须的！那么本节的主要目的是什么呢？很简单，就是为了让你能更快的下载服务器上的文件，之前的所有内容（包含本系列的第一篇、第二篇）都是在告诉大家如何用服务器下载。也教了大家如何取回服务器上的文件。但是，<strong>因为我们的服务器在国外，所以取回的速度是非常慢的！所以这里有必要优化下载速度！</strong>下如果你的网络非常好，或者人在国外的朋友可以跳过本节。下面先放上两张，优化前和优化后的速度对比图。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_22/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5f684fb488656.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><br /></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_23/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5f76c20ca4990.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">从上面2张对比图可以看出，我们的下载速度整整提高了30倍！因为BBR只是单边加速工具。能提高这么快已经很牛了，毕竟我们下载的数据可是绕了几个国家才到国内的。而且光靠1个算法就给我们提速了这么多，不得不佩服谷歌的人才辈出啊。但是，面对国内目前普遍的100MB的带宽，下载速度怎么也得10MB/S 才能让人满意。<strong>文章的最后会告诉大家如何才能“10MB/S”下载，当然有一个前提，就是你得根据本节的内容安装好“谷歌BBR”才可以！</strong></p> 
      <p itemprop="description">至于什么是BBR？有想了解的小伙伴自行百度搜索一下，简单点说，BBR是一种基于linux内核的一种TCP拥堵控制算法。<strong>你只需要知道“BBR”这个东西能加快你的下载速度就可以了</strong>。类似的工具还有ServerSpeeder。我测试过在windows系统的服务器上面ServerSpeeder效果比较牛。Linux系统还是用BBR吧。本节将会教大家如何开启“魔改版BBR加速”。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_24/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/27/5a6b5227471a52099.gif_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这里我们还是采用国内某大神写的一键脚本进行开启。这里有一点需要注意，<strong>因为脚本会更换Linux内核，所以存在一定的风险会升级失败！</strong>大家仔细考虑后在使用。如果你是租用“oneprovider”的服务器（也就是本系列第一篇文章推荐给大家的服务器），那么会有1个“坑”需要注意，因为他们家的部分机器使用的是Broadcom NetXtreme的<a class="seo_link" href="https://www.smzdm.com/fenlei/wangka/" target="_blank">网卡</a>，而升级后的linux内核默认不包含NetXtreme的驱动，所以会导致升级后服务器打不开！（本文也会教大家如何解决这个问题）</p> 
      <p itemprop="description"><strong>1、Putty输入命令：</strong></p> 
      <blockquote> 
       <p itemprop="description"><strong>wget -N --no-check-certificate &quot;https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh&quot; &amp;&amp; chmod +x tcp.sh &amp;&amp; ./tcp.sh</strong></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_25/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b554ef213f2846.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">输入这个命令，其实就是告诉服务器“下载并运行”我们的一键脚本，这个脚本是国内某大神编写的，我们直接使用即可。<strong>有一点需要注意，这个脚本只支持“Centos 6+/Debian 8+/Ubuntu 14+”这3类操作系统</strong>，如果你的操作系统不是这三种，那么即使运行了该脚本，也不会进行修改的。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_26/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b55beef4378275.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">当你运行过上面的命令后，紧接着就会出现“上图这个提示界面”，然后输入相应的数字即可进行相关的操作了。这里需要注意，<strong>如果你在“第二篇”文中根据教程优化了网络参数，那么请不要使用脚本自带的系统配置优化</strong>。会有冲突噢！说简单点也就是 数字 “7”就不要输入了！</p> 
      <p itemprop="description"><strong>2、putty输入命令：</strong><br /></p> 
      <blockquote> 
       <p itemprop="description"><strong>1</strong><br /></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_27/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b562e5dce16337.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">就像上面这样，我们输入1，然后回车之后，脚本就开始“自动升级”内核了！再此期间你就什么都不需要弄了，只管盯着屏幕即可。升级成功之后会有提示的！</p> 
      <p itemprop="description">因为是升级系统的内核，所以或多或少会存在一些问题，下面2个问题，是我经常遇到的，如果你也出现了相同的问题，那么请根据以下的教程进行。如果很顺利，没有出现下面提示的错误信息。OK，大吉大利，晚上吃鸡！</p> 
      <p itemprop="description"><strong>《问题1》</strong>如果你用的是Debian系统或者在升级内核的过程中出现了下面这张图的内容，请用<a class="seo_link" href="https://www.smzdm.com/fenlei/jianpan/" target="_blank">键盘</a>，按一下右方向键，把“红色”的光标移动到“NO”这个选项上，然后回车即可！<br /></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_28/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b56b330d2e2548.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>《问题2》</strong>如果你用的是第一篇文章中推荐的“oneprovider”服务器，或者在<strong>升级内核中出现了如下提示！结束后千万别重新启动</strong>，需要把网卡驱动装进去才行，不然服务器就失联了！也就意味着升级失败。切记，一定要仔细看。<br /></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_29/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5779075507425.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>（如果没有出现上面的提示，可以跳过这一步骤）</strong></p> 
      <p itemprop="description"><strong>《问题2》的解决方法：</strong><br /></p> 
      <p itemprop="description"><strong>输入命令：&nbsp;</strong></p> 
      <blockquote> 
       <p itemprop="description"><strong>n &nbsp;</strong></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_30/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b580844d005377.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">当你脚本运行到，问你是否要重启的时候，这时你需要输入“n”，也就是告诉服务器不重启！</p> 
      <p itemprop="description"><strong>输入命令：</strong></p> 
      <blockquote> 
       <p itemprop="description"><strong>&nbsp;mkdir -p /lib/firmware/bnx2/ &amp;&amp; cd /lib/firmware/bnx2/</strong></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_31/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5836c31dd1166.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">紧接着输入的命令，是告诉服务器在 特定目录创建1个名字为“bnx2”的文件夹并进入！</p> 
      <p itemprop="description"><strong>输入命令：</strong><br /></p> 
      <blockquote> 
       <p itemprop="description"><strong>wget https://github.com/cernekee/linux-firmware/raw/master/bnx2/bnx2-mips-09-6.2.1b.fw &amp;&amp; wget https://github.com/cernekee/linux-firmware/raw/master/bnx2/bnx2-mips-06-6.2.3.fw</strong></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_32/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b58b0f307f6073.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这一步的命令是下载2个“网卡驱动”文件到 我们刚才创建的文件夹里面。</p> 
      <p itemprop="description"><strong>输入命令：</strong></p> 
      <blockquote> 
       <p itemprop="description">cd &amp;&amp; reboot<br /></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_33/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b58e7636f23644.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这一步的命令是告诉服务器，我们要重启服务器了！然后服务器就开始重启了，不出意外的话一会服务器就能Ping通（至于怎么Ping 服务器，请看第一篇文章的教学内容），然后我们就可以继续操作了。</p> 
      <p itemprop="description">------------------------------------------------------------------------------------------------</p> 
      <p itemprop="description">如果你没出现上面的2个问题，那么在重启过服务器后，我们通过Putty工具登入服务器。然后继续进行操作！<strong><br /></strong></p> 
      <p itemprop="description"><strong>Putty输入命令：</strong><br /></p> 
      <blockquote> 
       <p itemprop="description"><strong>./tcp.sh</strong></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_34/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5a8b98f772458.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">这个时候我们就又一次进入了一件脚本，然后你会发现脚本已经提示，我们安装好了BBR加速内核，如下图所示。</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_35/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5ac83bfa57593.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>输入命令：</strong><br /></p> 
      <blockquote> 
       <p itemprop="description"><strong>4</strong><br /></p> 
      </blockquote> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_36/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://qnam.smzdm.com/201801/27/5a6b5af3622f93249.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">然后脚本就开始自动运行了，等待一会之后。就安装完成了。最后会出现如下提示。注意看图片上的标注，最后2个参数一定是1行1个！如果不是的话可以通过WinScp修改文件：/etc/sysctl.conf &nbsp;自行手动换行！（WinSC如果不会用，请看第一篇文章，之前都有教过的，提示了这么多次，相信聪明的小伙伴很快就能懂）</p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_37/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/27/5a6b5c20e322d9780.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">正如提示那样，我们已经成功的开启了魔改BBR加速。这里有一点需要说明一下，我们使用的是“魔改BBR”，之所以是这么有魔性的名字。因为这个BBR加速是某大神修改google原版BBR而来。就像名字一样，更加的魔性，更加的暴力。然而BBR对于Seedbox这类程序也是能起到加速效果的。<strong>简单点说“魔改BBR”对下载速度加速更好！</strong></p> 
      <p itemprop="description">-----------------------------------------------------------------------------------------------</p> 
      <p itemprop="description">文章结尾再给大家介绍一款<strong>http直链专用的下载工具 “internet download manager”</strong>，利用这个工具做到32线程同时下载。速度也能飚起来！这个工具大家自己百度一下，然后下并安装。下面只教大街如何设置这个工具。<br /></p> 
      <p itemprop="description"><strong>首先开启32线程：</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_38/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/27/5a6b62e7e73e88617.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description"><strong>然后我们下载看看吧！(还是同1个文件噢，之前加速后是400KB/S，现在直接到11M/S了！)</strong></p> 
      <p itemprop="description"><a href="https://post.smzdm.com/p/aw3vkwg/pic_39/" target="_blank"><img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://am.zdmimg.com/201801/27/5a6b63c4cbdbe1097.png_e600.jpg" title="" /></a></p> 
      <p itemprop="description">第三篇的文章就此结束了，感谢大家的观看。至于第四篇的内容，我脑海中有很多构思，但是还没有办法做一个系统的规划。以至于怎么写、写什么、成了现在困扰我的问题。这个系列是以“家庭影音之路”为主题，那么所有的东西都是围绕这个进行的。我在想是否可以介绍一些硬件相关的了。毕竟开了3章都是在教大家如何下载资源。相信有需要的同学应该能获得一些帮助。那么我们第四章再见。<img alt="给服务器开启HTTP下载，并高速取回“云上”文件" src="https://res.smzdm.com/images/emotions/184.gif" class="face" />&nbsp;</p> 
      <p itemprop="description"><br /></p> 
     </div> 
     <input type="hidden" id="isDetail" /> 
     <input type="hidden" id="channelID" value="11" /> 
     <input type="hidden" id="articleID" value="655850" /> 
    </article>
   </div>
  </article>
 </body>
</html>
