FROM docker.elastic.co/beats/filebeat:7.7.0
# Copy our custom configuration file
COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN chown root:filebeat /usr/share/filebeat/filebeat.yml
RUN mkdir /usr/share/filebeat/dockerlogs
RUN chown -R root /usr/share/filebeat/
RUN chmod -R go-w /usr/share/filebeat/
CMD ./filebeat -e
