# Problemas con el Karaoke Navidadeño (Inspirado en hechos reales)
Tras unas semanas de arduo trabajo y dificultades, las fiestas navideñas se acercan y el tsunami de tareas parece menguar. Como cada año, te aprestas a preparar el tradicional karaoke navideño para la familia pero... cual es tu sorpresa, que tras instalar la última versión de un conocidísimo programa para dichos menesteres, muchos de los temas estrella parecen no funcionar.
:-S :-S :-S

Tras una minuciosa investigación has descubierto que el problema viene por el fichero que especifica los datos de la canción y su letra. Concretamente ha una serie de campos que antes se soportaban como números en coma flotante, que ahora sólo se soportan como enteros por la última versión del programa de karaoke.

Tu misión, es crear un programa que cree una copia de las canciones del karaoke (almacenadas en el directorio resources/temazos) en el directorio (resources/grandesexitos), cambiando el formato del fichero que especifica los metadatos de la canción (llamado <nombre_cancion>.txt) por una compatible con la última versión del karaoke.

Concretamente las modificaciones que hay que hacer en los ficheros son:
- Si la línea del fichero comienza con el texto "#GAP:", significa que especifica el tiempo que hay entre el comienzo del video y el comienzo de la reproducción de la letra de la canción. Este valor debe ser un entero, por lo que si el valor especificado en el fichero contiene el carácter ',' hay que redondear el valor al valor entero más cercano.
- Si la linea del fichero comienza con el texto: "#BPM:", significa que especifica la velocidad a la que debe reproducirse (avanzar) la letra de la canción en el karaoke. Este valor debe ser un entero, por lo que si el valor especificado en el fichero contiene el carácter ',' hay que redondear el valor al valor entero más cercano.
- El resto de líneas del fichero debe permanecer inalteradas.



