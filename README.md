# Ejercicios prueba tecnica Pro Contacto

Este repositorio contiene ejercicios teóricos y prácticos sobre el protocolo HTTP, conceptos de APIs, y funcionalidades de Salesforce. Incluye desde preguntas conceptuales hasta implementaciones en código Apex para integración con servicios externos.

---

## 📚 Listado de Ejercicios

- [Ejercicio 2: Preguntas sobre HTTP](#-ejercicio-2-preguntas-sobre-http)  
- [Ejercicio 3: Ejemplo de respuesta JSON](#-ejercicio-3-ejemplo-de-respuesta-json)
- [Ejercicio 4: Módulos de Trailhead](#-ejercicio-4-módulos-de-trailhead)
- [Ejercicio 5: Objetos de Salesforce](#-ejercicio-5-objetos-de-salesforce)
- [Ejercicio 6: Conocimientos de Salesforce](#-ejercicio-6-conocimientos-de-salesforce)
- [Ejercicio 7: Resolución del ejercicio](#-ejercicio-7-resolución-del-ejercicio)

---

# 🔍 Ejercicio 2: Preguntas sobre HTTP

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

# 📄 Ejercicio 3: Ejemplo de respuesta JSON

## Punto 1 

![Captura del punto 1](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_1.png?raw=true)

[Ejercicio 3 - Punto 1](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_1.png)

## Punto 2 

![Captura del punto 2](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_2.png?raw=true)

[Ejercicio 3 - Punto 2](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_2.png)

## Punto 3 

![Captura del punto 3](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_3.png?raw=true)

[Ejercicio 3 - Punto 3](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Ejercicio_3_Punto_3.png)


### Diferencias entre el punto 1 y el punto 3 

- Punto 1: La respuesta mostrará los contactos existentes (probablemente vacío si es la primera vez). 

- Punto 3: La respuesta incluirá el nuevo contacto que agregaste con el POST. 

- Conclusión: El POST agrega datos al servidor, y el GET te permite ver esos datos actualizados. 


# 📚 Ejercicio 4: Módulos de Trailhead

- Fundamento de la plataforma Salesforce 
- Fundamentos de Apex y .NET 
- Modelado de datos 
- Fundamentos y base de datos de Apex 
- Desencadenadores de Apex 
- Apex Integration Services 

[Mi Perfil de Trailhead](https://www.salesforce.com/trailblazer/smmburzyroir9ubtkf)

# 📄 Ejercicio 5: Objetos de Salesforce


## 📊 Objetos de Salesforce: Explicación Conceptual, Campos y Relaciones

### 🎯 1. Lead (Prospecto)
**Concepto:** Representa un prospecto o posible cliente que no ha sido calificado aún. Es el punto de entrada en el proceso de ventas.

Campos Principales:

- `FirstName`, `LastName`
- `Company`
- `Email`, `Phone`
- `Status` (Nuevo, Contactado, Calificado, No calificado)
- `LeadSource` (Origen del lead)
- `Industry` (Industria)
- `Rating` (Calificación)

Relaciones:

- Puede convertirse en **Account **, **Contact ** y **Opportunity **

### 🏢 2. Account (Cuenta)
**Concepto:** Representa una empresa, organización o persona jurídica con la que se tiene una relación comercial.

**Campos Principales:**
- `Name`
- `Type` (Cliente, Prospecto, etc.)
- `Industry`
- `Phone`, `Website`
- `BillingAddress`, `ShippingAddress`
- `AnnualRevenue`

**Relaciones:**
- Tiene múltiples **Contacts**
- Puede tener múltiples **Opportunities**
- Relacionado con **Cases** y **Assets**

---

### 👤 3. Contact (Contacto)
**Concepto:** Representa una persona específica que trabaja en una cuenta, generalmente un contacto comercial.

**Campos Principales:**
- `FirstName`, `LastName`
- `Email`, `Phone`
- `Title` (Cargo)
- `Department` (Departamento)
- `AccountId` (Relación con Account)

**Relaciones:**
- Pertenece a un **Account**
- Puede estar relacionado con **Opportunities** y **Cases**

---

### 💼 4. Opportunity (Oportunidad)
**Concepto:** Representa una posible venta o negocio pendiente con un cliente.

**Campos Principales:**
- `Name`
- `AccountId` (Cuenta relacionada)
- `CloseDate` (Fecha de cierre esperada)
- `Stage` (Etapa en el proceso de ventas)
- `Amount` (Monto)
- `Probability` (Probabilidad de cierre)

**Relaciones:**
- Pertenece a un **Account**
- Puede tener **Quotes** y **Products**

---

### 📦 5. Product (Producto)
**Concepto:** Representa un producto o servicio que la empresa vende.

**Campos Principales:**
- `Name`
- `ProductCode` (Código del producto)
- `Description`
- `IsActive` (Está activo)
- `Family` (Familia del producto)

**Relaciones:**
- Relacionado con **PriceBookEntry**
- Puede ser parte de **Opportunities** y **Quotes**

---

### 💰 6. PriceBook (Lista de Precios)
**Concepto:** Define los precios de los productos. Puede haber una lista estándar y listas personalizadas.

**Campos Principales:**
- `Name`
- `IsActive`
- `Description`
- `IsStandard` (Es la lista estándar)

**Relaciones:**
- Contiene **PriceBookEntry** (entradas de precios)
- Usado en **Opportunities** y **Quotes**

---

### 📄 7. Quote (Cotización)
**Concepto:** Documento formal que presenta precios y términos para productos/servicios a un cliente.

**Campos Principales:**
- `Name`
- `OpportunityId` (Oportunidad relacionada)
- `Status` (Enviada, Aprobada, Rechazada)
- `ExpirationDate` (Fecha de expiración)
- `GrandTotal` (Total general)

**Relaciones:**
- Pertenece a una **Opportunity**
- Contiene **QuoteLineItems**

---

### 🔧 8. Asset (Activo)
**Concepto:** Representa un producto específico que un cliente ha comprado.

**Campos Principales:**
- `Name`
- `AccountId` (Cuenta propietaria)
- `ContactId` (Contacto principal)
- `Product2Id` (Producto relacionado)
- `PurchaseDate` (Fecha de compra)
- `Status` (Activo, Inactivo)

**Relaciones:**
- Pertenece a un **Account**
- Relacionado con un **Product**

---

### 🎫 9. Case (Caso)
**Concepto:** Representa una solicitud de servicio, problema o pregunta de un cliente.

**Campos Principales:**
- `CaseNumber` (Número automático)
- `Subject` (Asunto)
- `Description`
- `Status` (Nuevo, En curso, Cerrado)
- `Priority` (Prioridad)
- `AccountId`, `ContactId` (Relaciones)

**Relaciones:**
- Pertenece a un **Account** y **Contact**
- Puede usar **Articles** de **Knowledge Base**

---

### 📚 10. Article (Artículo)
**Concepto:** Representa artículos de la base de conocimiento que ayudan a resolver casos.

**Campos Principales:**
- `Title` (Título)
- `Summary` (Resumen)
- `Body` (Contenido)
- `KnowledgeArticleVersion`
- `PublishStatus` (Estado de publicación)

**Relaciones:**
- Usado para resolver **Cases**
- Parte de la **Knowledge Base**

## Diagrama de relaciones entre los objetos de Salesforce

![Diagrama de Arquitectura ProContacto - Relaciones entre Objetos Salesforce](./Diagrama_ProContacto.png?raw=true)

[Diagrama ProContacto](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Diagrama_ProContacto.png)

[Descargar de relaciones](https://github.com/Azursxz/DelgadoMatias_ProContacto_EvaluacionPractica/blob/main/Diagrama_ProContacto.drawio)

# 📚 Ejercicio 6: Conocimientos de Salesforce

### A. ¿Qué es Salesforce?
![Salesforce](https://img.shields.io/badge/Concepto-CRM-blue) 
Es una plataforma en la nube de CRM (Customer Relationship Management) que permite gestionar ventas, atención al cliente, marketing y otros procesos empresariales.

### B. ¿Qué es Sales Cloud?
![Sales Cloud](https://img.shields.io/badge/Producto-Sales_Cloud-orange)
Es la solución de Salesforce enfocada en la gestión de ventas: clientes potenciales, oportunidades, cuentas, contactos y pronósticos.

### C. ¿Qué es Service Cloud?
![Service Cloud](https://img.shields.io/badge/Producto-Service_Cloud-green)
Es la solución orientada al servicio al cliente. Permite gestionar casos, soporte, chat, conocimiento y canales de atención.

### D. ¿Qué es Health Cloud?
![Health Cloud](https://img.shields.io/badge/Producto-Health_Cloud-red)
Es una solución para el sector salud que centraliza datos de pacientes, historial médico y relaciones entre proveedores y aseguradoras.

### E. ¿Qué es Marketing Cloud?
![Marketing Cloud](https://img.shields.io/badge/Producto-Marketing_Cloud-purple)
Es la plataforma de automatización de marketing digital que gestiona campañas por correo, SMS, redes sociales y personalización de experiencias.

## ⚙️ Funcionalidades de Salesforce

### A. ¿Qué es un RecordType?
Permite crear diferentes procesos de negocio, campos y diseños de página según el tipo de registro dentro de un mismo objeto.

### B. ¿Qué es un ReportType?
Define qué objetos y relaciones están disponibles al crear un informe, sirviendo como plantilla base.

### C. ¿Qué es un Page Layout?
Es el diseño o distribución visual de los campos, secciones, botones y listas relacionadas de un registro.

### D. ¿Qué es un Compact Layout?
Determina qué campos se muestran en la vista de encabezado o resumen de un registro (por ejemplo, en la app móvil o vista compacta).

### E. ¿Qué es un Perfil?
Controla los permisos de acceso a objetos, campos, páginas, aplicaciones y funcionalidades dentro de Salesforce.

### F. ¿Qué es un Rol?
Define la jerarquía de visibilidad de datos (quién puede ver los registros de quién) dentro de la organización.

### G. ¿Qué es un Validation Rule?
Es una regla que verifica que los datos ingresados cumplan una condición antes de permitir guardar un registro.

### H. ¿Diferencia entre Master-Detail y Lookup?
- **Master-Detail**: relación dependiente; si se elimina el registro maestro, se eliminan los detalles.
- **Lookup**: relación independiente; los registros pueden existir por separado.

### I. ¿Qué es un Sandbox?
Es una copia del entorno de producción usada para pruebas o desarrollo sin afectar los datos reales.

### J. ¿Qué es un Change Set?
Herramienta para migrar configuraciones y personalizaciones entre entornos (por ejemplo, de Sandbox a Producción).

### K. ¿Para qué sirve el Import Wizard de Salesforce?
Para importar datos (Leads, Accounts, Contacts, etc.) desde archivos CSV de forma sencilla y sin necesidad de código.

### L. ¿Para qué sirve la funcionalidad Web to Lead?
Permite generar automáticamente Leads desde formularios web insertados en un sitio externo.

### M. ¿Para qué sirve la funcionalidad Web to Case?
Crea casos de soporte automáticamente a partir de formularios web de atención al cliente.

### N. ¿Para qué sirve la funcionalidad Omnichannel?
Distribuye automáticamente interacciones (casos, chats, leads, etc.) a los agentes disponibles según reglas y prioridades.

### O. ¿Para qué sirve la funcionalidad Chatter?
Es la red social interna de Salesforce para colaboración entre usuarios, intercambio de archivos y actualizaciones.

## 🌐 Conceptos Generales

### A. ¿Qué significa SaaS?
Software as a Service: software basado en la nube al que se accede por internet sin instalación local.

### B. ¿Salesforce es SaaS?
Sí, Salesforce es un ejemplo típico de SaaS.

### C. ¿Qué significa que una solución sea Cloud?
Que se aloja y ejecuta en servidores en la nube, accesible desde cualquier lugar con internet.

### D. ¿Qué significa que una solución sea On-Premise?
Que el software está instalado y gestionado en servidores locales del cliente.

### E. ¿Qué es un pipeline de ventas?
Es la representación visual o estructurada de las etapas por las que pasa una oportunidad de venta.

### F. ¿Qué es un funnel de ventas?
Es el embudo que muestra la conversión de prospectos a clientes a través de diferentes etapas del proceso comercial.

### G. ¿Qué significa Customer Experience?
Es la experiencia global que un cliente tiene con una empresa a lo largo de todas sus interacciones.

### H. ¿Qué significa omnicanalidad?
Capacidad de ofrecer una experiencia integrada y coherente en múltiples canales (teléfono, email, chat, redes, etc.).

### I. ¿Qué significa que un negocio sea B2B / B2C / Qué es un KPI?
- **B2B**: negocio entre empresas (Business to Business)
- **B2C**: negocio entre empresa y consumidor final (Business to Consumer)
- **KPI**: indicador clave de rendimiento usado para medir el éxito de un objetivo

### J. ¿Qué es una API y en qué se diferencia de una REST API?
- **API**: interfaz que permite que diferentes sistemas se comuniquen
- **REST API**: tipo de API que usa el protocolo HTTP y formato JSON, más ligera y moderna

### K. ¿Qué es un Proceso Batch?
Es un proceso que ejecuta grandes volúmenes de datos en lotes, útil para tareas programadas o masivas.

### L. ¿Qué es Kanban?
Método visual para gestionar tareas y flujos de trabajo mediante tarjetas en columnas (por ejemplo, "Pendiente", "En Progreso", "Hecho").

### M. ¿Qué es un ERP?
Enterprise Resource Planning: sistema que integra y gestiona los recursos internos de una empresa (finanzas, inventario, producción, etc.).

### N. ¿Salesforce es un ERP?
No. Salesforce es principalmente un CRM, aunque puede integrarse con ERPs o tener funciones similares mediante extensiones.


# 📚 Ejercicio 7: Resolución del ejercicio

## Aclaraciones de la resolución del ejercicio

### Remote Site Settings

Para que el código funcione se debe crear un nuevo sitio remoto de la pagina web que utilizamos, en nuestro caso es:

`https://procontacto-reclutamiento-default-rtdb.firebaseio.com`

### ¿Por qué se usó System.enqueueJob()?

- Límites de callouts en triggers: Los triggers no pueden hacer callouts directamente
- Procesamiento asíncrono: Permite ejecutar operaciones largas sin bloquear la transacción actual
- Flexibilidad: Mayor control sobre el procesamiento

## Resolución


```apex
      public class ContactCalloutService { 
      
      public static void updateEmailFromProcontacto(Set<Id> contactIds) { 
          // Encolar el trabajo asíncrono 
          System.enqueueJob(new EmailUpdateQueueable(contactIds)); 
      } 
       
      public class EmailUpdateQueueable implements Queueable, Database.AllowsCallouts { 
          private Set<Id> contactIds; 
           
          public EmailUpdateQueueable(Set<Id> contactIds) { 
              this.contactIds = contactIds; 
          } 
           
          public void execute(QueueableContext context) { 
              List<Contact> contactsToUpdate = [SELECT Id, idprocontacto__c, Email FROM Contact WHERE Id IN :contactIds AND idprocontacto__c != null]; 
              List<Contact> updatedContacts = new List<Contact>(); 
               
              for(Contact con : contactsToUpdate) { 
                  try { 
                      String endpoint = 'https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts/'  
                                         + con.idprocontacto__c + '.json'; 
                       
                      Http http = new Http(); 
                      HttpRequest request = new HttpRequest(); 
                      request.setEndpoint(endpoint); 
                      request.setMethod('GET'); 
                      request.setHeader('Content-Type', 'application/json'); 
                      request.setTimeout(10000); // 10 segundos timeout 
                       
                      HttpResponse response = http.send(request); 
                       
                      if(response.getStatusCode() == 200) { 
                          Map<String, Object> data = (Map<String, Object>) JSON.deserializeUntyped(response.getBody()); 
                          if(data != null && data.containsKey('email')) { 
                              String email = (String)data.get('email'); 
                              // Solo actualizar si el email es diferente y no está vacío 
                              if(String.isNotBlank(email) && email != con.Email) { 
                                  con.Email = email; 
                                  updatedContacts.add(con); 
                              } 
                          } 
                      } else { 
                          System.debug('Error en la respuesta HTTP: ' + response.getStatusCode() + ' - ' + response.getStatus()); 
                      } 
                  } catch(Exception e) { 
                      System.debug('Error al obtener datos del servicio para el contacto ' + con.Id + ': ' + e.getMessage() + ' - ' + e.getStackTraceString()); 
                  } 
              } 
               
              if(!updatedContacts.isEmpty()) { 
                  try { 
                      update updatedContacts; 
                      System.debug('Se actualizaron ' + updatedContacts.size() + ' contactos correctamente'); 
                  } catch(DmlException e) { 
                      System.debug('Error al actualizar contactos: ' + e.getMessage()); 
                  } 
              } 
          } 
      }
      }

```
### Trigger
```apex
    trigger ContactTrigger on Contact (after insert, after update) {
    Set contactIds = new Set(); 
    
    for(Contact con : Trigger.new){ 
     
        if(con.idprocontacto__c != null){ 
            contactIds.add(con.Id); 
        } 
    } 
     
    if(!contactIds.isEmpty()){ 
        ContactCalloutService.updateEmailFromProcontacto(contactIds); 
    } 
}

```
### Test

```apex
    @isTest private class ContactCalloutServiceTest { 
    
    // Mock que simula la respuesta del servicio REST 
    private class ContactHttpMock implements HttpCalloutMock { 
        public HTTPResponse respond(HTTPRequest req) { 
            HttpResponse res = new HttpResponse(); 
            res.setHeader('Content-Type', 'application/json'); 
            // Simula que el servicio devuelve un email 
            res.setBody('{"email": "mockedemail@test.com", "name": "Prueba"}'); 
            res.setStatusCode(200); 
            return res; 
        } 
    } 
     
    @isTest 
    static void testUpdateEmailFromProcontacto() { 
        // 1. Crear un contacto con idprocontacto 
        Contact c = new Contact( 
            LastName = 'Prueba Trigger', 
            idprocontacto__c = 'FAKE-ID-123' 
        ); 
        insert c; 
     
        // 2. Registrar el mock 
        Test.setMock(HttpCalloutMock.class, new ContactHttpMock()); 
     
        // 3. Ejecutar el método futuro dentro de Test.startTest / stopTest 
        Test.startTest(); 
        ContactCalloutService.updateEmailFromProcontacto(new Set<Id>{c.Id}); 
        Test.stopTest(); 
     
        // 4. Recuperar el contacto actualizado 
        Contact updated = [SELECT Email FROM Contact WHERE Id = :c.Id]; 
     
        // 5. Verificar que el campo Email se haya actualizado 
        System.assertEquals('mockedemail@test.com', updated.Email); 
    } 
     
    @isTest 
    static void testTriggerInvokesCallout() { 
        // Registrar el mock de nuevo 
        Test.setMock(HttpCalloutMock.class, new ContactHttpMock()); 
     
        // Insertar contacto que dispare el trigger 
        Test.startTest(); 
        Contact c2 = new Contact(LastName = 'Trigger', idprocontacto__c = 'FAKE-ID-456'); 
        insert c2; 
        Test.stopTest(); 
     
        // Verificar que el email fue actualizado por el trigger 
        Contact updated = [SELECT Email FROM Contact WHERE Id = :c2.Id]; 
        System.assertEquals('mockedemail@test.com', updated.Email); 
    } 
} 
```














  
