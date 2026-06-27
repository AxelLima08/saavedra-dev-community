# Guía de Git y GitHub para principiantes

Este documento está destinado a todas aquellas personas interesadas en la programación y la electrónica que buscan desafíos prácticos para mejorar como programadores y meter mano en el código.

## Herramientas que vas a usar

### Para simular circuitos

- **Tinkercad**: software web ideal para hacer simulaciones rápidas con Arduino Uno y componentes electrónicos básicos.
- **Wokwi**: software web avanzado para simular microcontroladores (como el ESP32 o Arduino Mega). Cuenta con una gran cantidad de componentes electrónicos y es muy fiel a la realidad.

### Para escribir código (IDEs)

- **Arduino IDE**: el software nativo de escritorio para escribir firmware usando el framework de Arduino.
- **VS Code**: el editor de código usado globalmente.

## Conceptos clave

### Repositorio (repo)

No lo pienses como una simple carpeta compartida de Google Drive o Dropbox. Un repositorio es una caja negra inteligente para tu proyecto: no solo guarda los archivos de código actuales, sino que registra todo el historial de cambios, quién los hizo y cuándo. Si un proyecto tiene tres años de vida, el repositorio te permite viajar en el tiempo y ver exactamente cómo era el código el primer día.

### Fork (tu copia personal)

El repositorio principal de los desafíos está guardado en una cuenta y está protegido para que nadie pueda romperlo o modificarlo sin autorización. Hacer un Fork es el equivalente a sacar una copia completa del proyecto y guardarla en tu propia cuenta de GitHub. Ahora tenés una copia idéntica que te pertenece, donde podés simular circuitos, cambiar líneas de código y experimentar con total libertad sin alterar el proyecto original.

### Commit (tu punto de guardado)

Un commit es mucho más que apretar Ctrl + S. Funciona como un checkpoint o punto de restauración del código. Imaginá que estás programando algo avanzado, con muchas líneas de código, donde todo ya funciona bien. Si te ponés a modificar cosas para agregar una función nueva, corrés el riesgo de romper lo que ya tenías y no recordar cómo estaba antes. Para evitar eso, hacés un commit: si algo deja de funcionar, podés volver exactamente a ese punto de guardado donde todo andaba bien.

Por ejemplo, un commit típico de este proyecto podría llamarse así:

```bash
git commit -m "feat: ejercicio blink solucionado"
```

Ese mensaje queda guardado para siempre en el historial, así que cualquiera (¡incluso vos mismo, meses después!) puede entender qué cambió en ese punto exacto.

### Pull Request (PR — tu propuesta de entrega)

Traducido literalmente es una "petición de arrastre", pero en la práctica es la entrega del ejercicio. Cuando resolvés un desafío en tu copia personal (tu Fork) y comprobás que funciona correctamente, abrís un Pull Request. Con esto le avisás al administrador del repositorio que ya terminaste el desafío y le entregás tu propuesta de solución para que la revise y, si está todo en orden, la fusione con el proyecto principal.

### Colaborador (Contributor)

Este es el premio mayor en GitHub. Cuando tu Pull Request es revisado, aprobado y fusionado (merged) con el repositorio principal, GitHub te otorga automáticamente el estado de colaborador. Esto significa que tu usuario de GitHub queda asociado públicamente al proyecto para siempre, demostrando que tu código tiene la calidad suficiente para formar parte de una comunidad de desarrollo real.

## ¿Qué es Git?

Git es como una máquina del tiempo para tus archivos de código, pero que solo funciona cuando vos decidís activarla. En vez de duplicar carpetas y guardar archivos con nombres como "codigo_final_v2_este_si", le indicás a Git de forma manual cuándo querés registrar un avance importante de tu circuito. En ese momento, la herramienta guarda un registro de los cambios realizados hasta ahí. Esto te da la tranquilidad de modificar, borrar o cambiar lo que necesites: si el código se rompe, podés deshacer los cambios y volver exactamente al punto anterior donde todo funcionaba. **El control sobre qué se guarda y cuándo es completamente tuyo.**

## ¿Qué es GitHub?

