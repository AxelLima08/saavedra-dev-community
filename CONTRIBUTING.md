# 📋 Guía de Contribución

Gracias por ser parte de **saavedra-dev-community**. Este archivo explica cómo participar y cuáles son las reglas del proyecto. Leelo completo antes de enviar tu primera solución.

---

## 🛠️ ¿Cómo enviar una solución?

Si nunca usaste Git o GitHub, consultá primero la guía para principiantes:
👉 [**Guía de Git y GitHub para principiantes**](GUIA_PARA_PRINCIPIANTES.md)

Si ya sabés manejarte, los pasos son:

1. **Forkeá** este repositorio (copia el repo en tu cuenta de GitHub)
2. **Cloná** tu fork en tu computadora
3. Colocá tu solución en el archivo `solucion.cpp` del desafío correspondiente
4. Completá el archivo `EXPLICACION.md` de ese desafío incluyendo el link de tu simulación y los detalles solicitados
5. Subí los cambios y abrí un **Pull Request**

> **¿Usás PlatformIO?** No hace falta nada especial: la estructura del código (`setup()` y `loop()`) es la misma que en Arduino IDE. Solo agregá al principio de `solucion.cpp` el contenido de tu `platformio.ini` como comentario, así sabemos qué board y configuración usaste.

---

## ⏳ Sistema de cola de Pull Requests

Las soluciones se revisan **en orden de llegada**. Esto significa:

- El primer Pull Request recibido es el primero en ser revisado
- Si tu solución tiene errores, se te notificará con una explicación clara de qué corregir
- Una vez corregida, tu solución vuelve a la cola **al final** — el lugar en la cola no se reserva
- Si la solución siguiente está correcta, esa será la que quede en el repositorio

Los tiempos de revisión pueden variar según la cantidad de Pull Requests en cola. Esto incentiva enviar soluciones bien pensadas desde el principio.

---

## 📝 Estándares de código

Para mantener el repositorio ordenado y legible, toda solución debe cumplir:

### Comentarios
No es necesario comentar cada línea, pero sí las partes que lo requieran. La regla es simple:

> Comentá el **por qué**, no el **qué**

```cpp
// ❌ Esto no aporta nada
int contador = 0; // declaro contador

// ✅ Esto sí aporta
delay(1000); // esperamos 1 segundo para que el sensor se estabilice antes de leer
```

El nivel de comentarios esperado varía según la dificultad del desafío — en un ejercicio avanzado los comentarios son más importantes que en uno de nivel aprendiz.

### Indentación
Todo el código debe estar correctamente indentado. Código sin indentar será devuelto para corrección antes de ser revisado.

---

## 🤖 Política de uso de Inteligencia Artificial

Creemos que la IA es una herramienta poderosa para aprender. Nuestra filosofía es:

> **Primero entendé, después copiá y pegá.**

**Está permitido:**
- Usar IA para entender un concepto o un error
- Usar IA para comparar tu solución con otras alternativas
- Usar IA como herramienta de debugging

**Está prohibido:**
- Enviar código generado por IA que no puedas explicar
- Presentar como propia una solución que no comprendés

El incumplimiento de esta regla tiene consecuencias definitivas:

> ⚠️ Ante cualquier irregularidad detectada, la contribución será eliminada del repositorio y el usuario quedará inhabilitado permanentemente para participar en el proyecto.

Antes de enviar tu solución, preguntate: **¿Puedo explicar cada línea de este código?** Si la respuesta es no, seguí aprendiendo — para eso está este proyecto.

---

## 🤝 Código de conducta

Este es un espacio de aprendizaje colaborativo. Se espera que todos los participantes:

- Se traten con respeto en todo momento
- Corrijan desde lo constructivo, explicando el **por qué** de cada observación
- Reciban las correcciones con apertura — un error es una oportunidad de aprender
- Eviten todo tipo de insulto, burla o comentario negativo hacia las soluciones de otros

Las contribuciones que no respeten estas pautas serán rechazadas.

---

## ©️ Licencia y qué implica enviar un Pull Request

Este repositorio está protegido bajo licencia [CC BY-NC 4.0](LICENSE.md) (Atribución-NoComercial).

Al enviar un Pull Request, aceptás que tu aporte se incorpora al proyecto bajo los términos de esa licencia: vas a conservar el crédito de autoría por lo que hiciste, pero el proyecto puede seguir usando y redistribuyendo tu contribución, incluso en futuras versiones del repositorio.

> Si aportás una solución (`solucion.cpp`), ese código es y sigue siendo tuyo — el repositorio simplemente queda habilitado a usarlo como parte del proyecto. Más detalles en [LICENSE.md](LICENSE.md).

---

## 🏆 ¿Querés proponer un nuevo desafío?

Por el momento, los desafíos son agregados exclusivamente por el administrador del repositorio para garantizar la calidad y coherencia del proyecto. Si tenés una idea para un desafío, podés abrir un [**Issue**](../../issues) describiéndola y será considerada.

---

*saavedra-dev-community — AxelLima08*
