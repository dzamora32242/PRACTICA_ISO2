===============================================================================

&#x20;          LISTADO DE TAREAS Y MODIFICACIONES POR CASO DE USO (CU)

===============================================================================



\[CU.001] - REGISTRO / IDENTIFICACIÓN

&#x20;   - \[ ] Gestión de Correo: El sistema debe enviar el correo desde este CU.

&#x20;   - \[ ] Añadir ID de Usuario: Incorporar el atributo 'id' al diagrama de paquetes.

&#x20;   - \[ ] Trazabilidad: Asegurar que el ID se asocie a compras para auditoría.



\[CU.002] - VERIFICACIÓN Y CAMBIO DE ESTADO

&#x20;   - \[ ] Flujo de entrada: Inicia cuando ya se tiene el correo (enviado por CU.001).

&#x20;   - \[ ] Funcionalidad: Buscar usuario y cambiar su estado.

&#x20;   - \[ ] REVISIÓN: Revisar el caso de uso por completo.



\[CU.003] - GESTIÓN DE PERFIL

&#x20;   - \[ ] Restricción de Datos: NO pedir ni permitir cambiar el DNI.

&#x20;   - \[ ] Validación (Paso 3): Añadir excepción para verificar formato correcto.



\[CU.004] - DARSE DE BAJA

&#x20;   - \[ ] Variable de Confirmación: Añadir booleano 'confirmacion' en los paquetes.

&#x20;   - \[ ] Interfaz de Usuario: Mostrar mensaje de "operación cancelada" por pantalla.

&#x20;   - \[ ] REVISIÓN: Revisar el caso de uso entero.

&#x20;   - \[!] NOTA (ZAPA): Preguntar a Luis Enrique sobre la lógica de este CU.



\[CU.005] - ALTA DE VIDEOJUEGO

&#x20;   - \[ ] Excepción (Paso 3): 

&#x20;       - Verificar que el nombre de la empresa existe.

&#x20;       - Verificar que el nombre del videojuego no esté duplicado.

&#x20;       - ELIMINAR comprobación de existencia del género.

&#x20;   - \[ ] Especificación: Solicitar 'Precio Base' y 'Fecha de Lanzamiento'.

&#x20;   - \[ ] Atributo Disponibilidad: Añadir booleano 'disponible' en paquetes y Create.

&#x20;       - Lógica: Si 'Fecha de lanzamiento' <= Hoy -> disponible = True.

&#x20;   - \[ ] Atributo Valoración: Añadir 'valoracionMedia' en Create.

&#x20;       - Lógica: Implementar mediante autoestímulo para cálculo posterior.

&#x20;   - \[ ] Añadir ID: Se ha incorporado el ID a la entidad videojuego.

&#x20;   - \[!] NOTA: Consultar a Luis Enrique qué hacer finalmente con el género.



\[CU.006] - GESTIÓN FINANCIERA

&#x20;   - \[ ] Diseño: Añadir 'IUEntidadFinanciera' en el diagrama de clases de diseño.

&#x20;   - \[ ] Integración: Actualizar la interfaz en todos los paquetes relacionados.



\[CU.007] - POR DEFINIR

&#x20;   - \[!] BLOQUEO: Hablar con Enrique para definir la funcionalidad.



\[CU.012] - DESCARGAS

&#x20;   - \[ ] Reestructuración: Rehacer de cero (está mal planteado).

&#x20;   - \[ ] Lógica de Selección: Decidir si el usuario selecciona el juego o si el sistema lo asume.

&#x20;   - \[ ] Actores: Incluir el 'Sistema de Descargas' como actor externo en los diagramas.



\[CU.013] - POR DEFINIR

&#x20;   - \[ ] Reestructuración: Rehacer el caso de uso por completo.



\[CU.014] - GENERACIÓN DE ENTIDADES

&#x20;   - \[ ] Automatización: El ID no se pide al usuario, lo genera el sistema automáticamente.



===============================================================================

&#x20;                   NOTAS GENERALES Y ARQUITECTURA

===============================================================================



\[ ] PROPUESTA: Crear nuevo CU "Publicar Videojuego".

&#x20;   - Condición: Se activa si el atributo 'disponible' es True.



\[ ] ORGANIZACIÓN DE PAQUETES:

&#x20;   - Evaluar creación de paquete: "Gestión Reseñas".

&#x20;   - Evaluar creación de paquete: "Gestión Desarrolladoras".



\[ ] DIAGRAMAS:

&#x20;   - Incluir ID de usuario y videojuego en todos los diagramas de paquetes.

&#x20;   - Incluir IC del Sistema de Descargas y actores externos.



\[!] TAREAS PENDIENTES DE REVISIÓN (ZAPA):

&#x20;   - Dar una vuelta al concepto de "Dar de baja" antes de cerrar CU.004.

===============================================================================usuario; debe ser generado automáticamente por el sistema.

