FROM alpine:3.8

WORKDIR /root

RUN apk add --no-cache curl bash docker openrc \
    && curl -LJO https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh \
    && chmod +x wait-for-it.sh \
    && rc-update add docker boot

ENTRYPOINT ["./wait-for-it.sh"]



