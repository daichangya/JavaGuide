# java面试指南

https://daichangya.github.io/JavaGuide/

## 微信公众号

扫码关注微信公众号，Java码界探秘。
![Java码界探秘](http://images.zthinker.com/qrcode_for_gh_1e2587cc42b1_258_1587996055777.jpg)

[https://zthinker.com/](https://zthinker.com/)


## 查询算法

- hash
- 数组
- 平衡树
- 跳表
- 字典树
- 倒排索引
- bitmap
- Bloom filter
![image](http://ww1.sinaimg.cn/mw600/693f0847jw1dnwuigpmxvj.jpg)

#### Elasticsearch

- 字典树 -> 倒排索引
- 多字段查询 bitmap

[参考链接](https://zthinker.com/archives/elasticsearch%E6%9F%A5%E8%AF%A2%E9%80%9F%E5%BA%A6%E4%B8%BA%E4%BB%80%E4%B9%88%E8%BF%99%E4%B9%88%E5%BF%AB "参考链接")

## 隔离级别

事务a 事务b

- b写未提交
- b写已提交
- a读一致
- ab串行化

![隔离级别](https://user-gold-cdn.xitu.io/2019/4/11/16a0d183bbd062be)

## 索引
#### B+ 树
块大小，树高度。
数据只存储在叶子节点
![image](http://blog.codinglabs.org/uploads/pictures/theory-of-mysql-index/10.png)

## 死锁
两个事物 相互等待

```
begin;
select * from table where id=1 for update;
update table set name=99 where id=2;

begin;
select * from table where id=2 for update;
update table set name=99 where id=1;
```

## 缓存

缓存a 数据库b

- 先a后b
- 先b后a
- ab一个事务

## 排序算法

[算法对比](/JavaGuide/算法/算法对比.md)
