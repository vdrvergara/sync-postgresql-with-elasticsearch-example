1
# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch:6.6.2

# Add your elasticsearch plugins setup#here
# Example: 
RUN elasticsearch-plugin install -b https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v6.6.2/elasticsearch-analysis-ik-6.6.2.zip
RUN elasticsearch-plugin install -b https://github.com/medcl/elasticsearch-analysis-pinyin/releases/download/v6.6.2/elasticsearch-analysis-pinyin-6.6.2.zip
ENTRYPOINT su - elasticsearch -s /bin/sh -c "export PATH=$PATH:/opt/jdk-12/bin/ && /usr/share/elasticsearch/bin/elasticsearch"
