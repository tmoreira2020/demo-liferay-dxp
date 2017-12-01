FROM elasticsearch:2.4.6
RUN /usr/share/elasticsearch/bin/plugin install analysis-smartcn
RUN /usr/share/elasticsearch/bin/plugin install analysis-kuromoji
RUN mkdir -p /shared/elasticsearch/data
RUN chown -R elasticsearch:elasticsearch /shared/elasticsearch
ADD elasticsearch.yml /usr/share/elasticsearch/config
