# **Shopper-system**

Este proyecto implementa una arquitectura de microservicios utilizando Docker Compose. Incluye servicios para la gestión de productos, clientes, pedidos y pagos, además de una aplicación frontend.

Servicios Incluidos

- PostgreSQL (Base de datos)

- RabbitMQ (Mensajería)

Microservicios:

- ms-product (Gestión de productos)

- ms-customer (Gestión de clientes)

- ms-order (Gestión de pedidos)

- ms-payments (Gestión de pagos)

Frontend:

- app-shopper (Aplicación web)

# **Requisitos Previos**

- Docker Desktop instalado

  **Configuración Inicial**

  1. Clona este repositorio:
  ```bash
  git clone https://github.com/koko112189/shopper-system.git
  cd shopper-system
  ```

  2. Asegúrate de que cada microservicio tiene un archivo .env.example. Si no existe un archivo .env, se generará automáticamente al ejecutar los servicios.

  3. Revisa el archivo docker-compose.yml para verificar los valores de configuración.
 
  **Despliegue del Proyecto**
  Para levantar todos los servicios ejecuta el siguiente comando:
     
  ```bash
  docker-compose up -d --build
  ```

  NOTA: Si no tienes Docker , puedes clonar cada uno de los submodulos de este repositorio y desplegarlos uno a uno en tu máquina local, 
configurando previamente las variables de entorno en el .env.example y creando una copia en  un nuevo archivo .env

