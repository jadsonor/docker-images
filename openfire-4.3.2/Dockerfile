FROM openjdk:8-jre-stretch

COPY ./openfire_4_3_2.tar.gz /home

COPY ./startup.sh /home

WORKDIR /home

RUN ["tar", "-xzf", "openfire_4_3_2.tar.gz"]

RUN ["chmod", "+x", "openfire/bin/openfire.sh"]

ENTRYPOINT [ "/home/startup.sh" ]

EXPOSE 9090 9091 5222 5223