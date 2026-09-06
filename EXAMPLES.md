## 📂 Ejemplos de registro de fechas

Código

```
USER:
El martes tengo examen de matemáticas.

QUETZALCOATL:
Mencionaste un evento para el martes.
¿Quieres que lo registre?
```

Código

```
USER:
Recuérdame pagar la luz el 10 de septiembre.

QUETZALCOATL:
Registrado para el 10 de septiembre.
```

Código

```
USER:
El domingo voy a salir de viaje.

QUETZALCOATL:
Evento detectado: salida de viaje el domingo.
¿Quieres que lo guarde?
```

## 🗂️ Ejemplos de organización de archivos

Código

```
USER:
Ordena mi inbox.

QUETZALCOATL:
Encontré 32 archivos.
Clasificados en: 12 imágenes, 8 documentos, 7 audios, 5 misceláneos.
¿Quieres que los mueva a sus carpetas correspondientes?
```

Código

```
USER:
Renombra mis fotos.

QUETZALCOATL:
Detecté 15 imágenes de WhatsApp.
Ejemplo: "WhatsApp-image-20260905-xyz" → "foto_whatsapp_05_09_26".
¿Quieres aplicar este patrón a todas?
```

Código

```
USER:
Limpia descargas.

QUETZALCOATL:
Carpeta inbox_00 contiene 47 archivos.
Propuesta: mover 20 PDFs a 02_docs, 15 imágenes a 05_fotos, 12 audios a 06_audio.
¿Confirmo?
```

## 💻 Ejemplos de estado del sistema

Código

```
USER:
¿Está activo el NAS?

QUETZALCOATL:
NAS: accesible
Latencia: 12 ms
Espacio libre: 73%
```

Código

```
USER:
Temperatura de la CPU.

QUETZALCOATL:
CPU: 47°C
Uso: 18%
No detecto sobrecalentamiento.
```

Código

```
USER:
¿Mi RAM está bien?

QUETZALCOATL:
RAM: 62% en uso
Procesos principales: navegador, Ollama, editor
Sistema estable.
```

Código

```
USER:
¿Hay problemas en mi PC?

QUETZALCOATL:
CPU: 9%
RAM: 44%
DISK: 58%
NAS: accesible
No detecto fallos.
```

## 🎛️ Ejemplos mixtos (combinando funciones)

Código

```
USER:
El jueves tengo junta y además ordena mi inbox.

QUETZALCOATL:
Evento detectado: junta el jueves. ¿Quieres registrarlo?
Encontré 21 archivos en inbox_00. ¿Quieres organizarlos?
```

Código

```
USER:
Revisa mi PC y dime si hay algo raro.

QUETZALCOATL:
CPU: 15%
RAM: 49%
DISK: 65%
NAS: accesible
No detecto anomalías.
```

Código

```
USER:
El 15 de septiembre es fiesta nacional, y quiero que mis fotos estén ordenadas.

QUETZALCOATL:
Evento detectado: fiesta nacional el 15 de septiembre. ¿Registrar?
Encontré 34 imágenes en inbox_00. Propuesta: mover a 05_fotos con nombres normalizados.
```

## 🧪 Casos límite / respuestas lúdicas

Código

```
USER:
El año que viene cumplo 18.

QUETZALCOATL:
Evento detectado: cumpleaños dentro de un año.
¿Quieres que lo registre?
```

Código

```
USER:
Organiza TODO.

QUETZALCOATL:
Carpeta inbox_00 contiene 123 archivos.
Clasificación completa lista.
¿Quieres aplicar organización masiva?
```

Código

```
USER:
Mi PC está explotando??

QUETZALCOATL:
CPU: 96%
RAM: 92%
DISK: 88%
Temperatura CPU: 89°C
⚠️ Alto consumo detectado. Recomendación: cerrar procesos pesados.
```