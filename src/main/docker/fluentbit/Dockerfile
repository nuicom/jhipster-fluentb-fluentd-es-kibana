FROM fluent/fluent-bit:1.2.2-debug

#RUN mkdir -p /logs && chmod 777 -R /logs
RUN ["mkdir", "-p", "/logs"]
RUN ["chmod", "777", "-R", "/logs"]

VOLUME ["/logs"]

ADD ./fluentbit.conf /fluent-bit/etc/fluentbit.conf
ADD ./custom_parsers.conf /fluent-bit/etc/custom_parsers.conf
