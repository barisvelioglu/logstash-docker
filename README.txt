docker build -t logstashtestimage .

docker run -p 5000:5000 -p 31311:31311 -v ~/Desktop/logstash/pipeline/:/usr/share/logstash/pipeline/ -v ~/Desktop/logstash/config/logstash.yml:/usr/share/logstash/logstash.yml logstashtestimage