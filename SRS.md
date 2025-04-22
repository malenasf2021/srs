# Especificación de Requisitos del Software (SRS)  
**Para:** `Programación II`  
**Version:** `1.0`  
**Autor:** `Malena Sánchez`  
**Organización:** `Ce.R.P. SurOeste Colonia`  
**Fecha:** `2025-04-30>`  

---

## **1. Introducción**  
### **1.1 Propósito**  
`<Identifique el producto cuyos requisitos de software se especifican en este documento, incluyendo el número de revisión o versión. Describa el alcance del producto que está cubierto por este ERS, particularmente si este ERS describe solo una parte del sistema o un único subsistema.>`  
Este documento describe los requisitos para el `<Nombre del Proyecto>`, un `<describir el sistema>`. Cubre `<enumerar las funcionalidades clave>`.  

### **1.2 Convenciones del documento**  
`<Describa cualquier estándar o convención tipográfica que se haya seguido al redactar este ERS, como el uso de fuentes o resaltados con un significado especial. Por ejemplo, indique si se asume que las prioridades de los requisitos de alto nivel se heredan en los requisitos detallados, o si cada declaración de requisito debe tener su propia prioridad.>`
- **Bold text** indicates key terms.  

### **1.3 Público objetivo y sugerencias de lectura**  
`<Describa los diferentes tipos de lectores a los que está destinado este documento, como desarrolladores, gerentes de proyecto, personal de marketing, usuarios, testers y redactores de documentación. Describa el contenido del resto de este ERS y cómo está organizado. Sugiérase una secuencia para la lectura del documento, comenzando por las secciones introductorias y continuando con las secciones más pertinentes para cada tipo de lector.>`

`<Ejemplo:>`  
- **Desarrolladores**: implementan el sistema.  
- **Testers**: verifican requerimientos.  
- **Interesados**: Revisar los objetivos del negocio.  

### **1.4 Alcance del proyecto**  
`<Proporcione una breve descripción del software que se está especificando y su propósito, incluyendo los beneficios, objetivos y metas relevantes. Relacione el software con los objetivos corporativos o estrategias empresariales. Si existe un documento separado de visión y alcance, haga referencia a él en lugar de duplicar su contenido aquí. Un ERS que especifique la próxima versión de un producto en evolución debe contener su propia declaración de alcance como un subconjunto de la visión estratégica a largo plazo del producto.>`

`<Ejemplo:>`  
Este sistema reemplazará a `<sistema heredado>` y proporcionará `<enumerar los beneficios clave>`.
Fuera del alcance: `<enumerar las funcionalidades excluidas>`.

### **1.5 Referencias**  
`<Enumere cualquier otro documento o dirección web a la que se haga referencia en este ERS. Estos pueden incluir guías de estilo de interfaz de usuario, contratos, normas, especificaciones de requisitos del sistema, documentos de casos de uso o un documento de visión y alcance. Proporcione suficiente información para que el lector pueda acceder a una copia de cada referencia, incluyendo el título, autor, número de versión, fecha y fuente o ubicación.>`

