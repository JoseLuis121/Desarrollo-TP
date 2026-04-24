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
Sistema de gestión de turnos de un consultorio odontológico centralizado en el manejo de pacientes y reservas en una interfaz simple e intuitiva. Abarca cada etapa del servicio, desde que el paciente realiza la reserva hasta que se realiza la consulta.

### Modelo
https://app.diagrams.net/#G1z93UDN1OUiycHQpA3MJCTfX8HWOygKV8#%7B%22pageId%22%3A%22lv6PCzvnAAI5jWWzNXJ_%22%7D


## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Practica<br>2. CRUD Paciente<br>3. CRUD Odontologo<br>4. CRUD Turno|
|CRUD dependiente|1. CRUD Consulta {depende de} CRUD Paciente y CRUD Odontologo<br>2. CRUD Reserva {depende de} CRUD Consuta|
|Listado<br>+<br>detalle| 1. Listado de odontologos filtrado por obra social, muestra nombre del odontologo y sus especialidades => detalle  muestra datos completos del odontologo<br>2. Listado de los próximos turnos disponibles por odontólogo => Detalle: muestra Fecha y hora y duración.<br>3. Listado de Mutuales disponibles => Detalle: Muestra nombres de las mutuales con sus respectivos planes<br>4. Listado de reservas => Detalle: Se le muestra al paciente todas las reservas que tiene, con su respectiva fecha de creacion,su estado, fecha y hora de consulta, nombre y apellido del odontologo, nombre y apellido del paciente y cualquier observacion pertinente<br>5. Listado de practicas realizadas en una consulta => detalle: Al terminar la consulta se guardan todas las practicas realizadas, quedando disponibles el codigo, el valor y el detalle de cada una, asi como el subtotal de la consulta ya calculado|
|CUU/Epic|1. Reservar un turno con un Odontolo <br>2. Enviar recordatorio de turno al Paciente <br>3. Cancelacion de reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Practica<br>2. CRUD Paciente<br>3. CRUD Odontologo<br>4. CRUD Turno<br>5. CRUD precio<br>6. CRUD Reserva<br>7. CRUD Mutual<br>8. CRUD Diente <br>9. CRUD Cara <br>10. CRUD Consulta |
|CUU/Epic|1. Reservar un turno con un Odontolo<br>2. Enviar recordatorio de turno al paciente<br>3. Cancelacion de turno<br>4. Calcular cobro de la atencion al paciente<br>5. Actualizar el precio de las practica<br>6. Cambio de turno|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Historial del Paciente muestra turnos atendidos, fecha turno y practicas realizadas <br>2. Reservas filtradas por estado muestra fecha reserva y datos del paciente<br>3. Odontologos filtrados por Practicas <br> |
|CUU/Epic|1. Realizar facturacion del cobro al paciente<br>2. Cancelación de reserva<br>3.Cambio de Mutual<br>4.Registrar practica realizada|
|Otros|1. Solicitud de cambio de turno|


Listado de turnos filtrado por rango de fecha, muestra codigo turno, fecha turno, estado del turno y nombre del paciente => detalle muestra datos completos del paciente, odontologo y practicas realizadas


