=== Plugin Name ===
Contributors: reage
Donate link: https://me.alipay.com/reage
Tags: SEO, segment, Chinese, SEO优化
Requires at least: 3.0.1
Tested up to: 3.5
Stable tag: 1.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

ReaSEO是一款基于云端分词的自动SEO工具，它能够帮您确定keywords项和description项，减轻您在SEO优化上的负担。

== Description ==

通过分析*搜狐和网易两家门户的新闻页面（分别抓取了451项、326项），我们发现了页面Title与KeyWords以及Title+Content与Description之间的关系：
KeyWords一般为Title中出现的名词、人名、机构团体名、地名(名处词专指：“中国”)、处所词(取英语space的第1个字母。“东部”)、及物动词(取英语动词verb的第一个字母。)、不及物谓词(谓宾结构“剃头”)、状态词(不及物动词,v-o、sp之外的不及物动词)。在新浪SAE提供的分词服务中，这些类别的词对应的分类如下：95、96、99、1021、130、131、170、171、180（130、131都对应处所词）。
在字符数不超过150的前提下，Description为正文的第一段（抽样中部分优秀WordPress站点的选择）；若字符数超标，则Description为文章的标题（搜狐新闻吻合率100%）。
*分析指基于新浪爱问API的中文分词及词性标注。

== Installation ==

1. Upload `reaseo.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= 我需要再额外添加什么调用代码吗？ =

不需要，ReaSEO hook了wp_head，会在页面载入时自动加上keywords和description

== Changelog ==

= 1.0 =
* 去掉了基于云的分词服务，改为实验的标题正文对照分词方法
* 去除了KeyWords末端的空格