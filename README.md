# Ejercicios prueba tecnica Pro Contacto

Este repositorio contiene ejercicios teóricos y prácticos sobre el protocolo HTTP, conceptos de APIs, y funcionalidades de Salesforce. Incluye desde preguntas conceptuales hasta implementaciones en código Apex para integración con servicios externos.

---

## 📚 Listado de Ejercicios

- [Ejercicio 2: Preguntas sobre HTTP](#ejercicio-2-preguntas-sobre-http)  
- [Ejercicio 3: Ejemplo de respuesta JSON](#ejercicio-3-ejemplo-de-respuesta-json)  
- [Ejercicio 6: Soluciones y funcionalidades de Salesforce](#ejercicio-6-soluciones-y-funcionalidades-de-salesforce)  
- [Ejercicio 7: Servicio de actualización de contactos](#ejercicio-7-servicio-de-actualización-de-contactos)  

---

## 🔍 Ejercicio 2: Preguntas sobre HTTP

### 1. ¿Qué es un servidor HTTP?
Un servidor HTTP es un programa que recibe y responde solicitudes hechas por los clientes mediante el protocolo HTTP. Su función principal es enviar páginas web, archivos u otros recursos al cliente.

### 2. ¿Qué son los verbos HTTP? Mencionar los más conocidos
Los verbos HTTP indican la acción que se quiere realizar sobre un recurso del servidor.

| Verbo   | Función principal |
|---------|------------------|
| GET     | Obtener datos del servidor |
| POST    | Enviar datos para crear algo nuevo |
| PUT     | Actualizar un recurso existente |
| PATCH   | Actualizar parcialmente un recurso |
| DELETE  | Eliminar un recurso |
| HEAD    | Solicitar solo los encabezados |

### 3. ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?
- **Request**: Mensaje que envía el cliente al servidor. Contiene URL, método, headers y, a veces, datos.
- **Response**: Mensaje que devuelve el servidor al cliente con el resultado (HTML, JSON, error, etc.).

Los headers son pares clave-valor incluidos en el request y response que aportan información adicional 
(ej: `Content-Type: application/json`).

### 4. ¿Qué es un queryString?
Es la parte de una URL que contiene parámetros enviados al servidor, colocados después del signo `?` y separados por `&`.  
Ejemplo: `https://ejemplo.com/usuarios?nombre=Pepe&edad=52`

### 5. ¿Qué es el responseCode?
Es un número que el servidor envía al cliente para indicar el resultado de la solicitud.

| Código | Significado |
|--------|-------------|
| 100-199 | Respuestas informativas |
| 200-299 | Respuestas exitosas |
| 300-399 | Redirecciones |
| 400-499 | Errores del cliente |
| 500-599 | Errores del servidor |

### 6. ¿Cómo se envía la data en un GET y cómo en un POST?
- **GET**: Los datos se envían en la URL como query string.
  Ejemplo: GET `/buscar?nombre=Juan`
- **POST**: Los datos se envían en el cuerpo (body) de la solicitud.

### 7. ¿Qué verbo HTTP utiliza el navegador cuando accedemos a una página?
El navegador usa el método **GET** para solicitar el contenido de la página.

### 8. Explicar brevemente JSON y XML
- **JSON**: Formato liviano, muy usado en APIs.
  ```json
  { "nombre": "Ana", "edad": 25, "ciudad": "Madrid" }
- **XML**: Formato basado en etiquetas, más pesado pero estructurado.
  ```xml
  <persona>
    <nombre>Ana</nombre>
    <edad>25</edad>
    <ciudad>Madrid</ciudad>
  </persona>
### 9. Explicar brevemente SOAP
SOAP es un protocolo estándar para comunicación entre sistemas usando XML. 
Es más riguroso y usado en entornos empresariales.
Se basa en mensajes muy estructurados 
Usa principalmente HTTP o SMTP 

### 10. Explicar brevemente REST
REST (Representational State Transfer) es un estilo de arquitectura para diseñar APIs que usan HTTP. 

Principios: 

Usa verbos HTTP (GET, POST, PUT, DELETE). 
Los recursos se identifican mediante URLs. 
Devuelve datos en formato JSON (mayormente). 
Es ligero, rápido y fácil de usar. 

### 11. ¿Qué son los headers en un request?  ¿Para qué se utiliza el key Content-Type en un header?
Los headers en una request son metadatos enviados por el cliente al servidor que describen el contenido o la petición. 

Ejemplo: 

`Authorization:` Bearer token123 
`Content-Type:` application/json 

El key Content-Type en un header se usa para indicar el tipo de datos que se envían o reciben.
Ejemplos:

`application/json` → cuerpo en formato JSON

`text/html` → cuerpo en HTML

`multipart/form-data` → envío de archivos

## 📄 Ejercicio 3: Ejemplo de respuesta JSON





































  
