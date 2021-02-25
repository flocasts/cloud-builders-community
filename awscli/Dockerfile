FROM python:3-alpine
RUN apk add --update \
    bash \
    groff \
    jq    \
    less  \
  && pip install awscli \
  && rm -rf /var/cache/apk/* ~/.cache/pip
ENV PAGER=less
ENTRYPOINT ["aws"]
