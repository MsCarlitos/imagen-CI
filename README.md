
# Documentación del Proyecto CodeIgniter 3

## Tabla de Contenidos

- [Creación de un Proyecto CodeIgniter 3](#creación-de-un-proyecto-codeigniter-3)
  - [Pasos para Configurar el Entorno de Desarrollo](#pasos-para-configurar-el-entorno-de-desarrollo)
    - [Opción 1: Nuevo Proyecto](#opción-1-nuevo-proyecto)
    - [Opción 2: Proyecto Existente](#opción-2-proyecto-existente)
- [Creating a CodeIgniter 3 Project](#creating-a-codeigniter-3-project)
  - [Steps to Set Up the Development Environment](#steps-to-set-up-the-development-environment)
    - [Option 1: New Project](#option-1-new-project)
    - [Option 2: Existing Project](#option-2-existing-project)

---

# Creación de un Proyecto de CodeIgniter 3

## Pasos para Configurar el Entorno de Desarrollo

### Opción 1: Nuevo Proyecto

1. **Ejecuta el archivo `docker-compose.yml`:**
   - Renombra el archivo `.env.development` a `.env`.
   - Edita el archivo `.env` y completa los campos según tus preferencias:
     ```plaintext
     DOCKER_CONTAINER=
     DB_NAME=

     MYSQL_ROOT_PASSWORD=
     MYSQL_DATABASE=
     MYSQL_USER=
     MYSQL_PASSWORD=
     MYSQL_PORT=

     WEB_PORT=
     ```
   - Ejecuta el siguiente comando en la terminal desde la raíz de tu proyecto:
     ```bash
     docker-compose up --build
     ```
   - Esto instalará las carpetas `php` y `mysql` dentro de la carpeta `app`, además de crear los archivos Dockerfile.

2. **Preparación del archivo `docker-compose-two.yml`:**
   - Arrastra el archivo `docker-compose-two.yml` dentro de la carpeta `app`.

   -Arrastra el archivo `.env` dentro de la carpeta `app`.

3. **Renombrar el archivo:**
   - Renombra el archivo `docker-compose-two.yml` a `docker-compose.yml`. Esto reemplazará el archivo anterior de configuración.

4. **Levantar el entorno de desarrollo:**
   - Abre una terminal y navega a la carpeta `app`:
     ```bash
     cd app
     ```
   - Ejecuta el siguiente comando para levantar todo el entorno de desarrollo de CodeIgniter 3:
     ```bash
     docker compose up --build -d
     ```

### Opción 2: Proyecto Existente

Si ya tienes un proyecto de CodeIgniter empezado:

1. **Agrega tu proyecto:**
   - Coloca tu proyecto de CodeIgniter en una carpeta llamada `php` dentro de la carpeta `app`.

2. **Crea una carpeta vacía:**
   - Crea una carpeta vacía llamada `mysql` dentro de la carpeta `app`.

3. **Agregar y renombrar el archivo:**
   - Desde la raíz del proyecto, arrastra el archivo `docker-compose-two.yml` a la carpeta `app` y renómbralo a `docker-compose.yml`.

4. **Renombrar y editar el archivo `.env`:**
   - Renombra el archivo `.env.development` a `.env`.
   - Edita el archivo `.env` y completa los campos según tus preferencias:
     ```plaintext
     DOCKER_CONTAINER=
     DB_NAME=

     MYSQL_ROOT_PASSWORD=
     MYSQL_DATABASE=
     MYSQL_USER=
     MYSQL_PASSWORD=
     MYSQL_PORT=

     WEB_PORT=
     ```

5. **Levantar el entorno de desarrollo:**
   - Abre una terminal y navega a la carpeta `app`:
     ```bash
     cd app
     ```
   - Ejecuta el siguiente comando para levantar todo el entorno de desarrollo de CodeIgniter 3:
     ```bash
     docker compose up -d
     ```

Ahora tu entorno de desarrollo de CodeIgniter 3 debería estar en funcionamiento.

**¡Feliz hackeo!**

---


# Creating a CodeIgniter 3 Project

## Steps to Set Up the Development Environment

### Option 1: New Project

1. **Run the `docker-compose.yml` file:**
   - Rename the `.env.development` file to `.env`.
   - Edit the `.env` file and fill in the fields according to your preferences:
     ```plaintext
     DOCKER_CONTAINER=
     DB_NAME=

     MYSQL_ROOT_PASSWORD=
     MYSQL_DATABASE=
     MYSQL_USER=
     MYSQL_PASSWORD=
     MYSQL_PORT=

     WEB_PORT=
     ```
   - Run the following command in the terminal from the root of your project:
     ```bash
     docker-compose up --build
     ```
   - This will create the `php` and `mysql` folders inside the `app` folder, as well as create the Dockerfile files.

2. **Prepare the `docker-compose-two.yml` file:**
   - Drag the `docker-compose-two.yml` file into the `app` folder.

   - Drag the `.env` file into the `app` folder.

3. **Rename the file:**
   - Rename the `docker-compose-two.yml` file to `docker-compose.yml`. This will replace the previous configuration file.

4. **Start the development environment:**
   - Open a terminal and navigate to the `app` folder:
     ```bash
     cd app
     ```
   - Run the following command to start the entire development environment for CodeIgniter 3:
     ```bash
     docker compose up --build -d
     ```

### Option 2: Existing Project

If you already have a CodeIgniter project started:

1. **Add your project:**
   - Place your CodeIgniter project in a folder named `php` inside the `app` folder.

2. **Create an empty folder:**
   - Create an empty folder named `mysql` inside the `app` folder.

3. **Add and rename the file:**
   - From the root of the project, drag the `docker-compose-two.yml` file into the `app` folder and rename it to `docker-compose.yml`.

4. **Rename and edit the `.env` file:**
   - Rename the `.env.development` file to `.env`.
   - Edit the `.env` file and fill in the fields according to your preferences:
     ```plaintext
     DOCKER_CONTAINER=
     DB_NAME=

     MYSQL_ROOT_PASSWORD=
     MYSQL_DATABASE=
     MYSQL_USER=
     MYSQL_PASSWORD=
     MYSQL_PORT=

     WEB_PORT=
     ```

5. **Start the development environment:**
   - Open a terminal and navigate to the `app` folder:
     ```bash
     cd app
     ```
   - Run the following command to start the entire development environment for CodeIgniter 3:
     ```bash
     docker compose up -d
     ```

Your development environment for CodeIgniter 3 should now be up and running.

**Happy hacking!**
