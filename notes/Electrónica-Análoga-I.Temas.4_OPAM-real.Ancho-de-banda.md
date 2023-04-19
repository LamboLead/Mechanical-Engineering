---
id: mcvkdvby4em6bvc9i6iqgzr
title: Limitación de ancho de banda
desc: ''
updated: 1680986217062
created: 1680982004213
---

El **ancho de banda** es la máxima frecuencia de una onda de entrada $V_{in}$ que un amplificador operacional puede procesar. Esta depende del amplificador en cuestión.

**Ancho de banda de ganancia unitaria $BW_1$**: Es el ancho de banda cuando el amplificador está conectado en una configuración con ganancia igual a 1.

## Simulación

Para simular una limitación de ancho de banda se utiliza un _Op. Amp (Level 1)_

### Diagrama de bode

Se quiere realizar un diagrama de bode de un amplificador operacional. Se debe realizar un análisis en frecuencia.

#### Elementos
**AC sweep:** Toma una entrada y aplica una serie de señales sinusoidales a diferente frecuencia, y por lo tanto mide el cambio en la amplitud y el cambio en la fase de la salida respecto a la entrada.   
**AC Sweep Probe:** Permite realizar un análisis frecuencial de un circuito.

#### Parámetros de AC Sweep
**Start Frequency:** Frecuencia de inicio del análisis  
**End Frequency:** Frecuencia final del análisis  
**No. of Points:** Número de frecuencias que la simulación va a realizar entre _Start frequency_ y _End frequency_.   
**Source Name:** Onda sinusoidal sobre la cual aplicar el AC sweep.   
**Start Amplitude:** Amplitud inicial sobre la cual iniciar el análisis.   
**End Amplitude:** Amplitud final sobre la cual terminar el análisis.
**Freq. for Extra Points:** Frecuencia adicional a la cual calcular la ganancia del amplificador.

![](/assets/images/2023-04-08-15-36-45.png)