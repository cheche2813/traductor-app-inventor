# 🇪🇸🇫🇷🇮🇹 Explorador de Países y Banderas del Mundo (APK para Android)

Una aplicación móvil para Android diseñada para explorar países, banderas nacionales y elementos geográficos. Cuenta con una interfaz limpia, elementos interactivos y recursos multimedia optimizados.

---

## 📱 Descripción General

- **Plataforma:** Android
- **Estructura:** Nativa de Android (con componentes AppCompat y soporte para archivos DEX)
- **Características Principales:**
  - Exploración de países y banderas (incluyendo España, Francia, Italia, Reino Unido y más).
  - Soporte para gráficos vectoriales (`.svg`) y formatos de imagen optimizados (`.png`, `.webp`).
  - Animaciones de transición personalizadas (`fade`, `slide`, `zoom`).
  - Estructuras adaptadas para diseño responsivo en múltiples densidades de pantalla.

---

## 🗂️ Estructura del Proyecto y Assets

El paquete de la aplicación contiene la siguiente jerarquía organizada de recursos y assets:

```text
├── AndroidManifest.xml
├── classes.dex
├── res/
│   ├── anim/          # Animaciones de transición (desplazamientos, zoom y desvanecimiento)
│   ├── color/         # Selectores de color y temas dinámicos
│   ├── drawable/      # Elementos gráficos de interfaz e insignias
│   ├── layout/        # Diseños XML para actividades, diálogos y barras de herramientas
│   ├── mipmap/        # Iconos de la aplicación (hdpi, mdpi, xhdpi, xxhdpi, xxxhdpi)
│   └── xml/           # Configuraciones de seguridad de red y proveedores de archivos
└── assets/
    ├── espana.png     # Bandera de España (Formato PNG)
    ├── espana.webp    # Bandera de España (Formato WebP optimizado)
    ├── francia.webp   # Bandera de Francia (Formato WebP optimizado)
    ├── italia.svg     # Bandera de Italia (Gráfico vectorial SVG)
    ├── italia.webp    # Bandera de Italia (Formato WebP optimizado)
    └── reino.webp     # Bandera del Reino Unido (Formato WebP optimizado)
```

---

## 🚀 Características Técnicas

1. **Recursos Gráficos Optimizados:** Uso de imágenes en formato WebP junto con gráficos vectoriales (SVG) para garantizar una gran nitidez visual en cualquier pantalla, manteniendo un peso ligero en la APK.
2. **Navegación Fluida:** Implementación de animadores basados en XML (`slide_enter`, `zoom_enter`, `fadein`, `fadeout`) para transiciones de pantalla pulidas.
3. **Diseño Adaptativo:** Compatible con diferentes tamaños de pantalla y configuraciones de tema (modo claro u oscuro).
4. **Seguridad y Proveedores:** Configurado con directrices de seguridad de red y rutas de proveedores de archivos (`network_security_config.xml`).

---

## 🛠️ Primeros Pasos y Desarrollo

Para inspeccionar o reconstruir esta estructura de APK:

1. **Prerrequisitos:**
   - Android Studio / Android SDK
   - Herramientas de ingeniería inversa (Apktool / jadx)
2. **Descompilación y Reconstrucción:**
   ```bash
   # Descodificar recursos de la APK con apktool
   apktool d app.apk -o decoded_app/
   
   # Reconstruir la APK
   apktool b decoded_app/ -o rebuilt_app.apk
   ```

---

## 📄 Licencia

Este proyecto y sus recursos se proporcionan con fines educativos y de análisis de desarrollo.
