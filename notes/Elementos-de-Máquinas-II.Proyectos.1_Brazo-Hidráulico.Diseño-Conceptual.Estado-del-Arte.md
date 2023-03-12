---
id: irxp89zxks86bygpmxfnrfu
title: Estado del Arte
desc: ''
updated: 1677620959331
created: 1677194757035
---

A continuación se especificarán los subsistemas de los que está compuesta la máquina, junto con tres diseños ya existentes, o diseños que pueden implementarse.

## Mecanismo de giro

1. Activación por hidráulico anclado al soporte y al eje.   
   ![](/assets/images/2023-02-23-18-31-29.png)

2. Implementación de engranes en el eje del brazo y en el eje de un motor eléctrico anclado al soporte.   
   ![](/assets/images/2023-02-23-18-42-51.png)  

   ![](/assets/images/2023-02-23-18-43-15.png)

3. Acople directo del eje a un motor eléctrico.   
   ![](/assets/images/2023-02-23-18-43-39.png)
   
## Actuadores

1. **Hidráulica con control manual:** Utilizar jeringas para efectuar el movimiento del brazo con control manual.
   ![](/assets/images/2023-02-28-00-28-09.png)
2. **Movimiento lineal:** Utilizar Arduino y relés para controlar actuadores lineales que permitan el movimiento del brazo.    
   ![](/assets/images/2023-02-28-00-27-25.png)
3. **Hidráulica con control eléctrico:** Utilizar jeringas que, con ayuda de una o más bombas, y control de Arduino, controlar el movimiento del brazo.  
   Como inspiración, ver [este video](https://www.youtube.com/watch?v=dqqWjWa2paQ) y [este video](https://www.youtube.com/watch?v=dZBua0wiV2g&list=WL&index=1)
   - Ver [bomba](https://didacticaselectronicas.com/~didactic/index.php/elementos-electromecanicos/motores-y-solenoides-1/bombas-y-solenoides-1/para-liquidos/mini-bomba-sumergible-100l-h-bom-sumer-01-mini-bombas-mini-de-aire-flujo-de-aire-sumergibles-detail)
   - Ver [bomba peristáltica](https://didacticaselectronicas.com/index.php/elementos-electromecanicos/motores-y-solenoides-1/bombas-y-solenoides-1/para-liquidos/mini-bombas-mini-de-flujo-de-agua-bombas-peristaltica-peristalticas-de-agua-liquido-de-2l-2-litros-detail)
   
4. **Neumática con control eléctrico:** Utilizar pistones neumáticos (o jeringas) que, con ayuda de uno o más compresores, e implementación de Arduino, controlar el movimiento del brazo.   
   Como inspiración, ver [este video](https://www.youtube.com/watch?v=iXNNjtK5hp8)
   - Ver [compresor](https://didacticaselectronicas.com/~didactic/index.php/elementos-electromecanicos/motores-y-solenoides-1/bombas-y-solenoides-1/para-aire/mini-bomba-de-aire-3v-0-5l-min-mini-bombas-mini-de-aire-flujo-de-aires-para-presi%C3%B3n-arterial-esfigoman%C3%B3metros-de-3v-detail)
   - Ver [manguera](https://didacticaselectronicas.com/~didactic/index.php/otros/nebulizador-rociador-formador-rociadores-de-niebla-para-jardines-jard%C3%ADn-6-metros-6m-85948-manguera-neumatica-aire-plastica-tubo-detail)
   - Ver [válvula](https://www.youtube.com/watch?v=osxvM_Y8xn0&t=0s)
   - Ver [pistón](https://www.youtube.com/watch?v=L3ZuC3Bu2vk&t=0s)
   - Ver [compresor](https://didacticaselectronicas.com/index.php/elementos-electromecanicos/motores-y-solenoides-1/bombas-y-solenoides-1/para-aire/mini-bomba-de-aire-y-de-vacio-2-5lpm-bombas-mini-de-flujo-de-aire-vacio-para-presi%C3%B3n-arterial-esfigomanometros-de-2-5l-de-5v-bombas-370-detail)
   - Ver [solenoide](https://didacticaselectronicas.com/index.php/elementos-electromecanicos/motores-y-solenoides-1/bombas-y-solenoides-1/valvula-solenoide/v%C3%A1lvula-solenoide-3vdc,-75ma-valvulas-bombas-solenoides-val-sol%C3%A9-3v-2-de-aire-de-3v-detail)


## Mecanismo de movimiento vertical

## Pinza

## Mecanismo de rotación de pinza

