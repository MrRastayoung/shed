########################################################################
# Dockerfile for Postgres training build
########################################################################

FROM shed/postgres_database

MAINTAINER Joan Ordinas <jordinas@escoladeltreball.org>

COPY training.sql.gz ${HOME}/database.sql.gz

RUN ./startdb.sh BUILD-TIME

# Space still wasted, but...
RUN rm -f ${HOME}/database.sql.gz

# vim:syntax=dockerfile:ai:sw=4:ts=4:et
