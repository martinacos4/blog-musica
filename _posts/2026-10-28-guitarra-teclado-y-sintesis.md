---
layout: post
title: "Guitarra, teclado y un poco de síntesis"
date: 2026-10-28
resumen: "Cómo uso la guitarra, el teclado MIDI y los sintetizadores virtuales, y lo básico que he aprendido sobre osciladores y la envolvente ADSR."
imagen: /assets/img/formas-de-onda.svg
imagen_alt: "Las cuatro formas de onda básicas: seno, cuadrada, sierra y triangular"
---

En casi todos mis proyectos aparecen tres cosas: la guitarra, el teclado y algún sintetizador virtual. En esta entrada cuento cómo uso cada uno y lo poco que he aprendido de síntesis, que es la parte que más curiosidad me ha dado.

## La guitarra

Es el instrumento con el que me siento más cómodo. La conecto directo a la interfaz y grabo la señal limpia, sin efectos. Después, en la DAW, le pongo un simulador de amplificador. Así puedo cambiar el sonido cuando ya está grabada, sin repetir la toma.

## El teclado

Con el controlador MIDI grabo acordes y melodías. Como lo que queda grabado son notas y no audio, puedo corregir una nota equivocada o cambiar el instrumento después. Lo uso mucho para pianos, bajos y colchones de sonido (pads).

## Los sintetizadores virtuales

Un sintetizador virtual es un plugin que genera el sonido desde cero. Uso los gratuitos, como Vital y Surge XT, y el ReaSynth que viene con Reaper. Todo empieza en el **oscilador**, que produce una onda que se repite. La forma de esa onda define el timbre:

- **Seno:** suave, parecido a un silbido.
- **Cuadrada:** suena hueca, como los videojuegos viejos.
- **Sierra:** brillante y áspera; se usa mucho para bajos y melodías.
- **Triangular:** queda en la mitad, suave pero con algo de brillo.

![Las formas de onda seno, cuadrada, sierra y triangular]({{ '/assets/img/formas-de-onda.svg' | relative_url }})
*Las cuatro formas de onda básicas.*

Después del oscilador viene el filtro, que recorta frecuencias. El más común es el pasabajos, que deja pasar los graves y le quita brillo al sonido.

## La envolvente ADSR

Lo que más me ayudó a entender los sonidos fue la envolvente, que controla cómo cambia el volumen de una nota en el tiempo. Tiene cuatro partes:

- **Ataque (attack):** lo que tarda el sonido en llegar al máximo.
- **Caída (decay):** lo que tarda en bajar hasta el nivel de sostenimiento.
- **Sostenimiento (sustain):** el nivel que se mantiene mientras la tecla siga presionada.
- **Liberación (release):** lo que tarda en apagarse después de soltar la tecla.

![Gráfica de la envolvente ADSR: el volumen sube, baja un poco, se mantiene y cae a cero]({{ '/assets/img/envolvente-adsr.svg' | relative_url }})
*La envolvente ADSR de una nota.*

Con un ataque y una liberación cortos sale un sonido percusivo. Con los dos largos sale un pad que entra y se va despacio.

Mi forma de practicar es sencilla: cargo un preset, lo reviso perilla por perilla y después intento recrearlo partiendo de una onda simple.
