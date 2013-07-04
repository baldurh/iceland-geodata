Iceland-geodata
===============

A collection of geographical data for Iceland in GeoJSON and TopoJSON format.  
A special thanks to **[Sævar Öfjörð Magnússon](https://github.com/saevarom)** for helping me getting started!  

Regions
-------

![Iceland regions](http://i.imgur.com/vycNgYe.png)

1 - 279,487 vertices (not simplified) GeoJSON - 12,567 KB / TopoJSON - 1,190 KB  
10 - 100,455 vertices (simplified with tolerance 10) GeoJSON - 4,548 KB / TopoJSON - 668 KB  
100 - 12,441 vertices (simplified with tolerance 100) GeoJSON - 564 KB / TopoJSON - 102 KB  
1000 - 1,150 vertices (simplified with tolerance 1000) GeoJSON - 54 KB / TopoJSON - 12KB  

Country
-------

1 - 266,651 vertices  
10 - 97,425 vertices  
100 - 11,685 vertices  
1000 - 962 vertices   

Points
------

###Towns


Tips
----

Combining GeoJSON files to a single TopoJSON file:  
```
topojson \
-p \
-o iceland_with_towns.topo.geojson \
iceland.geojson \
towns.geojson \
```  
will make a new file `iceland_with_towns.topo.json` with two objects, `iceland` and `towns`.

[Let’s Make a Map](http://bost.ocks.org/mike/map/) - A useful article for getting started with maps in D3.js

**Adding boundaries to a map will most likely only work for the most simplified data.** This is because the junctions
between polygons must be manually corrected after simplification to match perfectly. However, it is possible to
draw outlines for all polygons (lines around whole polygons instead lines between two different polygons only).

---

All geographical data derived from free data from [National Land Survey of Iceland (NLSI)](http://www.lmi.is/en/)  
[NLSI terms](http://www.lmi.is/en/stafraen-gogn/skilmalar-og-gjaldskra/)  

**Abstract**  
> **3. Copyrights**  
> The Republic of Iceland is the owner of all copyrights acquired by the NLSI. The 
NLSI defends the interests of the Republic of Iceland regarding the copyright and 
right of use of all materials it has acquired, processed or published regarding survey, 
maps or photos of Iceland. All other matters regarding copyright are covered by the 
Copyright Act, No. 73/1972 with subsequent amendments.  
> **4. User Rights**  
> Everyone is free to disseminate data originating from the NLSI for their own use and to
use when making their own material.  
> **6. Issuance and Publishing Licences**  
> Anyone who intends to distribute, display, publish or reprint material that is copyright 
under the Republic of Iceland from the NLSI shall apply for the issuance and 
publication to NLSI. The same applies to the use of derived materials based on 
material from NLSI. The application must include details of where it is planned to 
publish the material. As a confirmation of the application the NLSI grants the user a 
numbered publishing license.  

---
© Landmælingar Íslands V201307003