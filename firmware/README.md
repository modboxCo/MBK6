# Firmware MBK6

Versiones de firmware QMK para el macropad MBK6.

---

## Última versión: v1.2

**Compatibilidad:** VIAL y VIA

### Cambios en esta versión

- ✅ Corrección de errores reportados
- ✅ Flujo de trabajo optimizado
- ✅ Mejoras menores de rendimiento y estabilidad

---

## Guía rápida de actualización de firmware

Actualizar tu MBK6 es un proceso rápido y sencillo. En menos de un minuto podrás disfrutar de todas las novedades, mejoras y correcciones.

> ⚠️ **Disclaimer:** Este procedimiento se realiza bajo tu propia responsabilidad. No nos hacemos responsables por instalaciones incorrectas, daños al dispositivo o modificaciones no autorizadas.

---

### 🧰 Herramientas necesarias

- [QMK Toolbox](https://github.com/0x7c13/qmk_toolbox/releases) - Software de flasheo
- Firmware MBK6 (`.hex`) - Descarga desde `builds/`
- Archivo JSON para VIA (`mbk6.json`) - Desde `VIA/`

> ℹ️ **Nota:** Todas las versiones son full firmware. Puedes volver a una versión anterior sin problemas.

---

### ⚠️ Antes de actualizar (muy importante)

**Realiza un backup de tu configuración actual.** Durante la actualización, toda la información almacenada en el macropad se perderá.

En VIAL/VIA, exporta tu configuración de macros como archivo `.json` antes de continuar.

---

### 🪜 Paso a paso

#### 🔹 PASO 1: Descargar firmware

Descarga el archivo `.hex` de la versión que deseas instalar desde la carpeta `builds/`.

---

#### 🔹 PASO 2: Instalar QMK Toolbox

1. Descarga e instala QMK Toolbox
2. Al ejecutar por primera vez, instala los controladores desde **Tools → Install Drivers**
3. Asegúrate de aceptarlos para que el dispositivo sea reconocido

---

#### 🔹 PASO 3: Cargar firmware en QMK Toolbox

1. Abre QMK Toolbox
2. Carga el archivo `.hex` descargado
3. En la parte derecha, verifica que el microcontrolador sea: **ATmega32U4**

---

#### 🔹 PASO 4: Entrar en modo bootloader

El MBK6 permite actualizaciones sin abrir el dispositivo:

1. Desconecta el cable USB del macropad
2. Mantén presionada la **tecla superior izquierda**
3. Sin soltarla, conecta nuevamente el cable USB

QMK Toolbox detectará el dispositivo cuando el bootloader esté activo.

> ℹ️ **Si no hay cambios en QMK Toolbox:** Repite este paso o reinstala QMK Toolbox.

---

#### 🔹 PASO 5: Flashear firmware

1. El botón **Flash** se habilitará automáticamente
2. Presiónalo para iniciar la actualización
3. Espera el mensaje: `Flash complete`
4. El MBK6 se reiniciará automáticamente

> ⏱️ **Importante:** El modo bootloader tiene tiempo limitado. Si expira, el macropad reiniciará en modo normal y deberás repetir el PASO 4.

---

#### 🔹 PASO 6: Configurar en VIA

1. Abre [usevia.app](https://usevia.app/) en tu navegador
2. Autoriza el dispositivo cuando se solicite
3. Carga el archivo `mbk6.json` desde la carpeta `VIA/`

¡Listo! 🎉 Tu MBK6 ya está actualizado.

---

### 🔁 ¿Volver a una versión anterior?

No hay problema. Descarga el firmware de la versión deseada y repite el mismo procedimiento.

---

## Estructura de archivos

```
firmware/
├── builds/      # Archivos compilados (.hex)
└── README.md    # Esta guía
```
