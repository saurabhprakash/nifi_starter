# nifi_starter

* Downloading and starting nifi Docs: https://nifi.apache.org/docs/nifi-docs/html/getting-started.html#downloading-and-installing-nifi
* Starting nifi: https://nifi.apache.org/docs/nifi-docs/html/getting-started.html#starting-nifi
* Command for starting nifi(location on mac: "/usr/local/Cellar/nifi/1.4.0"): 
  * NiFi in the foreground: ```run bin/nifi.sh run``` [By default it starts on http://localhost:8080/nifi/ , port can be changed in nifi.properties file present in conf directory]
  * NiFi in the background: ```run bin/nifi.sh start```
  * To check the status and see if NiFi is currently running, execute the command ```bin/nifi.sh status```
  * NiFi can be shutdown by executing the command ```bin/nifi.sh stop```
* Manage Templates(Export/Import/Create/Remove): https://nifi.apache.org/docs/nifi-docs/html/user-guide.html#Manage_Templates


Samples:

1. fetchTwitterDataAndAddToElasticsearch.xml: Fetches data from twitter and dumps to elasticsearch(version 5.x used)[https://community.hortonworks.com/articles/56121/how-to-pull-data-from-twitter-and-push-data-to-ela.html].
   * Before importing above in nifi replace the value for these two variables: "Consumer Key" and "Access Token"
   * Post importing set the values of "Consumer Secret" and "Access token secret" in GetTwitter Processor
