# curator_30d
A simple curator image which deletes entries from elasticsearch based on environment variables:

             HOST: elasticsearch
             PORT: 9200
             COMMAND: "curator --dry-run --config /etc/curator/config.yml /etc/curator/action_file.yml"
             PREFIX: logstash-
             DAYS:    30
             SCHEDULE: "0 0 0 * * ?"

This is modified from https://github.com/jimmikristensen/elk-curator-docker
