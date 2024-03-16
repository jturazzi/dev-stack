<p align="center"><img src="https://www.docker.com/wp-content/uploads/2023/08/logo-guide-logos-1.svg" width="300" alt="Docker"></p>

<h3 align="center">This setup provides a development environment with multiple services including a web server, database, adminer, mail server monitoring tool, portainer, and Traefik for reverse proxy.</h3>

## Usage

1. Clone this repository.
2. Navigate to the directory.
3. Modify environment variables if needed.
4. Start Docker containers: `docker-compose up -d`.

Access services:
- Web server: [http://localhost](http://localhost)
- Adminer: [http://adminer.local](http://adminer.local)
- Mailpit: [http://mailpit.local](http://mailpit.local)
- Portainer: [http://portainer.local](http://portainer.local)

*Note: DNS configuration is required on your DNS server or in the hosts file to reach the services.*

## Services

- Web: PHP-Nginx.
- Adminer: Database management.
- DB: MySQL server.
- Mailpit: Mail server monitoring.
- Portainer: Docker management.
- Traefik: Reverse proxy.
- Watchtower: Automated container updates.

## Configuration

1. Copy the `.env.example` file and copy it to `.env`.
2. Open the `.env` file in a text editor.
3. Modify the environment variables as needed. Here are the available variables:
    - `TZ`: Set the timezone (default: Europe/Paris).
    - `MYSQL_ROOT_PASSWORD`: Set the MySQL root password (default: root).
    - `DEV_DOMAIN`: Set the domain for local development (default: local).
4. Save the `.env` file.

## License

This project is licensed under the [MIT](LICENSE) License.
