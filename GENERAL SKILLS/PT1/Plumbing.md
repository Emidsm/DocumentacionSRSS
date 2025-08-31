### - Descripción del reto

Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.
### - Procedimiento
Primero, hice el netcat me conecté a esa dirección, copié todo, lo puse en un bloc de notas y busqué la bandera, pero no tuve suerte. Por lo que vi una pista e investigué sobre pipes, el término que hace referencia a la plomería, llegué al comando "grep" que funciona para filtrar la salida y que contenga solamente el texto que necesitamos.

después de ejecutar este comando para jalar únicamente los resultados que contengan "pico"
```bash
nc jupiter.challenges.picoctf.org 14291| grep "pico"
```
la cadena fue la siguiente:
### - Solución
picoCTF{digital_plumb3r_ea8bfec7}