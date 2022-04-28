# 0_FineBI_Cross-market-stock-price-monitoring-and-analysis
2022/4/29 FineBI数据分析大赛-跨市场股价运行监测与分析
## 0 项目截图展示：
![跨市场股价运行监测与分析（盘中实时）](https://user-images.githubusercontent.com/78157334/165747699-bb9b7ef8-7a14-4402-b172-23b1ff360f51.jpg)
![跨市场股价运行监测与分析（个股详情）](https://user-images.githubusercontent.com/78157334/165747908-3187845f-a200-4de7-b5f2-7a7758480717.jpg)
![跨市场股价运行监测与分析（近期走势）](https://user-images.githubusercontent.com/78157334/165747926-2edb7b23-470a-469c-988b-c8a190b63f8f.jpg)

## 1 业务背景
近年来我国多层次股票市场加快发展，目前形成了上海、深圳、北京“三足鼎立”的三大股票市场，“股市是实体经济的晴雨表”，市场的平稳运行对金融、经济和资本市场稳定都具有十分重要的意义，防止股市大起大落、暴涨暴跌是监管部门最重要的日常工作职能之一。在日常的监管工作中，监管人员需要每天动态掌握股价的变化情况，以保持较高的市场敏锐性，以便在市场出现大涨或大跌时及时开展形势分析和研判.
## 2 业务痛点
1.日常工作中监管人员的时间有限，每天不可能花过多时间寻找数据来了解市场运行变化情况，迫切需要一目了然或者操作非常简单且很实用的数据监测分析工具。  
2.国内各金融资讯信息商均推出了各自的金融终端，汇集了各类数据信息，但主要以面向投资者用户为主，难以满足市场监管人员的个性化需求，在了解不同市场的运行情况时往往需要进入不同界面，不便于快速了解跨市场股价变化运行情况。
## 3.分析目标
1.对当日盘中股价进行实时监测：聚焦境内市场，实时动态展示A股市场（包括沪市、深市、京市）的股票价格总体变化情况；  
2.对当日盘中个股信息进行多维分析：满足监管人员在“盯盘”时对其感兴趣的个股进行灵活查询和分析，及时了解相关股票的量价变化情况。  
3.对近期市场股价运行走势进行分析：由于当前的股价变化很可能是近期趋势的延续，因此在监测分析当日实时股价变化的同时，还需对近期的市场历史走势进行分析。
## 4.数据集
1.数据主要来自东方财富Choice金融终端、聚宽（JoinQuant）量化交易平台  
2.初始数据情况如下表所示：
<img width="693" alt="image" src="https://user-images.githubusercontent.com/78157334/165751464-c3f997bf-02bf-48ed-8427-bd408e722c45.png">
## 5.可视化布局思路
1.第一个界面设计，用于盘中实时市场监测分析。按照数据分析的先后顺序，从上而下放置组件，上方用于对境内市场进行分析，下方用于观察境外市场。其中，重点对于境内市场，从上而下依次用于市场分析、行业分析和个股分析，层层细分。  
2.第二个界面设计，用于盘中实时个股监测分析。监管人员在“盯盘”时，可能需要对感兴趣的个股或某些特定类别的股票进行分析，因此需要专门提供用于个股分析的界面。对个股分析的维度众多，这里我们选取板块、行业、股价、市值、估值等5个常用的分析维度
3.第三个界面设计，用于近期走势情况分析。对近期走势进行分析，是从历史的角度对股票价格变化趋势及其原因进行的深入分析。具体而言，一方面，需要方便地对境内外主要股票市场的股价走势进行横向对比，便于监管人员分析了解总体情况；另一方面，需要对境内市场的股价走势原因进行结构性分析，包括行业板块和投资者资金行为两大因素。
