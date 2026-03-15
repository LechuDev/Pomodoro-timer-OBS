# Pomodoro Timer para OBS Studio

Un temporizador Pomodoro que se ejecuta desde OBS (sin plugins extras). Muestra el tiempo en pantalla, suena cuando cambian las fases y te deja controlar todo desde el panel de scripts.

---

## ✅ ¿Por qué usarlo?

- **Funciona dentro de OBS**: no necesitas otra app ni ventana adicional.
- **Control total**: inicia/pausa/reset/salta fase desde el panel de scripts.
- **Visual**: el contador se muestra en la escena usando una fuente de texto (puedes cambiar tipografía, color y tamaño).
- **Sonidos opcionales**: agrega alerts al inicio/fin de cada fase.

---

## 🎯 Guía rápida (en 2 minutos)

1. Copia `pomodoro_lechudev.lua` a una carpeta que recuerdes.
2. Abre OBS y ve a **Herramientas > Scripts**.
3. Haz click en **+** y agrega `pomodoro_lechudev.lua`.
4. Crea una fuente de texto en tu escena (Texto GDI+ o similar).
5. En el panel de scripts, selecciona esa fuente en **Fuente de texto del temporizador**.
6. Presiona **Start** para que el contador comience a mostrarse.

> 🔥 Consejo rápido: ajusta la fuente en OBS (tipo, tamaño, color) para que se vea bien en tu escena.

---

## 📸 ¿Qué ves en el panel de scripts?

Estas capturas muestran exactamente el panel de configuración dentro de OBS.

![Controles del temporizador](screenshots/Controles.png)
*Botones para iniciar, pausar, reiniciar y saltar fases.*

![Sesiones configurables](screenshots/Sesiones configurables.png)
*Define cuánto dura cada fase y cuántas sesiones forman un ciclo.*

![Activación de sonidos](screenshots/Activacion de Sonidos con uso de fuentes.png)
*Activa/desactiva los sonidos de notificación y configura las fuentes de audio en OBS.*

---

## 🧠 ¿Cómo se ve el contador en tu escena?

El script escribe texto en la fuente que elijas. Ejemplo de lo que verás en tu escena:

```text
FOCUS 24:59
Sesión 1 / 4
```

Cuando hay descanso:

```text
SHORT BREAK 04:30
Sesión 2 / 4
```

> 🔧 Cambia tipografía, color, tamaño y efectos desde las opciones de la fuente de texto en OBS.

---

## ⚙️ Configuración importante

- **Minutos Focus**: duración de la sesión de trabajo.
- **Minutos descanso corto**: duración del descanso corto.
- **Minutos descanso largo**: duración del descanso largo.
- **Cada cuántas sesiones hay descanso largo**: define cuándo entra el descanso largo.
- **Total de sesiones del ciclo**: cuántas sesiones conforman un ciclo completo.

### Sonidos (opcional)

Para que suenen avisos debes:

1. Crear fuentes de medios en OBS (MP3/WAV).
2. Seleccionar esas fuentes en los campos del script.
3. Activar las casillas de sonido que quieras usar.

---

## 🤝 Contribución

¿Encontraste un bug o querés mejorar algo? Abre un issue o un pull request.

---

## 📄 Licencia

Licencia MIT.

---

## ✨ Autor

Creado por lechudev.
