---
id: ylykqixgboiy0kqqiv46ipp
title: Ideas
desc: ''
updated: 1684347326884
created: 1684342361073
---

### Subsistema de rotación
- El eje hueco y engranaje conducido pueden imprimirse en 3D.

### Subsistema de elevación
- Se podría implementar el servomotor directamente como el elemento de giro, en vez de las ruedas dentadas (como se muestra en la figura). Sin embargo, al implementar las ruedas se puede aumentar el torque y por lo tanto, se requeriría de un servo menos potente.  
  ![](/assets/images/2023-05-17-11-54-48.png)

- Puede implentarse un [soporte ya existente](https://www.didacticaselectronicas.com/index.php/robotica/componentes-mecanicos/pan-tilt-bracket-nylon-sistemas-soportes-brackets-de-para-inclinaci%C3%B3n-giro-rotaci%C3%B3n-pan-tilt-para-servomotores-servo-motores-detail)  
  ![](/assets/images/2023-05-17-12-02-05.png)
  

### Subsistema de lanzamiento
- Puede implementarse el mecanismo de auto-ajuste para las ruedas.  
  ¿Cómo funciona?

  La rueda [1] gira por acción del motor. A medida que esta rueda gira, unos contrapesos [4] acoplados a unas ruedas pequeñas [5] se abren y hacen contacto con las paredes internas de un piñón [2]. El contacto entre las ruedas de los contrapesos y las paredes del piñón vencen la fuerza de restitución ejercida por el resorte de torsión [5], facilitando el movimiento vertical hacia abajo de todo el ensamblaje, a medida que el piñón gira y hace contacto con la cremallera fija [3]. La restitución se da gracias a la acción del resorte de torsión, elevando el ensamblaje.

### Subsistema eléctrico y de control
- Se puede utilizar una fuente de poder de computador para energizar el circuito.