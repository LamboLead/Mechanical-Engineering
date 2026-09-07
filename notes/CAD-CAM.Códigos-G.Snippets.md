---
id: 6t5oyect767djkhhc6puap5
title: Bloques de código
desc: ''
updated: 1708662051687
created: 1708634668672
---

# Bloques de código

**Inicio seguro:** Realiza un inicio seguro del proceso de mecanizado, eligiendo parámetros de coordenadas, cancelando ciclos fijos y compensaciones, eligiendo herramienta

```gcode
  G17 (Plano XY)
  G54 (Coordenadas de trabajo 1)
  G21 (Milímetros)
  G91 (Coordenadas incrementales)
  G32 (Posición segura en Z)
  G80 (Cancelación de ciclos fijos)
  G40 (Cancelación de compensación de herramienta)
  T1 M6 (cambio a herramienta 1)
```

**Salida segura:** Realiza una salida segura del programa
```gcode
  G32
  M05 (Paro de rotación del husillo)
  M30 (Finalización segura)
```