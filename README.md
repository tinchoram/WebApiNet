# WebApi .NET Framework

Este proyecto es una API REST desarrollada en .NET Framework que permite la gesti�n de productos en una base de datos SQL Server. Implementa operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para los productos y est� dise�ado para ser ejecutado en un entorno Windows.

## Tecnolog�as utilizadas

- .NET Framework
- Entity Framework 6
- SQL Server
- Swagger para la documentaci�n de la API (usando Swashbuckle)

## Estructura del proyecto

- **Controllers**: Contiene el `ProductsController`, que maneja los endpoints para las operaciones CRUD.
- **Models**: Incluye el modelo `Product`.
- **Data**: Define `AppDbContext`, el contexto de Entity Framework.

## Instalaci�n

1. Clona el repositorio y abre el proyecto en Visual Studio.
2. Aseg�rate de tener SQL Server en ejecuci�n y crea una base de datos llamada `webapinet`.
3. Actualiza la cadena de conexi�n en `Web.config` en la secci�n `connectionStrings`:
   ```xml
   <add name="DefaultConnection" connectionString="Data Source=localhost;Initial Catalog=webapinet;User ID=tu_usuario;Password=tu_contrase�a" providerName="System.Data.SqlClient" />
