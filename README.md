
# Cadena de Custodia y Análisis Forense Digital
Investigación forense digital centrada en la extracción, preservación e inspección de evidencia almacenada en una imagen de disco con extensión, haciendo uso de herramientas como AccessData FTK Imager, demostrando la recuperación de archivos protegidos por contraseña,  extracción de metadatos EXIF y la geolocalización 

> Tipo:Análisis técnico y forense.

Este repositorio documenta el procedimiento completo de **análisis forense digital** aplicado a una imagen forense en formato `.E01` de un dispositivo USB confiscado. El objetivo de la investigación fue desencriptar archivos protegidos, realizar la extracción limpia de evidencias sin alterar metadatos y utilizar inteligencia de fuentes abiertas (**OSINT**) para la georreferenciación de una ubicación físico.

## 🛠️ Metodología y Herramientas Utilizadas

* **Montaje y Adquisición:** AccessData FTK Imager v4.7.1.2 para preservación de solo lectura.
* **Análisis Lógico de Particiones:** Exploración del sistema de archivos NTFS en la imagen `mascota.E01`.
* **Criptoanálisis / Desencriptación:** Desbloqueo del contenedor Office mediante ataque/credenciales y remoción de cifrado].
* **Extracción de Evidencia Oculta:** Deconstrucción estructural de archivos OpenXML (`.docx` a `.zip`) para la extracción binaria de la evidencia gráfica `image1.jpg`.
* **Análisis de Metadatos EXIF:** Lectura de metadatos nativos para extraer el modelo de captura (*Xiaomi 23013PC75G*) y coordenadas GPS exactas.
* **Geolocalización & OSINT:** Triangulación geoespacial mediante Bing Maps y verificación a nivel de calle con Google Street View.

## Hallazgos Clave
* **Coordenadas GPS Extraídas:** `25.736846, -100.166077`[cite: 45, 46]
* **Geolocalización Confirmada:** Establecimiento comercial en Calle Nicolás Bravo, Parque Bugambilias de Huinalá, Ciudad Apodaca
