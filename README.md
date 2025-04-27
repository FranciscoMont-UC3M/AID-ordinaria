# AID-ordinaria
Proyecto final para la entrega ordinaria de la asignatura de Análisis Inteligente de Datos.

El objetivo es el entrenamiento de un modelo de visión artificial capaz de realizar clasificación de marcas de agua en capturas extraídas de videos. 

Los datos son vídeos de drones de dos fuentes distintas (canales de Telegram de unidades militares rusas): t.me/baikal40ob y t.me/brigada83
Los vídeos han sido seleccionados y editados para sólo mostrar imágenes con el vuelo de un único tipo de drones (guiados por cable de fibra óptica), y donde la marca de agua del canal sea claramente visible. 
Se ha prestado especial atención en editar los vídeo para no mostrar seres humanos o ataques a vehículos ligeros en movimiento, tratándose de mostrar los campos o vehículos abandonados en la medida de lo posible.
La nomenclatura de los vídeos es "X-Y", donde X es el número identificativo de la fuente (40 para t.me/baikal40ob, 83 para t.me/brigada83), y donde Y es el número asociado con ese archivo multimedia en ese canal. Por ejemplo, el vídeo "40-60" sería el vídeo editado correspondiente al publicado originalmente en t.me/baikal40ob/60

A partir de estos vídeos, se han extraído varios fotogramas desde el inicio del vídeo (uno por segundo), creando imágenes que se clasifican como "X-Y-Z", donde X-Y indican el vídeo editado del que proviene la imagen, y la Z corresponde al número de la captura.
Por ejemplo, la imagen "40-60-10" corresponde a la captura nº10 del vídeo "40-60", 9 segundos después de comenzar la reproducción del vídeo.
