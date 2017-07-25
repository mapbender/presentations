1.  Solr installieren
cd /data
wget http://apache.lauf-forum.at/lucene/solr/5.4.1/solr-5.4.1.tgz
tar -zxvf solr-5.4.1.tgz
cd solr-5.4.1/

2. solr_data aus der Cloud ablegen


Solr starten
/data/solr-5.4.1/bin/solr start -s /data/solr_data/

http://localhost:8983/solr/

Solr stoppen
/data/solr-5.4.1/bin/solr stop -all


Mapbender Element SimpleSearch hinzufügen:
* Dokumentation http://doc.mapbender3.org/de/bundles/Mapbender/CoreBundle/elements/simplesearch.html

http://localhost:8983/solr/places/select?wt=json&indent=true&rows=20

collection_path: response.docs

