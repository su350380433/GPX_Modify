# GPX_Modify
手机定位修改,GPX设置,手机轨迹设置吗，轨迹从行者导出（http://www.imxingzhe.com/lushu/536942/）

# 注意
-  行者导出导出的轨迹要替换标签 
```
<trkpt> => <wpt>
```


- 把<wpt>集合复制下，copy到下面的标签内

```
<?xml version="1.0" encoding="UTF-8" ?>
<gpx
    version="1.0"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns="http://www.topografix.com/GPX/1/0"
    xsi:schemaLocation="http://www.topografix.com/GPX/1/0 http://www.topografix.com/GPX/1/0/gpx.xsd">
    
    
  
    
</gpx>
```

例子

```
<?xml version="1.0" encoding="UTF-8" ?>
<gpx
    version="1.0"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns="http://www.topografix.com/GPX/1/0"
    xsi:schemaLocation="http://www.topografix.com/GPX/1/0 http://www.topografix.com/GPX/1/0/gpx.xsd">
    
     <wpt lat="24.489985" lon="118.143">
        <time>2019-04-26T12:00:00Z</time>
    </wpt>
    
    <wpt lat="24.489976" lon="118.143069">
        <time>2019-04-26T09:47:03Z</time>
    </wpt>
    
    <wpt lat="24.48987" lon="118.14308">
        <time>2019-04-26T09:47:6Z</time>
    </wpt>
    
  
    
</gpx>
```


如有备注：
- 格式如下，直接复制到头部

```
  <name>厦门北到中山路步行街</name>
    <desc>行者骑行软件</desc>
    <author>行者骑行软件</author>
    <url>http://www.imxingzhe.com</url>
    <urlname>行者骑行软件</urlname>
    <time>2014-10-24T16:32:13Z</time>
    <keywords>行者骑行软件</keywords>
    <distance>25.807</distance>
```
例子如


```

<?xml version="1.0" encoding="UTF-8" ?>
<gpx
    version="1.0"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns="http://www.topografix.com/GPX/1/0"
    xsi:schemaLocation="http://www.topografix.com/GPX/1/0 http://www.topografix.com/GPX/1/0/gpx.xsd">
    
    
    <name>厦门北到中山路步行街</name>
    <desc>行者骑行软件</desc>
    <author>行者骑行软件</author>
    <url>http://www.imxingzhe.com</url>
    <urlname>行者骑行软件</urlname>
    <time>2014-10-24T16:32:13Z</time>
    <keywords>行者骑行软件</keywords>
    <distance>25.807</distance>
    
    
    
     <wpt lat="24.489985" lon="118.143">
        <time>2019-04-26T12:00:00Z</time>
    </wpt>
    
    <wpt lat="24.489976" lon="118.143069">
        <time>2019-04-26T09:47:03Z</time>
    </wpt>
    
    <wpt lat="24.48987" lon="118.14308">
        <time>2019-04-26T09:47:6Z</time>
    </wpt>
    
  
    
</gpx>

