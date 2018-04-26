FROM centos:7
MAINTAINER nshota45 <shota.nakano.0405@gmail.com>

RUN yum install -y java-1.8.0-openjdk.x86_64 java-1.8.0-openjdk-devel.x86_64
RUN curl -o /usr/bin/digdag --create-dirs -L "https://dl.digdag.io/digdag-latest"
RUN chmod +x /usr/bin/digdag

EXPOSE 9876
ADD start_digdag_server.sh /usr/bin/start_digdag_server.sh
RUN chmod +x /usr/bin/start_digdag_server.sh
CMD ["/usr/bin/start_digdag_server.sh"]
