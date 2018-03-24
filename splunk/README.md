# unraid-docker-templates
Splunk docker container template for unraid

samarelo's Splunk template.

This template pulls the latest splunk version from https://hub.docker.com/r/splunk/splunk/
All other configuration options are setup in this template

Volumes:
Container Path: /opt/splunk/var
Container Path: /opt/splunk/etc

Mapped Ports:
Container Port: 1514
Container Port: 8000
Container Port: 8089
Container Port: 9997


Extra Parameters:
-e "SPLUNK_START_ARGS=--accept-license --answer-yes" -e "OPTIMISTIC_ABOUT_FILE_LOCKING=1"

SPLUNK_START_ARGS:
--accept-license    to accept license agreement
--answer-yes         to agree to updating configuration files on upgrade
OPTIMISTIC_ABOUT_FILE_LOCKING=1      to correct warnings related to database validation
