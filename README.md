# Animación Frame por Frame: Walk Cycle en Blender 2D

**Profesor:** Aristides Caballero Alfaro
**Alumno:** [Plascencia Mora David Emiliano]

## Objetivo del Proyecto
Realizar una animación 2D tradicional (frame por frame) de un ciclo de caminado ("walk cycle") utilizando la herramienta **Grease Pencil** en Blender.

## 1. Diseño y Guía de Poses (Proceso 100% Manual)
Para este proyecto, decidí realizar mi propia secuencia de poses de referencia completamente a mano, prescindiendo del uso de Inteligencia Artificial para enfocarme en los fundamentos tradicionales de la animación.

* **Método de bocetaje:** [Describe brevemente cómo lo hiciste. Ej: "Dibujé las poses base directamente en Blender usando una capa de Grease Pencil en color azul", o "Hice los bocetos en papel, los escaneé y los usé como imagen de fondo"].
* **Poses clave desarrolladas:** *Contact* (Contacto), *Down* (Abajo), *Pass* (Pase) y *Up* (Arriba).

![Guía de Poses Manual](./referencias/guia_poses_manual.png)
*(Arriba: Mi propia guía de poses utilizada como base para la animación final).*

## 2. Documentación "How To": Animación con Grease Pencil
A continuación se detalla el método paso a paso que utilicé para lograr la animación en Blender:

### Configuración del Entorno
1. Abrir Blender y seleccionar un nuevo espacio de trabajo **"2D Animation"**.
2. [Si usaste una imagen externa] Importar mi guía de poses dibujada a mano usando `Shift + A` > `Image` > `Reference` y bajarle la opacidad.
3. Crear un nuevo material para el trazo final (ej. tinta negra continua).

### Proceso de Dibujo (Frame x Frame)
1. **Creación de Keyframes:** Seleccionar el objeto *Stroke* (Grease Pencil) y entrar a **Draw Mode**.
2. **Trazado de Poses Clave:** * Me situé en el frame 1 y tracé la primera pose de "Contacto".
   * Avancé en la línea de tiempo y continué dibujando las siguientes poses clave respetando la guía.
3. **Uso de Onion Skinning (Papel Cebolla):** Activé la opción de *Onion Skinning* en las propiedades de la capa. Esto me permitió ver los trazos del frame anterior (en color verde) y posterior (en color rojo), lo cual fue fundamental para dibujar los *in-betweens* (cuadros intermedios) y mantener el volumen del personaje.

### Cierre del Ciclo (Loop)
* Para lograr que el ciclo de caminado fuera infinito, dupliqué el frame inicial y lo coloqué un cuadro después del final de la animación. Esto me sirvió de guía para conectar el último movimiento de la pierna con el primer paso de manera fluida.

## 3. Demostración Presencial
La validación del funcionamiento de esta animación se realizará de forma presencial durante la clase, mostrando el "loop" en tiempo real dentro del viewport de Blender.
