Propuesta TP DSW

## Grupo
### Integrantes
* 54443 - Carestia, Juan Andrés
* 52335 - Merad , Juan Segundo
* 53784 - Fernandez , Alejo
* 54429 - Gorandi Marmol, Jose Luis
  

### Repositorios
  https://github.com/AlejoFernandezAlcantara/Desarrollo-TP



## Tema
### Descripción
Sistema de gestión de turnos en un consultorio odontologico que se centraliza en  el manejo de pacientes, consultas y especialidades en una interfaz simple e intuitiva. Buscando agilizar cada etapa del servicio, desde que el paciente solicita el turno hasta que se realiza la atencion, mejorando tanto el manejo interno del consultorio como la experiencia del paciente.

### Modelo
https://app.diagrams.net/?src=about#G1ykwDR5jfFqt6A9WPDxQebTJC06Fh3MzD#%7B%22pageId%22%3A%22U16Np_kju9VaJ5zfGIP3%22%7D


## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Practica<br>2. CRUD Estado turno<br>3. CRUD Tipo Paciente<br>4. CRUD Especialidad|
|CRUD dependiente|1. CRUD Turno {depende de} CRUD Tipo Practica<br>2. CRUD Cliente {depende de} CRUD Tipo Paciente<br>3. CRUD Odontologo {depende de} CRUD Especialidad|
|Listado<br>+<br>detalle| 1. Listado de odontologos filtrado por especialidad, muestra nombre del odontologo, sus especialidades y practicas=> detalle  muestra datos completos del odontologo y obras sociales que trabaja <br> 2. Listado de turnos filtrado por rango de fecha, muestra practica realizada, fecha turno, estado del turno y nombre del paciente => detalle muestra datos completos del turno, del paciente y odontologo|
|CUU/Epic|1. Reservar un turno para una especialidad<br>2. Enviar recordatorio de turno al Paciente<br>3. Cancelacion de turno|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Practica<br>2. CRUD Estado Turno<br>3. CRUD Tipo Paciente<br>4. CRUD Especialidad<br>5. CRUD Consultorio<br>6. CRUD Odontologo<br>7. CRUD Paciente<br>8. CRUD Practica|
|CUU/Epic|1. Reservar un turno para una especialidad<br>2. Enviar recordatorio de turno al paciente<br>3. Cancelacion de turno|<br>4. Calcular cobro de la atencion al paciente<br>5. Realizar facturacion del cobro al paciente|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
