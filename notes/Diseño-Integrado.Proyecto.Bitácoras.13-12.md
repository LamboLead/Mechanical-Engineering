---
id: 6cd5c4qwtg6gvsbuj5lk378
title: 6. Revisión de diseño conceptual (13 dic)
desc: ''
updated: 1734203783037
created: 1734201517165
---

**Fecha:** 13 de dic. de 2024.   
**Hora:** 9:00.   
**Lugar:** Salón de profesores - Bloque 04.

## Resumen
Se tuvo una reunión con el profesor, y se le mostraron: Árbol de problemas y objetivos, análisis funcional (caja transparente), y PDS. Se recibieron comentarios al respecto, que están documentados en la sección de **Contenido** de este documento.

---

## Objetivo
- Dar a conocer los avances del proyecto
- Recibir comentarios del profesor para refinar y definir completamente los requerimientos del cliente, problemas a resolver y objetivos a alcanzar. 

## Contenido

A continuación se muestran comentarios del profesor respecto a tal o cual entregable:

**Árbol de problemas y árbol de objetivos**

- En el título del problema, el término 'Limitación local' podría no ser correcto, ya que restringir el problema a algo 'local' quiere decir que externamente este problema ya fue resuelto. Si esto es un problema a nivel mundial, es necesario agregarlo o darlo a entender en el título.
- Agregar de una vez que el miembro a tratar es el de rodilla.
- En el árbol falta todo lo relacionado con el fortalecimiento del miembro opuesto.
- El almacenamiento de la información debe tenerse en cuenta, bien sea porque la máquina mismta guarda los datos de cada terapia, o porque esta información puede ser exportada para su almacenamiento externamente.
- La electromiografía _debe_ estar integrada dentro del dispositivo para que, al mismo tiempo que se realiza la sesión de diagnóstico/terapia, se muestren los músculos siendo activados. Por lo tanto, debe existir también un módulo que procese los resultados de la electromiografía y entregue un reporte completo al profesional de la salud.

**Caja transparente**

- A la máquina no sólo va a entrar el miembro espástico, ¿cómo este paciente será acomodado en la máquina para sus sesiones? Falta agregar el subsistema que soporte al paciente.
- Incluir en las señales de entrada, la configuración de tiempo y repeticiones.
- Incluir los subsistemas que brindan redundancia a las partes más críticas de la máquina (aquellas que pueden ocasionar perjuicios contra el paciente o el profesional de la salud), incluyendo señales de entrada de parada de emergencia, por ejemplo.
- En las señales de salida, incluir señales de inicio, finalización, alerta, etc.

**PDS**

- Incluir todos los comentarios y requerimientos del profesor.
- Falta definir requerimientos de costo objetivo (#23), vida útil (#21) y disposición final (#31)
- Requerimiento #14: ¿Cualquier tipo de cuerpo? Debe especificarse más este estándar. Además, hay que tener en cuenta que los pacientes pueden sufrir de espasticidad en otros miembros de su cuerpo, por lo que la máquina debe también acomodarse a estos casos.
- Requerimiento #15: ¿Se producirá sólo un prototipo? El diseño ya debe tener en cuenta una producción en masa.
- Requerimeinto #36: Debe documentarse también un programa de entrenamiento de los profesionales en el uso de la máquina.

## Tareas

Para el domingo 15 de diciembre, completar cada una de las partes de la matriz morfológica, para que en una reunión ese mismo día o posterior se empiece a formular conceptos.

## Asistentes
- Juan Camilo Rengifo
- Jorge Andrés Montoya
- Daniel Hernández (virtual)
- Juan David López