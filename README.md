# WebApi .NET Framework

Este proyecto es una API REST desarrollada en .NET Framework que permite la gestión de productos en una base de datos SQL Server. Implementa operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para los productos y está diseñado para ser ejecutado en un entorno Windows.

## Tecnologías utilizadas

- .NET Framework
- Entity Framework 6
- SQL Server
- Swagger para la documentación de la API (usando Swashbuckle)

## Estructura del proyecto

- **Controllers**: Contiene el `ProductsController`, que maneja los endpoints para las operaciones CRUD.
- **Models**: Incluye el modelo `Product`.
- **Data**: Define `AppDbContext`, el contexto de Entity Framework.

## Instalación

1. Clona el repositorio y abre el proyecto en Visual Studio.
2. Asegúrate de tener SQL Server en ejecución y crea una base de datos llamada `webapinet`.
3. Actualiza la cadena de conexión en `Web.config` en la sección `connectionStrings`:
   ```xml
   <add name="DefaultConnection" connectionString="Data Source=localhost;Initial Catalog=webapinet;User ID=tu_usuario;Password=tu_contraseña" providerName="System.Data.SqlClient" />
