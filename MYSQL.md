# MySQL Docker Setup with Docker Compose

This project sets up a MySQL database instance using Docker and Docker Compose. The MySQL container is configured through a `docker-compose.yml` file, with environment variables defined in a separate `.env` file.

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Clone this repository.
2. Create a `.env` file in the root directory of the project with the following environment variables:

```
MYSQL_ROOT_PASSWORD=your_root_password
MYSQL_DATABASE=your_database_name
MYSQL_USER=your_username
MYSQL_PASSWORD=your_password
```

3. Run the following command to start the MySQL container:

```
docker-compose up -d
```

4. To stop the MySQL container, run the following command:

```
docker-compose down
```

## Connecting to the MySQL Database

To connect to the MySQL database, you can use a MySQL client such as MySQL Workbench or the MySQL command line client. Use the following connection details:

- Host: `localhost`
- Port: `3306`
- Username: `your_username`
- Password: `your_password`

Or you can connect to the MySQL container directly using the following command:

```
docker exec -it mysql-db mysql -u your_username -p
```

## License

This project is open source and available under the [MIT License](LICENSE).
```
