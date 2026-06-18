# Auto Fantástico (sin solucionar)

**Dificultad:** 1.3 — Aprendiz  
**Tags:** `hardware` `arduino` `led` `aprendiz`

---
## 📌 Consigna  

Escribe un programa que controle 4 LEDs conectados a pines digitales, con el objetivo de crear un efecto de ola de ida y vuelta.

### Más especifico
---
La secuencia debe seguir el orden **1→2→3→4→3→2→1**, manteniendo
un solo LED activo a la vez.    
Cada estado de encendido tendrá una duración fija de **200 ms**
controlada con `delay()`. Todos los pines deben quedar declarados
explícitamente como salidas en `setup()` usando `pinMode()`.


---

## ⚠️ Restricciones

- Solo se permite usar el framework de Arduino
- No se permite usar librerías externas
- Usar la placa arduino uno

---

## 💡 Hints

- Presta atención al orden de la secuencia proporcionada. Al llegar al cuarto LED, el siguiente en encenderse debe ser el tercero. Si notas que el primer o el último LED parpadean el doble de tiempo que el resto, revisa la secuencia de transiciones en tu código.
- Recuerda que para lograr un efecto visual fluido y unitario, debes asegurarte de apagar el LED actual antes (o en el mismo instante) de encender el siguiente.

---

## 📁 ¿Cómo subir tu solución?

1. Forkeá este repositorio
2. En la carpeta `soluciones/` encontraras un archivo `solucion.cpp` pegar la respuesta ahí y completa `EXPLICACION.md`.
3. Abrí un **Pull Request**

¿Es tu primera vez usando Git y GitHub? 👉 [**Guía de Git y GitHub para principiantes**](../../GUIA_PARA_PRINCIPIANTES.md)