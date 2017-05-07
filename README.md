<html>
<head>
    <title></title>
	 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
	 
         <meta name="viewport" content="width=device-width, initial-scale=1" />
<style type="text/css">
</style>


<script src="https://s11.cnzz.com/z_stat.php?id=1261390656&web_id=1261390656" language="JavaScript"></script>

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function()
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o)
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');
  ga('create', 'UA-92667320-1', 'auto');
  ga('send', 'pageview';
</script>


<script>
var _hmt = _hmt || [];
(function() {
  var hm = document.createElement("script");
  hm.src = "https://hm.baidu.com/hm.js?d21dd59855971c0bbeecae6d553edd66";
  var s = document.getElementsByTagName("script")[0]; 
  s.parentNode.insertBefore(hm, s);
})();
</script>

</head><
     <body bgcolor="#FFFFFF" link='#FF8080' vlink='#FF8080' alink='#FFFF00'> 
     <h2><font color='#CC6600'>常用</font> </h2>
     <a href="https://www.zhihu.com/question/21637013">如何成为有趣的人</a>&nbsp;&nbsp;&nbsp;
     <a href="http://www.bilibili.com/video/av5274541/index_4.html">1993~2011国际大专辩论赛</a>&nbsp;&nbsp;&nbsp;
     <a href="https://www.zhihu.com/search?type=content&sort=upvote&q=%E5%BC%BA%E5%8A%BF%E7%9A%84%E4%BA%BA">如何与强势的人相处</a>&nbsp;&nbsp;&nbsp;
     <a href="http://byr.wiki">北邮人</a>&nbsp;&nbsp;&nbsp;
     <a href="http://www.jiaowu580.com/">教务处</a>&nbsp;&nbsp;&nbsp;
     <a href="https://mail.qq.com/cgi-bin/frame_html?sid=aR8oxHg4KJq8WjJn&r=5368bba12c619c6e25d19abb7c5a979c/">邮箱</a>&nbsp;&nbsp;&nbsp;
     <a href="http://mooc.study.163.com/learn/PKU-1000003003?tid=1000003009#/learn/content?type=detail&id=1000024001">唐大仕C#</a>&nbsp;&nbsp;&nbsp;
     <a href="https://msdn.microsoft.com/zh-cn/library/618ayhy6(v=vs.100).aspx">C#参考-MSDN</a>&nbsp;&nbsp;&nbsp;
     
     
     
     <h2><font color='#CC6600'>工具</font></h2>
     <a href="http://so.baiduyun.me/">网盘搜索</a>&nbsp;&nbsp;&nbsp;
     <a href="http://pan.glgoo.com/">Glgoo</a>&nbsp;&nbsp;&nbsp;
     <a href="http://www.dodoca.com/">点点客</a>&nbsp;&nbsp;&nbsp;
     <a href="http://mi.jd.com/home.html">蜜享</a>&nbsp;&nbsp;&nbsp;
     
     
     
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
        <meta http-equiv="Access-Control-Allow-Origin" content="*"/>
        <title>GlobeLand30</title>
  
        <script type="text/javascript" src="OpenLayers.js"></script>
        
        


    </head>
    <body>
    	
    	<div style="width:100%; height:100%; position:absolute;">
			<div id="MainMap" style="width:100%;height:100%; float:left;"></div>
        </div>
        
        <script type="text/javascript">
		
		   var map = new OpenLayers.Map({
				div: "map",
				projection: "EPSG:900913"
			});
			
		   var Coverage2010_743 = new OpenLayers.Layer.WMS("Landsat imagery 743 in 2010",
				"http://218.244.250.80:8080/erdas-apollo/coverage/IMAGE2010",
				{
					layers: 'ImageAfrica2010_743_0,ImageAsia2010_743_0,ImageNorthAmerica2010_743_0,ImageSouthAmerica2010_743_0,ImageEurope2010_743_0,ImageAustralia2010_743_0',
					format:"image/png",
					transparent: true
				},
				{ displayInLayerSwitcher: true, 
					visibility: false,
					isBaseLayer: true,
					isditu: true
				}
			);
			
		   
			var options = {
				div: "MainMap",
				projection: new OpenLayers.Projection("EPSG:900913")
				};
			map1 = new OpenLayers.Map(options);
	  
			map1.addLayers([Coverage2010_743]);
			//定位  
			map1.setCenter(new OpenLayers.LonLat(126.58,72.8).transform('EPSG:4326', 'EPSG:900913'), 8);
  
        </script>
        
        
        
    </body>
</html>
