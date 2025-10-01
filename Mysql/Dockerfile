FROM mysql:8.0

# Set the root password and allow remote connections (optional)

COPY backend.sql /docker-entrypoint-initdb.d/backend.sql

ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
ENV MYSQL_DATABASE=expense_db

EXPOSE 3306

# No CMD needed; the base image handles MySQL startup
