# soccerbet
一个研究足球彩票购买策略的小项目

#数据源
各博彩公司的赔率数据来自于500.com，在运行程序后，从500.com实时抓取近期比赛数据，以及各比赛的赔率数据。由于500.com对于国外博彩公司的数据有延迟，所以在实际购买时还应该参照国外博彩公司官方网站公布的实时赔率。

#博彩策略
该项目采取的博彩策略是利用不同博彩公司的赔率差，通过建立一个购买彩票的portfolio，获得盈利的彩票组合。

#程序入口
请使用python执行项目中的main.py
即在安装好python环境，确保接入互联网，执行 python main.py

#程序输出
程序输出，程序会输出每场比赛的比赛信息，盈利百分比，以及应购买的彩票组合。
例子：
        642471                                              //比赛代号
        http://odds.500.com/fenxi/ouzhi-642471.shtml        //比赛信息页面
        match name:	17亚冠杯分组赛                            //比赛名称
        match members:	西悉尼漫步者 VS 浦和红钻               //交战双方
        match time:	比赛时间2017-02-21 16:00                 //比赛时间
        profit:	109.88                                      //按照下面的比例购买彩票，能够获得的收益109.88%，即盈利9.88%
        win:	168 Pinnbet	4.2	27                          //从Pinnbet下注 27%的资金押胜
        draw:	168 Pinnbet	3.5	32                          //从Pinnbet下注 32%的资金押平
        lose:	26 Leon	2.68	41                          //从Leon下注 41%的资金押负