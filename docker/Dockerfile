FROM lsiobase/alpine:3.9
FROM lsiobase/ubuntu:bionic

# set version label
ARG BUILD_DATE
ARG VERSION
LABEL build_version="Linuxserver.io version:- ${VERSION} Build-date:- ${BUILD_DATE}"
LABEL maintainer="<your github username here>"

# install packages
RUN \

##DO STUFF HERE
## END EACH LINE WITH && \
## EXCEPT THE LAST LINE OF THE BLOCK


# copy local files
COPY root/ /

# ports and volumes
EXPOSE PORT
VOLUME /volume

## NOTES ##
## Delete files\folders not needed
## The User abc, should be running everything, give that permission in any case you need it.
## When creating init's Use 10's where posible, its to allow add stuff in between when needed. also, do not be afraid to split custom code into several little ones.
## user abc and folders /app /config /defaults are all created by baseimage
## the first available init script is 30<your script>
## you can comment the beginning of each new RUN block but you cannot comment between commands in each RUN block.
