# Sistema de Gestión de Playa de Estacionamiento

## Requisitos Funcionales

1. **Mostrar Distribución de Lugares y Disponibilidad:**
   - **Distribución:** Mostrar el diseño del estacionamiento con la disponibilidad de los lugares. Utiliza diferentes íconos para representar los distintos tipos de vehículos:
     - **Lugar Disponible:** Mostrar un punto para los lugares disponibles.
     - **Lugares Ocupados:** Utiliza íconos de Bootstrap para mostrar autos, camionetas o motocicletas en los lugares ocupados.
   
2. **Formulario de Ingreso de Vehículo:**
   - **Campos del Formulario:**
     - **Marca** (Requerido): Proporcionar una lista predefinida de marcas.
     - **Modelo** (Opcional): Mínimo de 3 caracteres.
     - **Dominio Nuevo** (Booleano): Indica si el vehículo tiene un dominio nuevo.
     - **Dominio** (Requerido): La validación del dominio depende de si es un dominio nuevo (máximo 7 caracteres) o viejo (máximo 6 caracteres).
     - **Tipo de Vehículo**: Seleccionar de un enumerado con valores: moto, auto, camioneta.
     - **Fecha y Hora de Ingreso** (Requerido): Debe ser proporcionada.
   - **Validación:**
     - Mostrar errores solo después de que el usuario haya interactuado con los controles del formulario.
     - No marcar los campos como inválidos hasta que el formulario haya sido enviado al menos una vez.
   
3. **Visualización de Una Pantalla a la Vez:**
   - **Visibilidad del Formulario y del Mapa:**
     - Mostrar solo el formulario o el mapa, pero no ambos simultáneamente.
     - El formulario debe estar oculto mientras se visualiza el mapa y viceversa.
     - El usuario debe poder alternar entre ver el formulario y el mapa.
   
4. **Asignación de Lugares de Estacionamiento:**
   - **Tipo de Vehículo y Asignación de Lugares:**
     - Asignar los lugares de estacionamiento según el tipo de vehículo (cada plaza tiene 8 lugares y puede recibir varios vehiculos mientras haya espacio disponible):
       - **Camioneta:** Requiere 8 lugares.
       - **Auto:** Requiere 4 lugares.
       - **Motocicleta:** Requiere 1 lugar.
   - **Actualización de Disponibilidad:**
     - Al ingresar un vehículo, buscar un lugar disponible según el tipo de vehículo y actualizar la visualización del estacionamiento en consecuencia.
   
5. **Visualización de los Lugares:**
   - **Lugares Ocupados y Disponibles:**
     - **Ocupados:** Mostrar los lugares en rojo.
     - **Disponibles:** Mostrar los lugares en verde.
   - **Claridad:** Proporcionar indicadores visuales claros para ayudar al encargado de la playa de estacionamiento a identificar fácilmente los lugares ocupados y disponibles.

## Consideraciones

- **Estructura de Archivos:** Organizar los archivos en directorios según sus responsabilidades.
- **Estilo:** Respetar los estilos proporcionados utilizando el framework (Bootstrap).
- **Idioma:** Escribir todo el código y los comentarios en inglés, pero los mensajes dirigidos al usuario (etiquetas, alertas, validaciones, etc.) deben estar en el idioma del usuario.
- **Archivos Proporcionados:** No modificar ningún archivo proporcionado.
- **SPA** La pagina nunca debe ser recargada ateniendose al mecanismo proporcionado por las aplicaciones de una sola página.

## MockUps
![image](https://github.com/user-attachments/assets/3279d9de-f4ea-45fc-895d-95f3f488a7f8)
![image](https://github.com/user-attachments/assets/944eb0ed-1347-43cc-afa8-460e5f5faa20)

## Ejemplos: 
A continuación se presentan algunos ejemplos visuales indicando como debería quedar la disponibilidad de lugares al ingresar un nuevo vehiculo:

**En caso de agregar una moto:**
![image](https://github.com/user-attachments/assets/99b6558d-7f39-48fb-a381-a19ee1c4f4ba)

**En caso de agregar un auto:**
![image](https://github.com/user-attachments/assets/9171d8a9-099f-4c7e-a747-dda5452357b2)

**En caso de agregar una camioneta:**
![image](https://github.com/user-attachments/assets/722bef2b-74b3-40c2-a5bd-3f63f299677a)

## Rubrica:
- Registro ingreso (3)
- Validaciones (2)
- Mapa playa estacionamiento (3)
- Navegación componentes (1)
- Estilos (1)
