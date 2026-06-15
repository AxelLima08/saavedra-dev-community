# Auto Fantástico (sin solucionar)

**Dificultad:** 1.3 — Aprendiz  
**Tags:** `hardware` `arduino` `led` `aprendiz`

---
## 📌 Consigna  

Escribe un programa que controle 4 LEDs conectados a pines digitales, con el objetivo de crear un efecto de ola de ida y vuelta. (explicacion mas tecnica)

### Enfoque Técnico

La secuencia lógica debe ser estrictamente secuencial y unitaria, manteniendo un solo LED activo a la vez siguiendo el orden 1-2-3-4-3-2-1, donde cada estado de encendido tendrá una duración fija de 200 ms controlada mediante la función delay(). Todos los pines utilizados deberán quedar explícitamente declarados como salidas en el bloque setup() utilizando pinMode(), asegurando que el flujo de transiciones sea fluido y continuo sin repeticiones dobles en los extremos de la secuencia.


---

## ⚠️ Restricciones

- Solo se permite usar el framework de Arduino
- No se permite usar librerías externas

---

## 💡 Hints

- Presta atención al orden de la secuencia proporcionada. Al llegar al cuarto LED, el siguiente en encenderse debe ser el tercero. Si notas que el primer o el último LED parpadean el doble de tiempo que el resto, revisa la secuencia de transiciones en tu código.
- Presta atención al orden de la secuencia proporcionada. Al llegar al cuarto LED, el siguiente en encenderse debe ser el tercero. Si notas que el primer o el último LED parpadean el doble de tiempo que el resto, revisa la secuencia de transiciones en tu código.

---

## 📁 ¿Cómo subir tu solución?

1. Forkeá este repositorio
2. Colocá tu solución en la carpeta `soluciones/`
3. Nombrá tu archivo como `solucion-tuNombre.ino` o `solucion-tuNombre.cpp`
4. Abrí un **Pull Request**

¿Es tu primera vez usando Git y GitHub? 👉 [Guía para principiantes](https://docs.google.com/document/d/1xKinkK6HFmD4CzjkcRy7lE9HHumOA2GFtXmhV6OhRgw/edit?tab=t.0)