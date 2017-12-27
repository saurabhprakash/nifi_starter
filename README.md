# nifi_starter

* Downloading and starting nifi Docs: https://nifi.apache.org/docs/nifi-docs/html/getting-started.html#downloading-and-installing-nifi
* Starting nifi: https://nifi.apache.org/docs/nifi-docs/html/getting-started.html#starting-nifi
* Command for starting nifi(location on mac: "/usr/local/Cellar/nifi/1.4.0"): 
  * NiFi in the foreground: ```run bin/nifi.sh run``` [By default it starts on http://localhost:8080/nifi/ , port can be changed in nifi.properties file present in conf directory]
  * NiFi in the background: ```run bin/nifi.sh start```
  * To check the status and see if NiFi is currently running, execute the command ```bin/nifi.sh status```
  * NiFi can be shutdown by executing the command ```bin/nifi.sh stop```