`<Ejemplo:>`  
- [Vision Document](#) (Link if available).  
- ISO 25010 Standard for Software Quality.  

---

## **2. Descripción general**  
### **2.1 Perspectiva del producto**  
`<Describa el contexto y el origen del producto que se especifica en este ERS. Por ejemplo, indique si este producto es una continuación dentro de una familia de productos, un reemplazo de ciertos sistemas existentes o un producto nuevo e independiente. Si el ERS define un componente de un sistema más grande, relacione los requisitos del sistema general con la funcionalidad de este software e identifique las interfaces entre ambos. Puede ser útil incluir un diagrama simple que muestre los componentes principales del sistema general, las interconexiones entre subsistemas y las interfaces externas.>`

`<Ejemplo:>`  
This is a standalone system but integrates with `<External System X>` via `<API/Protocol>`.  

### **2.2 Funcionalidades del producto** 
`<Resuma las principales funcionalidades que contiene el producto o las funciones significativas que realiza o permite realizar al usuario. Los detalles se presentarán en la Sección 3, por lo que aquí solo se necesita un resumen a alto nivel. Organice las funciones de manera que sean comprensibles para cualquier lector del ERS. Suele ser útil una representación visual de los principales grupos de requisitos relacionados y cómo se vinculan entre sí, como un diagrama de flujo de datos de alto nivel o un diagrama de clases.>` 

`<Ejemplo:>`  
- User authentication (OAuth 2.0).  
- Dashboard with real-time analytics.  

### **2.3 Clases y características de usuarios**  
`<Identifique las distintas clases de usuarios que se prevé utilizarán este producto. Las clases de usuarios pueden diferenciarse según la frecuencia de uso, el subconjunto de funciones del producto que utilizan, el nivel de experiencia técnica, los niveles de seguridad o privilegios, el nivel educativo o la experiencia. Describa las características pertinentes de cada clase de usuario. Algunos requisitos pueden aplicarse únicamente a ciertas clases de usuarios. Distinga las clases de usuarios prioritarias de aquellas cuya satisfacción es menos crítica.>`

`<Ejemplo:>`  
| Tipos de usuarios | Características         | Prioridad|  
|------------------ |-------------------------|----------|  
| Admin             | Full system access      | High     |  
| End User          | Limited permissions     | Medium   |  

### **2.4 Entorno operativo**  
`<Describa el entorno en el que funcionará el software, incluyendo la plataforma de hardware, el sistema operativo y sus versiones, y cualquier otro componente o aplicación de software con los que deba coexistir sin inconvenientes.>`

### **2.5 Restricciones de diseño e implementación**  
`<Describa cualquier elemento o cuestión que limite las opciones disponibles para los desarrolladores. Estas pueden incluir: políticas corporativas o normativas; limitaciones de hardware (requisitos de tiempo, memoria); interfaces con otras aplicaciones; tecnologías, herramientas y bases de datos específicas a utilizar; operaciones en paralelo; requisitos de lenguajes de programación; protocolos de comunicación; consideraciones de seguridad; convenciones de diseño o estándares de programación (por ejemplo, si la organización del cliente será responsable del mantenimiento del software entregado).>`

### **2.6 Documentación para el usuario**  
`<Enumere los componentes de la documentación para el usuario (como manuales de usuario, ayudas en línea y tutoriales) que se entregarán junto con el software. Identifique cualquier formato o estándar conocido para la entrega de dicha documentación.>`

### **2.7 Supuestos y dependencias**  
`<Enumere cualquier factor asumido (en contraposición a hechos conocidos) que pueda afectar los requisitos establecidos en este ERS. Estos pueden incluir componentes de terceros o comerciales que se planea utilizar, cuestiones relacionadas con el entorno de desarrollo u operativo, o restricciones. El proyecto podría verse afectado si estos supuestos son incorrectos, no se comparten o cambian. También identifique cualquier dependencia del proyecto con factores externos, como componentes de software que se pretende reutilizar de otro proyecto, a menos que ya estén documentados en otro lugar (por ejemplo, en el documento de visión y alcance o en el plan del proyecto).>`

---

## **3. Características del Sistema**  
`<Esta plantilla ilustra cómo organizar los requisitos funcionales del producto según las características del sistema, es decir, los servicios principales que proporciona el producto. También puede optar por organizar esta sección según los casos de uso, modo de operación, clase de usuario, clase de objeto, jerarquía funcional o una combinación de estos enfoques, lo que tenga más sentido lógico para su producto.>`

### **3.1 Característica del sistema 1**  
`<No escriba literalmente “Característica del Sistema 1”. Indique el nombre de la funcionalidad en pocas palabras.>`

#### **3.1.1 Descripción y prioridad**  
`<Proporcione una breve descripción de la funcionalidad e indique si su prioridad es Alta, Media o Baja. También puede incluir calificaciones específicas de prioridad, como beneficio, penalización, costo y riesgo (cada uno evaluado en una escala relativa del 1 al 9).>` 

#### **3.1.2 Secuencias estímulo/respuesta**  
`<Enumere las secuencias de acciones del usuario y respuestas del sistema que desencadenan el comportamiento definido para esta funcionalidad. Estas secuencias corresponden a los elementos de diálogo asociados con los casos de uso.>` 

#### **3.1.3 Requisitos funcionales**  
`<Enumere los requisitos funcionales detallados asociados con esta funcionalidad. Estas son las capacidades del software que deben estar presentes para que el usuario pueda realizar los servicios proporcionados por la funcionalidad o ejecutar el caso de uso. Incluya cómo debe responder el producto ante condiciones de error previstas o entradas inválidas. Los requisitos deben ser concisos, completos, no ambiguos, verificables y necesarios. Utilice “TBD” (por determinar) como marcador si la información necesaria aún no está disponible.>` 

`<Cada requisito debe identificarse de manera única con un número de secuencia o una etiqueta significativa.>` 
- **REQ-1**: System shall validate credentials against `<Database/API>`.  
- **REQ-2**: Failed attempts trigger a 5-minute lockout.  

### **3.2 Característica del sistema 2 (y así sucesivamente)**  
`<..........>` 

---

## **4. Requisitos de interfaces Externas**  
### **4.1 Interfaces de usuario**  
`<Describa las características lógicas de cada interfaz entre el producto de software y los usuarios. Esto puede incluir imágenes de pantallas de ejemplo, cualquier estándar de GUI o guías de estilo de la familia de productos que se deban seguir, restricciones de diseño de pantalla, botones y funciones estándar (por ejemplo, ayuda) que aparecerán en cada pantalla, atajos de teclado, estándares de visualización de mensajes de error, etc. Defina los componentes del software para los cuales se necesita una interfaz de usuario. Los detalles del diseño de la interfaz de usuario deben ser documentados en una especificación separada de la interfaz de usuario.>` 

`<Example:>`  
- **Login Screen**: Fields for email/password, "Forgot Password" link.  
- **Dashboard**: Responsive layout (support for mobile/desktop).  

### **4.2 Interfaces de Hardware**  
`<Describa las características lógicas y físicas de cada interfaz entre el producto de software y los componentes de hardware del sistema. Esto puede incluir los tipos de dispositivos soportados, la naturaleza de las interacciones de datos y control entre el software y el hardware, y los protocolos de comunicación que se utilizarán.>` 

`<Example:>`  
- Supports barcode scanners (USB HID standard).  

### **4.3 Interfaces de Software**  
`<Describa las conexiones entre este producto y otros componentes específicos de software (nombre y versión), incluyendo bases de datos, sistemas operativos, herramientas, bibliotecas y componentes comerciales integrados. Identifique los elementos de datos o mensajes que entran y salen del sistema y describa el propósito de cada uno. Describa los servicios necesarios y la naturaleza de las comunicaciones. Haga referencia a documentos que describan los protocolos detallados de las interfaces de programación de aplicaciones (API). Identifique los datos que se compartirán entre componentes de software. Si el mecanismo de intercambio de datos debe implementarse de una manera específica (por ejemplo, el uso de un área de datos global en un sistema operativo multitarea), especifique esto como una restricción de implementación.>` 

`<Example:>`  
- Supports barcode scanners (USB HID standard).  

### **4.4 Interfaces de comunicaciones**  
`<Describa los requisitos asociados con cualquier función de comunicación requerida por este producto, incluyendo correo electrónico, navegador web, protocolos de comunicaciones de servidores de red, formularios electrónicos, etc. Defina cualquier formato de mensaje pertinente. Identifique los estándares de comunicación que se utilizarán, como FTP o HTTP. Especifique cualquier cuestión de seguridad o cifrado en las comunicaciones, tasas de transferencia de datos y mecanismos de sincronización.>`  

`<Example:>`  
- Supports barcode scanners (USB HID standard).  

---

## **5. Otros requisitos no funcionales**  
### **5.1 Rendimiento**  
`<Si existen requisitos de rendimiento para el producto en diversas circunstancias, indíquelos aquí y explique su justificativo, para ayudar a los desarrolladores a entender la intención y tomar decisiones de diseño adecuadas. Especifique las relaciones temporales en sistemas de tiempo real. Haga estos requisitos lo más específicos posible. Puede ser necesario definir requisitos de rendimiento para requisitos funcionales o características individuales.>`

`<Example:>`  
- 95% of API responses must be `<500ms` under 1000 concurrent users.  

### **5.2 Seguridad**  
`<Especifique los requisitos relacionados con posibles pérdidas, daños o perjuicios que puedan derivarse del uso del producto. Defina las salvaguardas o acciones que deben adoptarse, así como las acciones que deben evitarse. Remítase a políticas o normativas externas que establezcan cuestiones de seguridad que afecten al diseño o uso del producto. Defina las certificaciones de seguridad que deben cumplirse.>`

`<Example:>`  
- All passwords stored as bcrypt hashes.  

### **5.3 Seguridad y privacidad**  
`<Especifique cualquier requisito relativo a la seguridad o privacidad en el uso del producto o la protección de los datos que éste utilice o genere. Defina los requisitos de autenticación de identidad de los usuarios. Haga referencia a políticas o normativas externas que contengan asuntos de seguridad o privacidad que afecten al producto. Defina las certificaciones de seguridad o privacidad que deben satisfacerse.>`

`<Example:>`  

### **5.4 Atributos de calidad del software**  
`<Especifique cualquier característica de calidad adicional del producto que sea importante tanto para los clientes como para los desarrolladores. Algunas a considerar son: adaptabilidad, disponibilidad, corrección, flexibilidad, interoperabilidad, mantenibilidad, portabilidad, fiabilidad, reutilización, robustez, capacidad de prueba y usabilidad. Redacte estos atributos de forma específica, cuantitativa y verificable cuando sea posible. Al menos, aclare las preferencias relativas entre varios atributos, como facilidad de uso frente a facilidad de aprendizaje.>`

`<Example:>`  

---

## **6. Otros requisitos**  
`<Defina cualquier otro requisito no cubierto en las secciones anteriores del ERS. Esto podría incluir requisitos de bases de datos, requisitos de internacionalización, requerimientos legales, objetivos de reutilización para el proyecto, y otros. Añada cualquier nueva sección que sea pertinente al proyecto.>`  

---

## **Apéndices**  
### **Apéndice A: Glosario**  
`<Example:>`  
- **SSO**: Single Sign-On.  
- **API**: Application Programming Interface.  

### **Apéndice B: Modelos de Análisis**  
- `TBD`: Maximum password length policy.  
