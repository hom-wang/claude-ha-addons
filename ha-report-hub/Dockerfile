ARG BUILD_FROM
FROM $BUILD_FROM
# busybox httpd lives in busybox-extras on Alpine; nothing else is needed for static pages
RUN apk add --no-cache busybox-extras
COPY run.sh httpd.conf /
RUN chmod a+x /run.sh
CMD ["/run.sh"]
