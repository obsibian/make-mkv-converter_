# Make MKV Converter

Make MKV Converter es una aplicación gráfica diseñada para convertir archivos de video al formato MKV con codificación de audio PCM, específicamente optimizada para edición de video y trabajo de audio profesional.

<img width="582" height="539" alt="makewa" src="https://github.com/user-attachments/assets/091c082b-03da-4e55-908c-aa82342cceb2" />

---

## ✨ Características

- **Interfaz de Arrastrar y Soltar**: Simplemente arrastra archivos de video a la ventana de la aplicación
- **Optimizado para DaVinci Resolve**: Genera MKV con audio PCM (16 bits, 48kHz, estéreo)
- **Sin Pérdida de Calidad**: El flujo de video se copia sin recodificar
- **Salida Configurable**: Elige directorios de salida personalizados

## 🖥️ Uso

### Conversión Básica

1. **Inicia la aplicación**
2. **Selecciona un archivo de video**:
   - Arrástralo y suéltalo en el área púrpura
   - Haz clic en "Examinar" para seleccionarlo manualmente
   - Formatos admitidos: MP4, AVI, MOV, MKV, WMV, FLV, WEBM
3. **Configura la salida** (opcional):
   - Por defecto: `~/Videos/`
   - Haz clic en "Cambiar" para seleccionar una carpeta diferente
4. **Haz clic en "Crear MKV con PCM"**
5. **Espera a la conversión**:
   - El progreso se muestra en la barra de estado
   - Informe detallado al finalizar

### Formato de Salida

El convertidor crea archivos MKV con:
- **Video**: Códec original (copiado sin recodificar)
- **Audio**: PCM 16-bit, 48kHz, estéreo (compatible con DaVinci Resolve)
- **Nombre de archivo**: `[nombre_original]_convertido.mkv`

## 🔧 Detalles Técnicos

### Configuración de Audio

DaVinci Resolve funciona mejor con las siguientes configuraciones de audio:
- **Formato**: PCM (Sin comprimir)
- **Profundidad de bits**: 16-bit
- **Frecuencia de muestreo**: 48kHz
- **Canales**: Estéreo (2)

### Formatos de Entrada Admitidos

| Formato | Extensión | Notas |
|---------|-----------|-------|
| MP4 | `.mp4` | H.264, H.265 |
| AVI | `.avi` | Varios códecs |
| MOV | `.mov` | Formato QuickTime |
| MKV | `.mkv` | Contenedor Matroska |
| WMV | `.wmv` | Windows Media |
| FLV | `.flv` | Video Flash |
| WEBM | `.webm` | Formato Web |

---

## 📦 Instalación

Instala el paquete `.deb` en Debian 13 con:

```bash
sudo dpkg -i ./*.deb
sudo apt install -f
```

---

## 🧰 Requisitos

* Sistema operativo: **Debian 13**.
* Dependencias estándar incluidas en el paquete `.deb`.

---

## 📜 Licencia

Este proyecto está bajo la **Licencia Pública General de GNU v3.0**.

---

## 📧 Contacto

Opcional: telegram @geinux
