# Proyecto 4 Modelos Probabilísticos de señales y sistemas 
### Brayan Martínez Granados 
### B74495

Mediante el código adjunto se realiza una simulación de una sistema de comunicaciones para la transmisión de imágenes de baja resolución mediante
la implementación de una modulación QPSK. El código consiste en 6 funciones las cuales se detallan acontinución.

- fuente_info: Simula una fuente de información al convertir la imagen formato .jpg en un vector de Numpy
- rgb_a_bit: Convierte los pixeles del vector en un vector unidimencional de N bits.
- modulador: Agrupa el vector unidimencional en grupos de 2 bits los cuales seran modulados bajo QPSK.
- canal_ruidoso: Simula un medio de transmisión no ideal (ruidoso) empleando ruido AWGN.
- demodulador: Demodula la señal mediante decodificación por detección de energía.
- bit_a_rgb: Convierte los bits demodulados a a un vector de pixeles.

Finalmente se grafica la imagen recuperada. 

Complementariamente se realizan pruebas de estacionaridad y ergodicidad mediante las cuales se determinada que la señal modulada es estacionaria en sentido amplio. Tambien se determina la densidad espectral de potencia 
