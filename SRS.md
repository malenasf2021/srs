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
### **3.1 Feature 1: User Authentication**  
#### **3.1.1 Description & Priority**  
`[High]` Allows users to log in via email or SSO.  

#### **3.1.2 Functional Requirements**  
- **REQ-1**: System shall validate credentials against `<Database/API>`.  
- **REQ-2**: Failed attempts trigger a 5-minute lockout.  

---

## **4. Requisitos de interfaces Externas**  
### **4.1 User Interfaces**  
`<Example:>`  
- **Login Screen**: Fields for email/password, "Forgot Password" link.  
- **Dashboard**: Responsive layout (support for mobile/desktop).  

### **4.2 Hardware Interfaces**  
`<Example:>`  
- Supports barcode scanners (USB HID standard).  

---

## **5. Otros requisitos no funcionales**  
### **5.1 Performance**  
`<Example:>`  
- 95% of API responses must be `<500ms` under 1000 concurrent users.  

### **5.2 Security**  
`<Example:>`  
- All passwords stored as bcrypt hashes.  

---

## **Apéndices**  
### **Apéndice A: Glosario**  
`<Example:>`  
- **SSO**: Single Sign-On.  
- **API**: Application Programming Interface.  

### **Apéndice B: Modelos de Análisis**  
- `TBD`: Maximum password length policy.  
