# 一、以爬取内容建立商业模式的公司 #

1. [星图数据](http://www.syntun.com.cn)：电商商品

	搜索全网所有目标商品的相关信息，比如售价、销售量、客户评价以及同类产品的销量情况，并按照自己独特的算法来进行整理、归纳并以可视化的报告呈现给用户，并且整个过程可以随时进行，获得近乎实时的统计结果，帮助企业主随时调整经营策略、迅速应对市场变化，以获得最大化的利润。并且基于云端技术，数据结果可以跨平台显示，客户可以随时随地获得数据分析结果。
	
1. [IT桔子](https://www.itjuzi.com)：企业信息

	- 一类是技术抓取，包括主要新闻媒体、应用商店等，目前大概30%比例
	- 一类是用户UGC贡献，目前大概30%比例
	- 一类是合作伙伴数据渠道，比如和一些招聘网站、开发者社区建立联系，	定期获取；还包括来自于投资机构的数据，尤其是在投资事件的信息获取上，大概占比也有30%
	- 另外10%则来自于 IT桔子的成员作为互联网创业和投资爱好者，主动去发现及个人人脉积累了~~
	
1. [Everstring](http://www.everstring.com)：企业信息

1. [GuruDigger](https://gurudigger.com)：个人信息

	是一个面向互联网工程师和创业者的求职招聘社区。这个社区所能解决的需求有二：一是通过爬取用户在互联网上留下的“脚印”分析其职场基因及技术能力；二是分析用户与每一支创业团队的匹配度，来帮助用户找到最适合的团队。
	


# 二、爬取内容的应用 #

1. **双语、多语资料：机器翻译语料库**


	我们的爬取步骤大概是：
 
	1. 对当前网页进行简易判断，如果有双语嫌疑，则收录整理出来双语的正文；如果没有，弃用；
	2. 将正文内容进行详细判断，确定是双语文本，则进行段落对齐和句子对齐，整理到语料库；如果没有，弃用；
	3. 对当前网页的所有链接网页，重复步骤 1
	
	有详细介绍的我们申请的专利在这里：http://www.soopat.com/Patent/201210442487
	
	参考链接：https://www.zhihu.com/question/27621722/answer/48658220


1. **社交数据：情绪地图**
	
	@Emily L 提到了著名的根据情绪预测股市的论文：http://battleofthequants.net/wp-content/uploads/2013/03/2010-10-15_JOCS_Twitter_Mood.pdf 。
	
	其实我们也仿照做了国内的，不过没有预测，只是监测目前微博上大家的情绪，也是极有趣的。我们把情绪类型分为“喜悦”“愤怒”“悲伤”“恐惧”“惊奇”，并且对能体现情绪的词语进行权重的标记，从而给每天每个省份都计算出一个情绪指数。
	
	参考链接：https://www.zhihu.com/question/27621722/answer/48658220
	
1. **社交数据：饮食地图**
	
	我们抽取出所有美食相关词语，然后基于大家提到的美食次数，做了这么一份饮食地图。你可以查看不同省份、不同性别的用户、不同的时间段对不同类别食物的关注程度。
	
	参考链接：https://www.zhihu.com/question/27621722/answer/48658220
	
	访问地址：[微博用户饮食习惯分析](http://ys.8wss.com)

	
1. **交通数据：机场实时流量**
	
	![image](https://pic3.zhimg.com/adbee8589f03b1f4edd58e6c80a82fe6_b.jpg)

1. **交通数据：热点城市火车票情况**
![image](https://pic1.zhimg.com/47e2545e510ccce3d6a31827f1755c34_b.jpg)

1. **招聘数据：各种热门公司招聘中的职位数及月薪分布**
![image](https://pic3.zhimg.com/8aa8fc1babe66f6a89e603a9ed7f60aa_b.jpg)

1. **零售数据：某公司的门店变化情况**
![image](https://pic2.zhimg.com/cb19bace7864b680b325203ebe5ce71d_b.jpg)

1. **金融数据：对某一类金融产品的检测和跟踪**
![image](https://pic2.zhimg.com/49d24f9303436a786074734e23d1a3f9_b.jpg)

1. **汽车数据：对某车型用户数变化情况的跟踪**
![image](https://pic3.zhimg.com/9c0eb28f3b5321578a9efa2cea7d49a2_b.jpg)

1. **对某个App的下载量跟踪**
![image](https://pic1.zhimg.com/ace11806119acbe204b9193dfce2c378_b.jpg)

	参考链接：https://www.zhihu.com/question/27621722/answer/51806082
	
	

# 可供爬取的数据资源 #

## 生活服务－API ##

1. [APIX](http://www.apix.cn)
	
	* 	手机话费充值
	* 	天气查询
	* 	快递查询
	* 	健康食谱
	* 	查医院
	* 	水电媒缴费
	* 	电影大全
	* 	谜语、歇后语、脑筋急转弯
	* 	音乐搜索
	* 	健康知识
	* 	百度糯米、团购等信息
	* 	彩票开奖
	
类似还有：
	
1.	[聚合数据](https://www.juhe.cn)
	
1. 	[API Store](http://apistore.baidu.com)

1.	[91cha.com](http://www.91cha.com)

## 金融数据－API ##

### 股票 ###
	
1. [Tushare](http://tushare.org/fundamental.html#id4)：财经数据接口包
	
	国内好心人做的开源财经数据接口，这里几乎可以获取到A股的所有信息了，还包括一些经济数据。重点是他不仅免费，还提供了一个Python库tushare。
	
		pip install tushare
		import tushare as ts
	
	这样一来你便可以通过这个库方便地获取大量A股信息了。	
		
1. 新浪财经：	最多人用的就是新浪财经了，因为它是免费的，并且使用起来也不难。以下是网上找的教程：
	[获取历史和实时股票数据接口](http://www.cnblogs.com/seacryfly/articles/stock.html)
	
1. [东方财富网](http://data.eastmoney.com/xuangu/#Yz1beWxubDAxKDF8MC4wNSldfHM9eWxubDAxKDF8MC4wNSl8c3Q9LTE=)：网站提供了大量信息，也是基本面投资者的好去处。可以查看财务指标或者根据指标选股，有相对应的API。
	
1. [中财网](http://data.cfi.cn/cfidata.aspx)：	提供各种产品的数据
			
### 大宗商品 ###
	
1. [黄金头条](http://www.goldtoutiao.com)：大宗商品行情，包括技术分析方面。
	
2. [Investing](http://www.investing.com)：
	
### 美股等综合类 ###
	
1. [Wind](http://www.wind.com.cn)：很多机构用的都是这里的数据，当然普通个人是拿不到的，可以向财经院校学生免费提供。
	
1. [Xignite](http://www.xignite.com)：Market Data Feed and API

	外国网站，提供了大量数据，付费。有试用期。
	
1. [Quandl](https://www.quandl.com)：Quandl Financial and Economic Data
	
	部分免费，自带Python库
		
		pip install Quandl
		
	[96 Stocks APIs](http://www.programmableweb.com/news/96-stocks-apis-bloomberg-nasdaq-and-etrade/2013/05/22)：Bloomberg, NASDAQ and E*TRADE
	外国网站整合的96个股票API合集
	
	[雅虎财经](http://finance.yahoo.com)

## 其他－非API ##
	
1. **电商数据：比价打折**
	
	白菜网、超值分享汇、发现值得买、惠惠购物、今日聚超值、留住你、买手党、没得比、慢慢买、牛杂网、买个便宜货、什么值得买、天上掉馅饼、一分网、折800值得买、值值值等网站的折扣信息。

	这些网站都是提供的一些及时的、性价比较高的商品，很多时候要一个一个网站的看（重度用户），很容易就会错过一些很划算的商品。
	
2. **图片**

	如贴吧、知乎、Tumblr等。
	
3. **影评、电影资讯、图书等** 

	如豆瓣电影、时光网等。
