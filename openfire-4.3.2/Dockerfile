FROM openjdk:8-jre-stretch

WORKDIR /home/openfire

COPY ./openfire_4_3_2.tar.gz /home/openfire

RUN ["tar", "-xvzf", "openfire_4_3_2.tar.gz"]

RUN ["chmod", "+x", "./openfire/bin/openfire.sh"]

ENTRYPOINT [ "./openfire/bin/openfire.sh", "start" ]

EXPOSE 9090 9091 5222 5223