FROM centos:8

RUN yum update -y && yum install -y bind bind-utils

RUN mkdir -p /opt
COPY ./entrypoint.sh /opt/entrypoint.sh
RUN chmod +x /opt/entrypoint.sh

ENTRYPOINT ["/opt/entrypoint.sh"]
