# Walmart
爬取沃尔玛网站指定产品的评论内容  
Crawl specified product reviews from Wal-Mart web site

##Platform and Version: 
* Python 3.5
* Windows 10 64bit

##Usage: python walmart [options]

##Options:
 * -h --help                 Show this on screen.
 * -v --version              Show version.
 * -l --link=<link>          Product review page link
 * -p --page=<page>          The number of pages that you want to scrap
 * -t --translate            Translate title and content via Youdao API
 * -f --filename=<filename>  Specify output file name

##Example:
  walmart -l https://www.walmart.com/reviews/product/47055697 -p 10 -t walmart.xlsx

##Remark:
  1. Link can be multiple and just need to be separated with ';'  
  e.g. python walmart.py -l [linka];[linkb]

  2. Use -t --translate option carefully thus Youdao translate API can only use 1000 times / Hour.  
  It will translate fail when the query limit is reached.
