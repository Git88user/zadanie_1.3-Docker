FROM postgres:latest
ENV POSTGRES_PASSWORD=secret
ENV POSTGRES_USER=username
ENV POSTGRES_DB=database
ENV POSTGRES_HOST=db
COPY init_scripts/init.sql /docker-entrypoint-initdb.d/init.sql
CMD ["psql", "U", "postgres"]
#RUN psql -U postgres