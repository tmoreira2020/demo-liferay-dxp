FROM mysql:5
ADD ./health-check /usr/local/bin/
RUN chmod +x /usr/local/bin/health-check
COPY conf.d/* /etc/mysql/conf.d/
HEALTHCHECK CMD ["health-check"]
CMD ["mysqld", "--datadir=/shared/mysql"]
