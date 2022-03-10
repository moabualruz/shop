# Shop Microservice

![Infrastructure broad design](https://github.com/moabualruz/shop/raw/main/Micro%20Services%20Diagram.png?raw=true)

## Start

- Clone the 2 sample modules
- Build up using docker

 ```bash
 docker compose up -d
 ```

- Go to each service docker machine and in the module folder:
    + composer packages
       ```bash
       composer install
       ```
    + do migrate
       ```bash
       php bin/console doctrine:migrations:migrate
       ```

## Ports

All ports are forwarded to local host, main ones are:

- 8030 for voucher service
- 8040 for order service
- Please check other ports in the `docker-compose.yml` file
