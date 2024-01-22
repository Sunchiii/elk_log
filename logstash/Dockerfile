FROM docker.elastic.co/logstash/logstash:7.7.0

RUN rm -f /usr/share/logstash/pipeline/logstash.conf
COPY logstash.conf /usr/share/logstash/pipeline/

CMD bin/logstash -f /usr/share/logstash/pipeline/logstash.conf
