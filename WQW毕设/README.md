### 进度
1. 已经成功爬取携程的排名前200景点（爬虫.py）
   * 景点名称
   * 景点对应的url
   * 热度
   * 评分
   * 评论数
2. 可以在对应景点的url里面翻页（css爬取.py）
3. 爬取对应景点url里面评论信息
   * 用户名
   * 评分
   * 评论时间
   * IP所属地
   * 点赞数
4. 通过读取之前的.xlsx文件来爬取每个景点的信息并且保存

5. 采用bert预训练模型来对景点介绍，用户评论进行embedding，用于下游任务
* 将所有景点的介绍放入bert，然后进行聚类，将他们分为不同的类型
* 结合用户评论来进行更深入的情感分析
现在先爬取200个景点的介绍，将他们保存
* 在文件夹bert中：爬取景点介绍.py，爬取了200个景点的介绍，但是有一些介绍为空，明天排查