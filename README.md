Iceland-geodata
===============

##Regions

![Iceland regions](http://i.imgur.com/vycNgYe.png)


1 - 279,487 vertices (not simplified) geojson - 12,567 KB / topojson - 1,190 KB <br> 
10 - 100,455 vertices (simplified with tolerance 10) geojson - 4,548 KB / topojson - 668 KB <br>
100 - 12,441 vertices (simplified with tolerance 100) geojson - 564 KB / topojson - 102 KB <br>
1000 - 1,150 vertices (simplified with tolerance 1000) geojson - 54 KB / topojson - 12KB <br>

##Country

1 - 26,6651 vertices <br> 
10 - 97,425 vertices <br> 
100 - 11,685 vertices <br> 
1000 - 962 vertices <br> 

##Points

###Towns


##Tips

Combining GeoJSON files to a single TopoJSON file: <br>
```
topojson
-p
-o iceland_with_towns.topo.json
iceland.json
towns.json
```  
will make a new file `iceland_with_towns.topo.json` with two objects, `iceland` and `towns`.


[Let’s Make a Map](http://bost.ocks.org/mike/map/) - A useful article for getting started with maps in D3.js

All geographical data derived from free data from [National Land Survey of Iceland (NLSI)](http://www.lmi.is/en/) <br>
[NLSI terms](http://www.lmi.is/en/stafraen-gogn/skilmalar-og-gjaldskra/)

