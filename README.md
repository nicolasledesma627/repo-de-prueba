# repo-de-prueba
DESCRIPCIÓN DEL PROYECTO

El proyecto consiste en el diseño y desarrollo de un sistema de conteo controlado
de comprimidos o pastillas. El sistema permite al usuario establecer desde una computadora,
mediante comunicación serie (UART), la cantidad objetivo de unidades requeridas en un rango
de 01 a 99 pastillas. Una vez fijado el objetivo, el sistema mantiene dos servomotores en 
posición de reposo, permitiendo el paso de las unidades. A medida que cada pastilla atraviesa 
el canal de detección, un sensor óptico/infrarrojo conectado a una entrada analógica provoca 
el decremento unitario del contador, visualizándose en tiempo real la cantidad restante en 
dos displays de siete segmentos multiplexados. 

Al alcanzar el conteo el valor 00 , el microcontrolador acciona los servomotores hacia su estado
activo para liberar el lote dosificado y transmite hacia la PC la cadena de texto "Completo" .
Asimismo, si el suministro de pastillas resulta insuficiente para alcanzar la meta programada, 
el usuario dispone de un pulsador de apertura forzada conectado a RB0 (atendido por interrupción externa)
que activa los servomotores de inmediato, lleva el contador a cero y notifica a la PC mediante
el mensaje "Incompleto" . 




