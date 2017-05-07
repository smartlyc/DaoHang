
     
     
     
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
