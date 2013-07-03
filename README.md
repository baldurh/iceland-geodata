Iceland-geodata
===============

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
-o iceland_with_towns.topo.json \
iceland.json \
towns.json \
```  
will make a new file `iceland_with_towns.topo.json` with two objects, `iceland` and `towns`.


[Let’s Make a Map](http://bost.ocks.org/mike/map/) - A useful article for getting started with maps in D3.js

---

All geographical data derived from free data from [National Land Survey of Iceland (NLSI)](http://www.lmi.is/en/)  
[NLSI terms](http://www.lmi.is/en/stafraen-gogn/skilmalar-og-gjaldskra/)  

**Abstract**  
> **6. Issuance and Publishing Licences**  
> Anyone who intends to distribute, display, publish or reprint material that is copyright under the Republic of Iceland from the NLSI shall apply for the issuance and publication to NLSI. The same applies to the use of derived materials based on material from NLSI. The application must include details of where it is planned to publish the material. As a confirmation of the application the NLSI grants the user a numbered publishing license.