GitHub es el paso siguiente: el puente en internet que conecta tu computadora con el resto del mundo. Si Git es la herramienta que usás dentro de tu máquina para registrar tus avances, GitHub es como una red social combinada con un espacio en la nube donde guardar esos registros. Es el lugar donde subís tus carpetas de código para que no se pierdan si algo le pasa a tu computadora, pero también es la plataforma que permite que muchas personas colaboren en un mismo proyecto de forma ordenada, compartiendo soluciones y mejorando el código entre todos sin generar un caos de archivos.

Si te querés dedicar a la programación, **tu cuenta de GitHub se convierte, literalmente, en tu currículum de la vida real**. Hoy en día, las empresas y los equipos de desarrollo quieren ver qué sabés hacer en la práctica antes que un papel que diga dónde estudiaste. Tu perfil funciona como una vidriera pública: muestra los proyectos que armás, cómo pensás los problemas, qué tan prolijo sos y cuánto tiempo le dedicás a practicar.

Al resolver los ejercicios de este repositorio y enviar tu solución a través de un Pull Request, estás haciendo mucho más que practicar código. Una vez que tu solución sea revisada y aprobada, se fusionará con el proyecto principal y GitHub te registrará automáticamente y de forma permanente como colaborador oficial del repositorio. Para cualquier selector o empresa, entrar a tu perfil y ver que ya sabés trabajar con repositorios reales, que entendés el flujo de trabajo de la industria (Forks, Commits, Pull Requests) y que colaboraste en una comunidad, te posiciona muy por encima de quien nunca haya tocado la herramienta. Es tu oportunidad de empezar a construir experiencia real.

## Cómo empezar

### 1. Creá tu cuenta de GitHub

