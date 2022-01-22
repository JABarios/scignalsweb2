---
id: "0006"
title: "Recording brain signals with Signalino"
date: 2019-07-21T15:45:23+02:00
draft: false
image : "images/blog/1_600.jpg"
bg_image: "images/mano_cerebro2.jpg"
categories: ["Projects"]
tags: ["Neuromonitoring","Technology"]
description: "this is meta description"
summary: "Signalino, a signal recorder"
description: "Signalino, a signal recorder"
author:
---

## Introducción

En Signalino somos makers desde el principio, y apoyamos la
Movimiento Do It Yourself (DIY), trabajo en equipo, obtención y producción
conocimiento en comunidad. Creemos en un cambio de mentalidad que ayude
compartir ideas, proyectos y desarrollarlos juntos. Esta es la razón por
Signalino desarrolla herramientas que permiten a todos los "makers" impulsar sus
ideas y sacarlas de los cajones. Si quieres una buena presentación
al concepto fab lab, [aquí tenéis uno (de la UA)](http://fablab.ua.es/que-es-fab-lab/).


Las bioseñales, como lo son EEG, EMG y ECG, son un gran recurso para la investigación.
en fisiología: monitorización de la salud o del ejercicio, neurofeedback o EEG
entrenamiento de biorretroalimentación, experimentos con interfaces cerebro-computadora o
simplemente quiere echar un vistazo a su cerebro, corazón o músculos en el trabajo.

Lamentablemente, los dispositivos comerciales de EEG/ECG suelen ser demasiado caros para
Conviértase en una herramienta o juguete para aficionados. Nuestra respuesta es Signalino: hemos desarrollado software y hardware para
dispositivos bioamplificadores de bricolaje disponibles de forma gratuita (como en GPL).


## Nuestra solución: un escudo Arduino

![artículo-img-centrado](/img/blog/0001/EEG2_600.png)

Signalino Shield es una poderosa herramienta de código abierto para aquellos que quieren
registrar bioseñales y recopilar datos para poner en marcha sus proyectos. Para esto
motivo, alentamos a los usuarios de Signalino a compartir con nosotros sus ideas y
proyectos Pertenecemos a la comunidad abierta y nos encantaría ver una fuerte
comunidad creciendo alrededor de algunos de nuestros productos.

{{< youtube O9Kai4d3IyU >}}

[La placa principal de Signalino](http://www.signalino.com/products) depende
en Arduino. La placa OpenBCI de 32 bits es un escudo para Arduino-Due de 32 bits
lo que lo convierte en un impresionante amplificador de bioseñales de 8 canales.

![articulo-img](/images/blog/signalino_prototipo_600.jpg)

Es una plataforma de desarrollo de Hardware para dispositivos médicos y eHealth
aplicaciones a todos aquellos desarrolladores, investigadores y fabricantes de hardware
que necesitan leer señales biométricas. Es un kit móvil que mide ECG
y EEG:**[ EEG/ECG Shield de código abierto para Arduino-Due 32bit Biosignal
Kit Placa Amplificador (8 canales)](http://www.signalino.com/tienda/). **

Signalino está dirigido a aficionados que deseen experimentar con
bioseñales. Y, si eres un profesional en cualquiera de los campos de la electrónica,
neurofeedback, desarrollo de software, etc., por supuesto, eres bienvenido a
Únete a nuestra comunidad.

Todo lo que necesitas es un arduino Due, un cable USB con un conector tipo C y
algunos electrodos, cuyo número depende de la configuración: dos para cada
canal bipolar o uno para cada monopolar con referencia a algunos comunes
electrodo y 1 electrodo pasivo para DRL (los electrodos se venden
por separado). Compra uno de nuestros kits por 199€, descarga el software y
estas grabando!

{{< youtube NhLkvW6aybU >}}


#<http://www.signalino.com/wp-content/uploads/2016/12/Signalino-Test1.mp4>

<!---
%<div class="youtube-container">
%            <iframe src="http://www.signalino.com/wp-content/uploads/2016/12/Signalino-Test1.mp4" frameborder="0" allowfullscreen></iframe>
%          </div>
-->
## Descripción técnica

Seguro que algunos de los técnicos estarán interesados ​​en los detalles, así que seamos más específicos:

### Descripción del producto:

La placa OpenBCI de 32 bits es un escudo para Arduino-Due de 32 bits que lo convierte en un amplificador de bioseñales de 8 canales. Gracias a la potencia de Due, un potente microcontrolador de 32 bits, con mucha memoria local y velocidades de procesamiento rápidas, podrás desarrollar aplicaciones increíbles.

La placa Signalino se puede utilizar para tomar muestras de la actividad cerebral (EEG), la actividad muscular (EMG) y la actividad cardíaca (EKG). La placa se comunica de forma inalámbrica con una computadora a través de un módulo HC-06 BT económico, para que pueda comunicar su proyecto con cualquier dispositivo BT.

Si solo está interesado en usar la placa para investigación y no quiere programar, no hay problema. Descargue SCIGNALS, un potente pero fácil de usar registrador de gráficos basado en Java que hemos desarrollado, conecte su Due+Signalino en un puerto USB libre y ¡comience a grabar!.

La placa viene precargada con el último firmware, lo que hace que Signalino sea accesible para investigadores y desarrolladores con poca o ninguna experiencia en hardware.

Este kit viene con 8 electrodos. Si necesitas más (y sabes que lo harás...) puedes comprar alguno en nuestra tienda. ¡Y muchas cosas más!

Este kit incluye:
- (x1) Signalino
- (x1) Pin de cabecera para adaptador de electrodo a prueba de contacto
- (x8) Electrodos de copa
- (x1) Paquete de baterías AA de 6V (baterías no incluidas)
- (x4) pies de plástico (para estabilización de tablas)

### Especificaciones técnicas:

 - 8 canales de entrada diferenciales, de alta ganancia y bajo ruido
 - Compatible con electrodos activos y pasivos
 - Texas Instruments ADS1299 ADC (enlace a la hoja de datos)
 - Resolución de datos de canal de 24 bits
 - Frecuencia de muestreo de 1 kHz
 - Ganancia programable: 1, 2, 4, 6, 8, 12, 24
 - Voltaje de funcionamiento digital de 3,3 V.
 - +/- voltaje de funcionamiento analógico de 2,5 V
 - Voltaje de entrada ~3.3-6V
 - 5 pines GPIO, 3 de los cuales pueden ser analógicos
![article-img](/img/blog/0001/signalino_prototipo_600.jpg)


###### ***Descargo de responsabilidad***\
*La placa Signalino no es un dispositivo médico ni está diseñada para el diagnóstico médico y se le proporciona "tal cual", y no ofrecemos garantías expresas o implícitas de ningún tipo con respecto a su funcionalidad, operabilidad o uso, incluidos, entre otros, cualquier garantía implícita, idoneidad para un propósito particular o infracción. Renunciamos expresamente a cualquier responsabilidad por daños directos, indirectos, consecuentes, incidentales o especiales, incluidos, entre otros, la pérdida de ingresos, la pérdida de ganancias, las pérdidas resultantes de la interrupción del negocio o la pérdida de datos, independientemente de la forma de acción o teoría legal bajo que se puede hacer valer la responsabilidad, incluso si se le advierte de la posibilidad de tales daños. Esta placa/kit de evaluación está diseñada para usarse ÚNICAMENTE CON FINES DE DESARROLLO DE INGENIERÍA, DEMOSTRACIÓN O EVALUACIÓN** y no se considera como un producto final apto para el uso general del consumidor. Las personas que manipulan el producto deben tener formación en electrónica y observar las normas de buenas prácticas de ingeniería. Como tales, los bienes que se proporcionan no están destinados a ser completos en términos de consideraciones de protección relacionadas con el diseño, la comercialización y/o la fabricación requeridas, incluidas las medidas ambientales y de seguridad del producto que normalmente se encuentran en los productos que incorporan dichos componentes semiconductores o placas de circuito. Esta placa/kit de evaluación no se encuentra dentro del alcance de las directivas de la Unión Europea con respecto a la compatibilidad electromagnética, FCC, CE o UL y, por lo tanto, es posible que no cumpla con los requisitos técnicos de estas directivas u otros documentos relacionados.*

### Read next
[Memboost, improve learning by improving sleep](/blog/enhancing-memory-memboost/)
