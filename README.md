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
   - Asegúrate de que tu estructura de directorios tenga la carpeta `application` con las subcarpetas `php` y `mysql`.
   - Ejecuta el siguiente comando en la terminal desde la raíz de tu proyecto:
     ```bash
     docker-compose up -d
     ```
   - Esto instalará las carpetas `php` y `mysql` dentro de la carpeta `application`.

2. **Preparación del archivo `docker-compose-two.yml`:**
   - Arrastra el archivo `docker-compose-two.yml` dentro de la carpeta `application`.

3. **Renombrar el archivo:**
   - Renombra el archivo `docker-compose-two.yml` a `docker-compose.yml`. Esto reemplazará el archivo anterior de configuración.

4. **Levantar el entorno de desarrollo:**
   - Abre una terminal y navega a la carpeta `application`:
     ```bash
     cd application
     ```
   - Ejecuta el siguiente comando para levantar todo el entorno de desarrollo de CodeIgniter 3:
     ```bash
     docker compose up -d
     ```

### Opción 2: Proyecto Existente

Si ya tienes un proyecto de CodeIgniter empezado:

1. **Agrega tu proyecto:**
   - Coloca tu proyecto de CodeIgniter en una carpeta llamada `php` dentro de la carpeta `application`.

2. **Crea una carpeta vacía:**
   - Crea una carpeta vacía llamada `mysql` dentro de la carpeta `application`.

3. **Agregar y renombrar el archivo:**
   - Desde la raíz del proyecto, arrastra el archivo `docker-compose-two.yml` a la carpeta `application` y renómbralo a `docker-compose.yml`.

4. **Levantar el entorno de desarrollo:**
   - Abre una terminal y navega a la carpeta `application`:
     ```bash
     cd application
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
   - Ensure your directory structure has the `application` folder with the subfolders `php` and `mysql`.
   - Run the following command in the terminal from the root of your project:
     ```bash
     docker-compose up -d
     ```
   - This will install the `php` and `mysql` folders inside the `application` folder.

2. **Prepare the `docker-compose-two.yml` file:**
   - Drag the `docker-compose-two.yml` file into the `application` folder.

3. **Rename the file:**
   - Rename the `docker-compose-two.yml` file to `docker-compose.yml`. This will replace the previous configuration file.

4. **Start the development environment:**
   - Open a terminal and navigate to the `application` folder:
     ```bash
     cd application
     ```
   - Run the following command to start the entire development environment for CodeIgniter 3:
     ```bash
     docker compose up -d
     ```

### Option 2: Existing Project

If you already have a CodeIgniter project started:

1. **Add your project:**
   - Place your CodeIgniter project in a folder named `php` inside the `application` folder.

2. **Create an empty folder:**
   - Create an empty folder named `mysql` inside the `application` folder.

3. **Add and rename the file:**
   - From the root of the project, drag the `docker-compose-two.yml` file into the `application` folder and rename it to `docker-compose.yml`.

4. **Start the development environment:**
   - Open a terminal and navigate to the `application` folder:
     ```bash
     cd application
     ```
   - Run the following command to start the entire development environment for CodeIgniter 3:
     ```bash
     docker compose up -d
     ```

Your development environment for CodeIgniter 3 should now be up and running.

**Happy hacking!**
