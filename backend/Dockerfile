FROM openjdk:8-jre-alpine

COPY *.jar /srv/
COPY ext/ /srv/
COPY backend-entry.sh /

ENTRYPOINT [ "/backend-entry.sh" ]

