# ⚡️ **TRON ARES by Viaja Tech** ⚡️  
*El launcher multimedia inspirado en el próximo film **TRON ARES** que fusiona OFICINA + STREAM + IA en una sola ventana.*

[![Ver video en YouTube](https://img.youtube.com/vi/asnVBRyndiI/0.jpg)](https://youtu.be/asnVBRyndiI?si=aUrW-pMObsz4LAP2)

> «Bienvenido al Grid: aquí tu PC se convierte en un HUB cinético donde Word, Excel, navegadores, YouTube‑DL y tu modelo local conversan como si fueran light‑cycles iluminando la oscuridad.»

---

## ✨ Por qué te encantará

| Superpoder | Descripción rápida |
|------------|--------------------|
| 🎞️ **Descarga & conversión turbo** | Baja vídeos o listas completas con `yt‑dlp`, convierte a MP3/MP4 on‑the‑fly y muestra barras **cyber‑HUD** en consola. |
| 🎧 **Reproductor integrado** | Pásate directo a la acción: playlist dinámica (pygame + VLC) con atajos ⏮ ⏯ ⏭ y control de volumen/mute. |
| 🖥️ **Modo Oficina** | Escribe en *Notepad*, edita *Word* o llena hojas *Excel*… ¡sin salir de la app! Automatización COM con autoguardado de emergencia. |
| 🌐 **Navegación ninja** | Lanza búsquedas “*,fotos de neon bikes*”, “*videos en YouTube de synthwave*”, o abre Spotify en 1 comando (Selenium + driver manager). |
| 🗣️ **Chatbot Gradio** | Conecta tu *LLM local* (OpenAI compatible) y dicta comandos: “Descarga el audio de …”, “Reproduce *Daft Punk*” o “Abre Word y escribe…”. |
| 🔊 **STT/TTS ready** | Reconoce voz (Google Speech) y, si tienes Azure, responde hablándote con voz de sintetizador. |
| 🕶️ **Estilo Tron** | Logging en tiempo real con color + archivos, GUI Tkinter dark‑grid, pestañas modulables, y nombre épico en la barra de título. |

---

## 🚀 Instalación

```bash
# 1. Clona el repositorio
git clone https://github.com/viajatech/ARES.git
cd ARES

# 2. Crea un entorno (recomendado)
python -m venv venv
source venv/Scripts/activate   # PowerShell
# o
source venv/bin/activate       # macOS/Linux (solo para pruebas, GUI completa en Windows)

# 3. Instala dependencias principales
pip install -r requirements.txt
```

> **Requisitos extra**  
> * Windows 10/11 para integración Office y notepad.exe  
> * FFmpeg en PATH (para conversiones)  
> * `ffmpeg`, `yt-dlp`, `Chrome`/`Firefox` instalados  
> * Pygame y VLC opcionales → el instalador los detecta y silencia las funciones que falten.

---

## ⚙️ Uso rápido

```bash
python tron_ares.py
```

1. Aparecerá la **ventana Tron Ares** con pestañas: Notepad · Word · Excel · Chrome · Firefox · Downloader · Player.  
2. Se abrirá un **Chat Gradio** en tu navegador:  
   *Escribe* «Descarga el video de https://youtu.be/…» → el bot limpia la URL, crea carpeta y muestra barra de progreso.  
   *Escribe* «Reproduce galaxy.mp3» → se busca en Descargas/Escritorio y comienza a sonar.  
   *Escribe* «Abre Excel y escribe inventario» → genera y abre la hoja.  

### CLI de consola (sin Chat)

```python
from tron_ares import direct_download_media
ok, msg = direct_download_media("https://youtu.be/dQw4w9WgXcQ", is_audio=True, format_type="mp3")
print(msg)
```

---

## 🛠️ Roadmap

- [ ] **Overlay “Derezz”** en reproducción video (shader retro).  
- [ ] Integración **ElevenLabs** TTS + avatar 3D.  
- [ ] Modo **portable USB** (sin instalación).  
- [ ] Dashboards de métricas (descargas/duración/bitrate) con *Plotly*.

---

## 🤝 Contribuciones

Pull requests son bienvenidos: ideas, issues o mejoras de GUI.  
Por favor sigue el formato de *commit* estilo **Conventional Commits** y asegúrate de probar en Windows.

---

## 📜 Licencia

**Apache License 2.0** – haz forks, modifícalo, mejóralo y comparte el neon love.  
Consulta `LICENSE` para ver los detalles.

---

## 👤 Autor

**David Ruiz (@viajatech)** – hotel‑tech futurist, creator of immersive stacks & cyber‑aesthetics.

---

### 📝 Resumen funcional del script

*TRON ARES by Viaja Tech* es una suite Python/Tkinter que:

* automatiza Word, Excel y Notepad con COM,
* descarga y convierte audio + video vía `yt‑dlp` con barra de progreso ASCII,
* reproduce playlists con Pygame (audio) y VLC (video),
* abre Chrome/Firefox y ejecuta búsquedas inteligentes,
* expone todo dentro de una GUI por pestañas **y** un chatbot Gradio integrado que entiende comandos naturales para orquestar las funciones anteriores,  
  registrándolo todo en logs duales consola+archivo para que nunca pierdas el hilo de tu aventura en el Grid.

¡Disfruta el viaje al ciber‑universo TRON ARES y lleva tu flujo multimedia al siguiente nivel! 🎇

![](https://github.com/viajatech/ARES/blob/main/ARES%202.0%20.png)
