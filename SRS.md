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
### **2.1 Product Perspective**  
`<Example:>`  
This is a standalone system but integrates with `<External System X>` via `<API/Protocol>`.  

### **2.2 Funcionalidades del producto**  
`<List major features in bullet points. Example:>`  
- User authentication (OAuth 2.0).  
- Dashboard with real-time analytics.  

### **2.3 Clases y características de usuarios**  
`<Example:>`  
| User Class       | Characteristics          | Priority |  
|------------------|--------------------------|----------|  
| Admin            | Full system access       | High     |  
| End User         | Limited permissions      | Medium   |  

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
