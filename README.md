# Inein Test Backend

Este proyecto es una API backend desarrollada para el test de Inein. A continuación, se detallan las instrucciones para la instalación, configuración y uso del proyecto.

## Requisitos

- PHP >= 7.4
- Composer
- MySQL

## Instalación

1. Clonar el repositorio:
    ```bash
    git clone https://github.com/MoisesGJ/inein-test-backend.git
    ```
2. Navegar al directorio del proyecto:
    ```bash
    cd inein-test-backend
    ```
3. Instalar las dependencias:
    ```bash
    composer install
    ```

## Configuración

1. Validar las variables de entrono en el archivo .env que se encuentran en la carpeta principal.

## Uso

1. Generar la clave de la aplicación:
    ```bash
    php artisan key:generate
    ```
2. Ejecutar las migraciones de la base de datos:
    ```bash
    php artisan migrate
    ```
3. Iniciar el servidor de desarrollo:
    ```bash
    php artisan serve
    ```

## Endpoints

A continuación, se listan algunos de los endpoints disponibles en la API:

- `POST /api/register` 
```json
{
	"name": "Moisés",
	"email": "moi@moi.com",
	"password": "moisesprb",
	"password_confirmation": "moisesprb"
}
```
- `POST /api/login` 
```json
{
	"email": "moi@moi.com",
	"password": "moisesprb",
}
```
- `POST /api/logout`
```json
{
    "Authorization": "Bearer your_access_token"
}
```

## Estructura del Proyecto

La estructura básica del proyecto es la siguiente:


- `app/`: Contiene el código fuente de la aplicación.
- `config/`: Contiene los archivos de configuración.
- `database/`: Contiene las migraciones y seeders de la base de datos.
- `routes/`: Contiene los archivos de rutas de la aplicación.
- `.env`: Archivo de configuración de entorno.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
