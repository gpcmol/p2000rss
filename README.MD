Aardbevingen:
http://cdn.knmi.nl/knmi/map/page/seismologie/lijst-van-herziene-plaats.csv

Mapping:
PUT aardbevingen
 {
   "mappings": {
     "items": {
	   "_all": { "enabled": false  },
       "properties": {
	     "Diepte" : { "type": "float" },
	     "Plaats_herzien" : { "type": "keyword" },
	     "Plaats_oud" : { "type": "keyword" },
	     "Magnitude" : { "type": "float" },
	     "Diepte" : { "type": "keyword" },
	     "location": { "type": "geo_point" },
	     "DatumTijd": { "type": "date","format": "yyyy-MM-dd HH:mm:ss" }
       }
     }
   }
 }
 