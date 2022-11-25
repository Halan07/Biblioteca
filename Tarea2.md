## **Integrantes**
- Erick Martinez
- Sebastian Torrejon
- Ian Meneses


## **Modelo de capas Google Cloud Platform**

![alt text](ImagenCloud.png)


## **Documentacion**

- Firebase Hosting: Permite acceder a la aplicación basada en React, accediendo a contenidos de forma segura a través de un certificado SSL integrado al servicio de hosting, otorgados a cada dominio y subdominio hosteado.

- React.js: Permite flexibilidad y facil integración con diferentes tecnologías, en caso de cambiar el proveedor de servicios en el futuro.

- Cloud Load Balancing: Permite la distribución de la carga en servidor, distribuyendola entre diferentes nodos para asegurar alta disponibilidad y baja latencia.

- Cloud Armor: Impide ataques contra el componente Cloud Load Balancing, permitiendo el funcionamiento continuo de la solución.

- Cloud Run: Permite ejecutar aplicaciones en cualquier lenguaje de programación, a la vez de librerías de cualquier sistema operativo, otorgando gran flexibilidad al desarrollo. El pago por servicio es por uso, lo que permite escalar el servicio a medida de lo requerido, considerando que existen métricas y metas específicas en este caso.

- Logging: Registra la actividad dentro de los servicios del sistema, que se utilizará para facilitar la auditoría del proyecto.

- Dataflow: Orquesta los servicios del sistema, autoescalando los servicios adaptando el alcance a la demanda en tiempo real.

- Firebase Authentication: Permite el registro y autenticación de los usuarios de manera segura, con encriptación local. Otorga la posibilidad de autenticación con huella digital, la que será utilizada dentro de la biblioteca para permitir el registro final y la ejecución de los préstamos solicitados por los usuarios.

- Firestore: Permite el almacenamiento de los datos de los usuarios, tales como nombre, dirección, teléfono, etc. Más relevante aún, permite generar documentos de préstamo y devolución para cada usuario, separando los datos de la biblioteca de aquellos de los usuarios.

- Cloud Storage: Permite almacenar objetos con atributos, lo que facilita el ingreso de documentos, archivos, audios, etc. con formatos estandarizados.
