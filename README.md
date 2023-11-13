# Segundo parcial - seminario

## Creación de Imágenes:

A continuación, se detallan los comandos necesarios para construir las imágenes requeridas para los servicios utilizando Docker:

1. **API REST:**
    ```bash
    docker build -t backend .
    ```

2. **API SOAP:**
    ```bash
    docker build -t soap .
    ```

3. **Cliente:**
    ```bash
    docker build -t frontend .
    ```

4. **MySQL:**
    ```bash
    docker build -t mysqldb .
    ```

## Despliegue con Docker Swarm:

Para llevar a cabo el despliegue de los servicios mediante Docker Swarm, siga los siguientes pasos:

1. **Inicialización de Swarm:**
    ```bash
    docker swarm init
    ```

2. **Despliegue con Docker Stack:**
    ```bash
    docker stack deploy -c docker-compose.yml mis-servicios
    ```

## Detalles Adicionales:

- Para visualizar la interfaz, acceda a http://127.0.0.1:8080