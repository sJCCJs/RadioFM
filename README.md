# Receptor de Radio FM con SDR (Software Defined Radio)

Este proyecto implementa un receptor de radio FM utilizando bloques de procesamiento de señales en un entorno de GNURadio con un dispositivo RTL-SDR. El código está diseñado para trabajar con hardware compatible con SDR y procesa la señal recibida para su reproducción como audio.

## Descripción

El código proporciona una estructura modular utilizando bloques de procesamiento de señales, cada uno con una función específica en el procesamiento de la señal de radio FM. Algunos de los bloques y su funcionalidad incluyen:

- **osmosdr_source_0:** Controla los aspectos técnicos del receptor SDR, como la frecuencia de sintonización y la ganancia.
  
- **low_pass_filter_0:** Filtra las frecuencias no deseadas, conservando únicamente las asociadas al audio FM.

- **blocks_multiply_const_vxx_0:** Ajusta el volumen de la señal mediante una multiplicación por una constante.

- **blocks_null_sink_0:** Posiblemente utilizado para propósitos de depuración o interno, este bloque no tiene salida aparente en el flujo principal de la señal.

- **qtgui_freq_sink_x_0:** Visualiza la distribución de energía de la señal en el dominio de la frecuencia.

- **qtgui_time_sink_x_0:** Muestra la forma de onda de la señal en el dominio del tiempo.

## Uso

Para utilizar este código, se requiere un hardware RTL-SDR y las dependencias adecuadas instaladas. Asegúrate de seguir las instrucciones específicas del entorno de desarrollo y las bibliotecas necesarias para ejecutar este receptor de radio FM.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, no dudes en realizar un pull request. Antes de realizar cambios significativos, por favor, abre un issue para discutirlos.
