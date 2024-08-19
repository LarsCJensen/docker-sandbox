FROM ubuntu

LABEL maintainer="Lars Jensen <lars.c.jensen@gmail.com>"

USER root

COPY ./entrypoint.bash /

RUN apt -y update
RUN apt -y install curl bash
RUN chmod 755 /entrypoint.bash

USER nobody

# What should be run
ENTRYPOINT [ "/entrypoint.bash" ]