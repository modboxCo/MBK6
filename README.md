# MBK6 Macropad

Te presento el **MBK6**, un macropad compacto y altamente personalizable, diseñado para ofrecer una experiencia de usuario óptima en flujos de trabajo que requieren accesos rápidos y configuraciones avanzadas.

Su diseño incorpora una pantalla OLED para visualización de información en tiempo real, un encoder rotatorio para funciones adicionales y compatibilidad con switches mecánicos intercambiables.

---

## Diseño y fabricación

Este macropad ha sido desarrollado íntegramente con un enfoque en funcionalidad y calidad:

**✅ Carcasa impresa en 3D**

La estructura del macropad es fabricada mediante impresión 3D, el resultado de un diseño propio optimizado para resistencia y estética.

**✅ PCB de desarrollo propio**

La placa de circuito impreso ha sido diseñada específicamente para este modelo, asegurando el funcionamiento total de sus componentes y un rendimiento óptimo. El Pro Micro es el cerebro del macropad, un procesador estable y flexible en la programación.

---

## Características principales

| Característica | Descripción |
|----------------|-------------|
| 🎮 **Programación VIAL/VIA** | Asignación de funciones completamente personalizables a través de hasta 4 capas configurables |
| 🖥️ **Pantalla OLED 0.96"** | Muestra el número de capa activa + animación Nyan Cat |
| 🎛️ **Knob rotatorio** | Encoder EC11 para control preciso de volumen, zoom, scroll y más |
| 🎨 **Dos combinaciones** | Blanco con acentos negros / Negro con acentos blancos |

---

## Especificaciones técnicas

| Especificación | Detalle |
|----------------|---------|
| Teclas | 6 teclas mecánicas (switches Halu Halu) |
| Pantalla | OLED 0.96" I2C monocromática |
| Encoder | EC11 rotatorio de alta precisión |
| Microcontrolador | Pro Micro |
| Conectividad | USB-C |
| Firmware | QMK (actualizable y personalizable) |
| Capas | Hasta 4 capas configurables vía VIAL/VIA |
| Dimensiones | 94 × 79 × 28 mm (L×A×H) |
| Peso | 88g (sin switches ni keycaps) |
| Material | PLA impreso en tecnología FDM |

---

## Estructura del repositorio

```
MBK6/
├── firmware/     # Firmware QMK y archivos de compilación
├── VIA/          # Archivo JSON para configuración en VIAL/VIA
└── media/        # Fotos y videos del proyecto
```

## Enlaces rápidos

- [Configuración VIA](VIA/README.md)
- [Firmware](firmware/README.md)

---

## Licencia

MIT License - ver [LICENSE](LICENSE) para más detalles.
