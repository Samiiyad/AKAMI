CEF Connector 1.7.8 Configuration for Akamai SIEM

System Requirements

Hardware Requirements


Installation Instructions

Retrieve the latest CEFConnector distribution package from the Akamai Support Page and transfer the package using either Linux command “wget http://server/CEFConnector-1.0.zip” or using SFTP (SSH File Transfer Protocol).



You can execute the shell script with the following commands (start | stop | status | resetdb). Resetdb will delete cefconnector.db which contains the last successful offset. Removing the file will cause the connector to process offset=NULL as long as timebased is false. If timebased is true and to parameter is null, a new offset will be saved after the first successful pull.