## **Integrantes**
- Erick Martinez
- Sebastian Torrejon
- Ian Meneses


## **Modelo de capas Google Cloud Platform**

![alt text](ModeloGcp.jpeg)


## **Documentacion**


**Implementación RFID**

- TAG RFID: Etiqueta física adherida al material de la biblioteca que permite a esta solución almacenar información sobre los este, con un identificador único y sus características. Es posible leer esta información a través de un lector de RFID.

- TAG RFID Reader: Lector físico de etiquetas RFID. Serán utilizados dentro de la biblioteca para leer las etiquetas al realizar los prestamos de material.

- Filtering Aggregation: Componente de middleware encargado de filtrar y empaquetar la información leída por el Lector RFID.

- Data Management: Componente de middleware encargado de organizar la salida de datos hacia el sistema Cloud para su procesamiento.

**Vista**

- Firebase Hosting: Permite acceder a la aplicación basada en React, accediendo a contenidos de forma segura a través de un certificado SSL integrado al servicio de hosting, otorgados a cada dominio y subdominio hosteado.

- React.js: Permite flexibilidad y facil integración con diferentes tecnologías, en caso de cambiar el proveedor de servicios en el futuro.

**Servicios**

- Cloud Load Balancing: Permite la distribución de la carga entre diferentes nodos del servicio para asegurar alta disponibilidad y baja latencia.

- Cloud Run: Permite ejecutar aplicaciones en cualquier lenguaje de programación, a la vez de librerías de cualquier sistema operativo, otorgando gran flexibilidad al desarrollo. El pago del servicio es por uso, permitiendo escalarlo a medida de lo requerido. Considerando que existen métricas y metas específicas en este caso (40.000 usuarios activos en dos años).

- Logging: Registra la actividad dentro de los servicios del sistema, lo que se utilizará para facilitar la auditoría del proyecto.

- Dataflow: Orquesta los servicios del sistema, haciendose cargo de la gestión de devolución y sus respectivas alertas tempranas y tardías.

**Seguridad**

- Firebase Authentication: Permite el registro y autenticación de los usuarios de manera segura, con encriptación SHA256. Otorga la posibilidad de autenticación con huella digital, la que será utilizada dentro de la biblioteca para permitir el registro final y la ejecución de los préstamos solicitados por los usuarios.

- Cloud Armor: Impide ataques de sobrecarga, permitiendo el funcionamiento continuo de la solución.

**Almacenamiento**

- Firestore: Permite el almacenamiento de los datos de usuario, tales como nombre, dirección, teléfono, etc. Más relevante aún, permite almacenar documentos de préstamo y devolución para cada usuario, separando los datos de la biblioteca de aquellos de los usuarios.

- Cloud Storage: Permite almacenar objetos con atributos, lo que facilita el ingreso de documentos, archivos, audios, etc. con formatos estandarizados.