Entrá a [GitHub.com](https://github.com) y hacé clic en **Sign up**. Si querés, podés vincular tu cuenta de GitHub con la de Google para iniciar sesión con mayor comodidad.

> **Importante:** se recomienda no usar la cuenta institucional `@alum.tec17ba.edu.ar`, sino una cuenta personal.

### 2. Hacé un Fork del repositorio

Una vez creada la cuenta, entrá a la página del repositorio `AxelLima08/saavedra-dev-community` y dejá una estrella. Dentro de la página, leé el `README.md` y el `CONTRIBUTING.md`.

Luego presioná la opción **Fork** (al lado de la estrella). No modifiques nada y confirmá con **Create fork**.

---

### 3. Elegí cómo vas a trabajar

A partir de acá tenés dos opciones. Elegí la que te resulte más cómoda:

---

## 🌐 Opción A — VS Code en el navegador (sin instalar nada)

Esta es la opción más rápida para arrancar: no requiere instalar ningún programa, todo corre desde el navegador.

### A.1. Abrí el editor en el navegador

Ya en tu fork del repositorio, presioná la tecla `.` en tu teclado para abrir VS Code directamente en el navegador.

Te va a pedir iniciar sesión con GitHub: hacé clic en **Permitir** y, en la ventana que se abre, iniciá sesión. Lo primero que vas a ver es el `README.md` del proyecto; podés cerrar esa ventana.

### A.2. Preparé tu solución

Suponiendo que ya tenés tu código listo, comentado, y la explicación junto al link de la simulación de Tinkercad o Wokwi:

1. Desplegá la carpeta de la dificultad correspondiente: `1.0-aprendiz`, `2.0-competente` o `3.0-avanzado`.
2. Dentro vas a encontrar las carpetas de los ejercicios. Por ejemplo, para el ejercicio *blink* dentro de `1.0-aprendiz`, vas a ver un `README.md` con la consigna, hints y restricciones.
3. También hay una carpeta `soluciones`, donde está el archivo `solucion.cpp` (ahí va tu código de respuesta) y un archivo `EXPLICACION.md`.
4. En `solucion.cpp`, reemplazá el texto `GIT_USER` en el comentario `// autor: Saavedra Dev Community - GIT_USER` por tu nombre de usuario de GitHub. Por ejemplo: `// autor: Saavedra Dev Community - AxelLima08`.
5. En `EXPLICACION.md`, completá con tu usuario de GitHub, borrá el texto `"TU_LINK_VA_AQUI"` y poné el link de la simulación con tu código. Donde dice `"Escribí acá tu explicación…"`, borrá esa oración y explicá con tus palabras la solución del ejercicio y cómo llegaste a ella.

> **¿Programaste con PlatformIO en vez de Arduino IDE?** No hay ningún problema: la estructura del código (`setup()` y `loop()`) es exactamente la misma en ambos casos, ya que los dos usan el framework de Arduino. Lo único que tenés que hacer es agregar, al principio de tu `solucion.cpp`, el contenido de tu `platformio.ini` como comentario. Así sabemos qué board y configuración usaste para poder reproducir tu simulación si hace falta.

### A.3. Abrí una terminal

Al costado izquierdo del editor vas a ver tres líneas (menú); hacé clic ahí y elegí **Terminal → Nueva terminal**.

Van a aparecer dos botones azules; el que nos interesa es el que dice **"Continuar trabajando con GitHub Codespaces"**. En la barra de búsqueda de VS Code van a aparecer dos opciones:

a. Elegí **"Sí, continuar con mis cambios de trabajo"**.
b. Luego **"Iniciar sesión con GitHub"**.

Te va a volver a pedir iniciar sesión: confirmá con **Permitir**, **Continuar** y **Autorizar**. Si te pide confirmar el acceso, completalo. Después elegí la versión de **2 cores / 8 GB de RAM**, y se va a abrir una nueva ventana.

> Los nombres exactos de los botones pueden variar levemente si GitHub actualiza su interfaz, pero el flujo general (iniciar sesión, autorizar y elegir la versión del entorno) se mantiene igual.

### A.4. Subí tu código

Una vez completo el ejercicio, volvé a la terminal y ejecutá los siguientes comandos en orden:

```bash
git add .
```

Este comando prepara los archivos que vas a subir con el commit. El argumento `.` le indica a Git que guarde todos los archivos modificados.

```bash
git commit -m "feat: ejercicio NOMBRE_DEL_EJERCICIO solucionado"
```

Esto crea el commit, el punto de guardado de tu avance. Por ahora esto es solo un guardado local.

```bash
git push
```

Esto sube el commit a tu fork del repositorio en GitHub. Si todo salió bien, al entrar a tu fork (`https://github.com/NombreDeUsuario/saavedra-dev-community`) vas a poder ver tus cambios reflejados.

---

## 💻 Opción B — VS Code de escritorio (instalado en tu computadora)

Esta opción es la forma en que trabajan los desarrolladores en la industria: todo corre en tu máquina, tenés más control y no dependés del navegador.

### B.1. Requisitos previos

Antes de arrancar, asegurate de tener instalado:

- [Git](https://git-scm.com/downloads)
- [VS Code](https://code.visualstudio.com/)

### B.2. Configurá tu identidad en Git

Git necesita saber quién sos para asociar tus commits a tu cuenta de GitHub. Abrí una terminal (en Windows podés usar Git Bash o la terminal de VS Code) y ejecutá estos dos comandos, reemplazando los valores con los tuyos:

```bash
git config --global user.name "TuUsuarioDeGitHub"
git config --global user.email "tu@email.com"
```

> Usá el mismo email que registraste en GitHub. Esto es una configuración global: solo tenés que hacerlo una vez en tu computadora.

### B.3. Cloná tu fork

Entrá a la página de tu fork en GitHub (`https://github.com/NombreDeUsuario/saavedra-dev-community`), hacé clic en el botón verde **Code** y copiá el link que aparece bajo **HTTPS**.

Luego, en la terminal, navegá a la carpeta donde querés guardar el proyecto y ejecutá:

```bash
git clone LINK_DE_TU_FORK
```

Esto va a descargar una copia completa del repositorio en tu computadora. Una vez terminado, abrí la carpeta descargada con VS Code.

### B.4. Preparé tu solución

El proceso es idéntico al de la opción A:

1. Desplegá la carpeta de la dificultad correspondiente: `1.0-aprendiz`, `2.0-competente` o `3.0-avanzado`.
2. Dentro vas a encontrar las carpetas de los ejercicios. Por ejemplo, para el ejercicio *blink* dentro de `1.0-aprendiz`, vas a ver un `README.md` con la consigna, hints y restricciones.
3. También hay una carpeta `soluciones`, donde está el archivo `solucion.cpp` (ahí va tu código de respuesta) y un archivo `EXPLICACION.md`.
4. En `solucion.cpp`, reemplazá el texto `GIT_USER` en el comentario `// autor: Saavedra Dev Community - GIT_USER` por tu nombre de usuario de GitHub. Por ejemplo: `// autor: Saavedra Dev Community - AxelLima08`.
5. En `EXPLICACION.md`, completá con tu usuario de GitHub, borrá el texto `"TU_LINK_VA_AQUI"` y poné el link de la simulación con tu código. Donde dice `"Escribí acá tu explicación…"`, borrá esa oración y explicá con tus palabras la solución del ejercicio y cómo llegaste a ella.

> **¿Programaste con PlatformIO en vez de Arduino IDE?** No hay ningún problema: la estructura del código (`setup()` y `loop()`) es exactamente la misma en ambos casos. Lo único que tenés que hacer es agregar, al principio de tu `solucion.cpp`, el contenido de tu `platformio.ini` como comentario.

### B.5. Subí tu código

Con la terminal de VS Code abierta (o cualquier terminal dentro de la carpeta del proyecto), ejecutá los siguientes comandos en orden:

```bash
git add .
```

```bash
git commit -m "feat: ejercicio NOMBRE_DEL_EJERCICIO solucionado"
```

```bash
git push
```

Si es la primera vez que hacés push desde esta computadora, Git puede pedirte que inicies sesión en GitHub. Seguí las instrucciones que aparecen en pantalla. Una vez terminado, entrá a tu fork en GitHub y vas a ver los cambios reflejados.

---

## Antes de abrir tu Pull Request

Una última cosa antes de mandar tu solución: este repositorio tiene una [licencia](LICENSE.md) que protege el proyecto. Al abrir tu Pull Request, estás aceptando que tu aporte pase a formar parte del repositorio bajo esos términos — pero tranquilo, tu código sigue siendo tuyo y vas a aparecer como su autor. Si te interesa el detalle, podés leer el archivo `LICENSE.md`, aunque no es obligatorio para seguir con los pasos.

## Abrí tu Pull Request

Un fork es personal: todavía no lo puede ver nadie en el repositorio original. Por eso el último paso es crear tu primer Pull Request. Este paso es igual independientemente de la opción que hayas elegido.

1. En la página principal de tu fork va a aparecer un mensaje similar a: *"This branch is 1 commit ahead of AxelLima08/saavedra-dev-community:main."*
2. Al costado vas a ver un botón **Contribute**. Si estás seguro de que hiciste todo correctamente, hacé clic en **Open pull request**.
3. El título se va a autocompletar si el commit se hizo correctamente. No hace falta llenar la descripción.
4. Confirmá con **Create pull request**.

Del resto nos encargamos nosotros: revisaremos tu código, tus comentarios y tu simulación. Si está todo correcto, fusionaremos tu fork con el repositorio original y vas a aparecer como colaborador del repositorio.

> **Importante: mandar un solo ejercicio por Pull Request.**

## Para las próximas veces: sincronizá tu fork

Antes de ponerte a trabajar en un nuevo ejercicio, es importante que tu fork esté actualizado con el repositorio original. Si el repositorio recibió nuevos ejercicios o correcciones desde la última vez que trabajaste, tu copia personal va a estar desactualizada y puede generar conflictos al abrir el Pull Request.

### 1. Sincronizá desde GitHub

Entrá a la página de tu fork en GitHub. Si hay cambios nuevos en el repositorio original, vas a ver un mensaje similar a:

*"This branch is X commits behind AxelLima08/saavedra-dev-community:main."*

Hacé clic en **Sync fork** y luego en **Update branch**. Esto actualiza tu fork en GitHub con los últimos cambios del repositorio original.

### 2. Bajá los cambios a tu entorno de trabajo

Después del Sync fork, según la opción que uses:

- **Opción A (navegador):** abrí la terminal del Codespace y ejecutá:

  ```bash
  git pull
  ```

- **Opción B (escritorio):** abrí la terminal de VS Code dentro de la carpeta del proyecto y ejecutá:

  ```bash
  git pull
  ```

En ambos casos, `git pull` baja los cambios que acabás de sincronizar en GitHub a tu entorno local. Una vez hecho esto, ya podés arrancar con el siguiente ejercicio.

## ¿Necesitás ayuda?

Si te quedaste atascado en alguna parte del proceso, no te preocupes: no hay pregunta tonta, todos arrancamos en algún momento sin saber nada de esto. Escribí explicando el inconveniente a:

**axellima726@gmail.com**