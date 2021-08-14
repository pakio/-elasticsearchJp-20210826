# Use Elasticsearch v7.14.0
FROM docker.elastic.co/elasticsearch/elasticsearch:7.14.0

# install icu and kuromoji
RUN elasticsearch-plugin install analysis-icu && elasticsearch-plugin install analysis-kuromoji

# copy original dictionary
COPY ./sample.dic /usr/share/elasticsearch/config/sample.dic
COPY ./synonyms.txt /usr/share/elasticsearch/config/synonyms.txt
