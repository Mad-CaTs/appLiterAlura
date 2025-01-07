# Biblioteca Literaria - LiterAlura

Proyecto de biblioteca de libros desarrollado en Java con Spring Boot y Gradle que permite almacenar y gestionar información de libros a través de una API y realizar búsquedas en una base de datos PostgreSQL.

## Características

- **Consulta de libros**: Busca libros por título, autores, idioma, temas y número de descargas.
- **Almacenamiento**: Guarda libros y autores en PostgreSQL.
- **Estadísticas**: Calcula estadísticas sobre el número de descargas de los libros.
- **Consulta de API**: Obtiene datos de libros de la API de Gutendex y los transforma para la base de datos.

## Tecnologías

- **Java 17**
- **Spring Boot**: Framework principal.
- **Gradle**: Gestión de dependencias.
- **JPA (Java Persistence API)** y **Hibernate**: Gestión de entidades y relaciones en la base de datos.
- **PostgreSQL**: Base de datos para libros y autores.
- **Jackson**: Deserialización de datos JSON.
- **Gutendex API**: Fuente de información de libros.

## Instalación y Configuración

1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/tu_usuario/appLiterAlura.git
   cd appLiterALura
   ```

2. **Configura la base de datos**:
   - Crea una base de datos en PostgreSQL (ej. mdleo_literalura).
   - Actualiza `application.properties` con tus credenciales:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/tu_base_de_datos
     spring.datasource.username=tu_usuario
     spring.datasource.password=tu_contraseña
     ```

3. **Construye el proyecto**:
   ```bash
   ./gradlew build
   ```

4. **Ejecuta la aplicación**:
   ```bash
   ./gradlew bootRun
   ```

5. **Alternativa sin línea de comando**: Usa Spring Initializr:
   - Link: https://start.spring.io
   - Introduce la información y dependencias necesarias.

## Uso

Al iniciar la aplicación, verás un menú en la consola con las siguientes opciones:

1. **Buscar Libros**: Busca libros en la API de Gutendex y los guarda en la base de datos.
2. **Listar Libros**: Muestra todos los libros almacenados.
3. **Listar Libros por idioma**: Filtra libros por idioma.
4. **Listar Autores**: Muestra todos los autores y sus libros.
5. **Listar Autores por año**: Encuentra autores vivos por año.
6. **Top 10 Libros más descargados**: Muestra los más descargados.
7. **Buscar Autores por nombre**: Busca autores por nombre.
8. **Análisis de datos**: Muestra estadísticas de descargas.

## Contribuciones

Las contribuciones son bienvenidas. Abre un *issue* para discutir cambios que desees hacer.

## Documentos Complementarios

- Spring Boot Documentation: https://docs.spring.io/spring-boot/index.html
- JPA Query Methods: https://docs.spring.io/spring-data/jpa/reference/jpa/query-methods.html
- API Gutendex: https://gutendex.com
- Postman: https://www.postman.com/downloads/

## Conclusiones

Un gran desafío que me llevó a investigar sobre el uso de JPA en Java con Gradle y relaciones muchos a muchos. Resultó interesante desarrollar conceptos nuevos y afrontar problemas complejos.
