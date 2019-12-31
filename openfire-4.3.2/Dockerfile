FROM openjdk:8-jre-stretch

COPY ./openfire_4_3_2.tar.gz /home

WORKDIR /home

RUN ["tar", "-xzf", "openfire_4_3_2.tar.gz"]

RUN ["rm", "-rf", "openfire_4_3_2.tar.gz"]

RUN ["chmod", "+x", "openfire/bin/openfire.sh"]

ENTRYPOINT [ "/home/openfire/bin/openfire.sh", "start" ]

EXPOSE 9090 9091 5222 5223