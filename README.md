# springboot004网页时装购物系统

## 简介

本代码仅供学习参考使用

加QQ(**3055269939**)免费获取项目和论文

## 主要内容

## 数据表

将数据库概念设计的E-R图转换为关系数据库。在关系数据库中，数据关系由数据表组成，但是表的结构表现在表的字段上。

表名：shangpinfenlei

功能：商品分类

| 字段名称       | 类型      | 长度 | 字段说明 | 主键 | 默认值            |
| -------------- | --------- | ---- | -------- | ---- | ----------------- |
| id             | bigint    |      | 主键     | 主键 |                   |
| addtime        | timestamp |      | 创建时间 |      | CURRENT_TIMESTAMP |
| shangpinfenlei | bigint    |      | 商品分类 |      |                   |

 

 

表名：shangpinpingjia

功能：商品评价

| 字段名称          | 类型      | 长度 | 字段说明 | 主键 | 默认值            |
| ----------------- | --------- | ---- | -------- | ---- | ----------------- |
| id                | bigint    |      | 主键     | 主键 |                   |
| addtime           | varchar   | 100  | 创建时间 |      |                   |
| dingdanbianhao    | varchar   | 100  | 订单编号 |      |                   |
| shangpinmingcheng | varchar   | 100  | 商品名称 |      | 管理员            |
| shangpinfenlei    | timestamp |      | 商品分类 |      | CURRENT_TIMESTAMP |
| pinpai            | varchar   | 100  | 品牌     |      |                   |
| yanse             | varchar   | 100  | 颜色     |      |                   |
| chima             | varchar   | 100  | 尺码     |      |                   |
| pingfen           | varchar   | 100  | 评分     |      |                   |
| pingjianeirong    | varchar   | 100  | 评价内容 |      |                   |
| tianjiatupian     | varchar   | 100  | 添加图片 |      |                   |
| pingjiariqi       | varchar   | 100  | 评价日期 |      |                   |
| yonghuming        | varchar   | 100  | 用户名   |      |                   |
| lianxidianhua     | varchar   | 100  | 联系电话 |      |                   |
| sfsh              | varchar   | 100  | 是否审核 |      |                   |
| shhf              | varchar   | 100  | 审核回复 |      |                   |

 

 

表名：shangpinxinxi

功能：商品信息

| 字段名称          | 类型      | 长度 | 字段说明 | 主键 | 默认值            |
| ----------------- | --------- | ---- | -------- | ---- | ----------------- |
| id                | bigint    |      | 主键     | 主键 |                   |
| addtime           | timestamp |      | 创建时间 |      | CURRENT_TIMESTAMP |
| shangpinmingcheng | varchar   | 200  | 商品名称 |      | fuzhuangxinxi     |
| shangpinfenlei    | bigint    |      | 商品分类 |      |                   |
| tupian            | bigint    |      | 图片     |      |                   |
| biaoqian          | varchar   | 200  | 标签     |      |                   |
| pinpai            | varchar   | 200  | 品牌     |      |                   |
| yanse             | int       |      | 颜色     |      |                   |
| chima             | float     |      | 尺码     |      |                   |
| shangpinxiangqing | float     |      | 商品详情 |      |                   |

 

 

表名：yanse

功能：颜色

| 字段名称 | 类型    | 长度 | 字段说明 | 主键 | 默认值 |
| -------- | ------- | ---- | -------- | ---- | ------ |
| id       | bigint  |      | 主键     | 主键 |        |
| addtime  | bigint  |      | 创建时间 |      |        |
| yanse    | varchar | 100  | 颜色     |      |        |

 

表名：yonghu

功能：用户

| 字段名称      | 类型      | 长度 | 字段说明 | 主键 | 默认值            |
| ------------- | --------- | ---- | -------- | ---- | ----------------- |
| id            | bigint    |      | 主键     | 主键 |                   |
| addtime       | timestamp |      | 创建时间 |      | CURRENT_TIMESTAMP |
| yonghuming    | varchar   | 200  | 用户号   |      | fuzhuangxinxi     |
| mima          | bigint    |      | 密码     |      |                   |
| xingming      | bigint    |      | 姓名     |      |                   |
| touxiang      | varchar   | 200  | 头像     |      |                   |
| xingbie       | varchar   | 200  | 性别     |      |                   |
| lianxidianhua | int       |      | 联系电话 |      |                   |