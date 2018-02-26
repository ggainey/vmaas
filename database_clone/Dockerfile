# Dockerfile uses default postgresql latest image
# with applied vmaas database schema
FROM postgres

# Maintener
MAINTAINER Grant Gainey <ggainey@redhat.com>

ENV POSTGRES_USER 'vmaas_user'
ENV POSTGRES_PASSWORD 'vmaas_passwd'
ENV POSTGRES_DB 'vmaas'

ADD ./pgres_dump_file.sql /docker-entrypoint-initdb.d/

# Expose port
EXPOSE 5432
