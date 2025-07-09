#  Proyecto Zion - Plataforma de Música Inteligente

##  Propósito

Zion es una aplicación web impulsada por IA que permite a cualquier persona subir una canción y obtener su letra, acordes y partituras de forma automática, gratuita y sin anuncios. El proyecto busca democratizar la música y facilitar tanto la creación como el aprendizaje musical.

Zion nace como respuesta a una necesidad real: muchas plataformas actuales limitan el acceso con pagos, publicidad o acceso incompleto. Esta app está creada con un enfoque accesible, educativo y colaborativo.

---

##  Visión

Ser una plataforma inteligente que facilite el acceso a la música como lenguaje universal, ayudando a músicos amateurs, profesionales y entusiastas a aprender, crear, compartir y crecer.

---

## 🛠️ MVP (Versión Mínima Viable)

### Funcionalidades:

* Subida de canciones (MP3/WAV)
* Separación de pistas (voz / instrumentos)
* Extracción automática de acordes y letra
* Visualización en pantalla de resultados
* Descarga de PDF con acordes y letra
* Acompañamiento textual del asistente Zion

### Flujo de uso:

```
1. El usuario entra a la app
2. Sube un archivo de audio
3. El backend con IA separa voz e instrumentos (Spleeter)
4. Se detectan acordes y letra (BasicPitch + otras herramientas)
5. Se muestran los resultados con ayuda textual de Zion
6. El usuario puede exportar los resultados en PDF
```

---

##  Tecnologías Propuestas

| Módulo            | Herramientas                          |
| ----------------- | ------------------------------------- |
| Frontend          | React.js + TailwindCSS + Vercel       |
| Backend           | Node.js (Express) o FastAPI (Python)  |
| IA Musical        | Python, Spleeter, Librosa, BasicPitch |
| Exportación       | jsPDF o pdfkit                        |
| Almacenamiento    | Firebase / temporal local             |
| Asistente IA      | Chat Zion (JSON, JS o luego GPT API)  |
| Control de código | Git + GitHub + GitHub Actions         |

---

##  Estructura del Repositorio

```
zion-app/
├── frontend/
│   └── src/
│       ├── App.jsx
│       ├── UploadForm.jsx
│       ├── ResultView.jsx
│       └── ZionAssistant.jsx
│
├── backend/
│   ├── index.js (o main.py)
│   └── ia/
│       ├── spleeter_process.py
│       └── chord_detector.py
│
├── docs/
│   └── arquitectura.md
│
└── README.md
```

---

##  Roadmap Inicial

### Etapa 1: MVP

* [x] Documentación de visión, arquitectura y flujo
* [ ] Subida de audio desde frontend
* [ ] Procesamiento backend con Spleeter y extracción de acordes
* [ ] Mostrar resultados básicos
* [ ] Exportar a PDF
* [ ] Chat Zion básico

### Etapa 2: Beta pública

* [ ] Mejorar UI/UX
* [ ] Almacenamiento en la nube
* [ ] Soporte multiusuario (cuentas básicas)
* [ ] Editor simple de acordes

### Etapa 3: Plataforma educativa

* [ ] Sistema de cursos
* [ ] Progreso del estudiante
* [ ] Zion como guía educativa interactiva

### Etapa 4: Comunidad

* [ ] Perfiles de usuario
* [ ] Compartir canciones y creaciones
* [ ] Feedback entre usuarios

---

##  Modelo de Sostenibilidad

### Público objetivo:

* Músicos amateurs y profesionales
* Productores, iglesias, instituciones sin fines de lucro
* Estudiantes autodidactas

### Fuentes de ingreso éticas (opcional):

* Donaciones voluntarias (tipo Ko-fi / Patreon)
* Plan educativo opcional con cursos premium
* Patrocinios sociales de organizaciones musicales
* Alianzas con conservatorios o instituciones públicas

Zion será siempre gratuito para lo esencial: extraer, aprender y compartir música.

---

## Zion: el Asistente Inteligente

Zion es más que una IA. Es un compañero.

### Capacidades iniciales:

* Acompañar con frases motivadoras y explicativas
* Guiar paso a paso el uso de la plataforma
* Recordar buenas prácticas musicales

### Futuro:

* Evaluar conocimientos teóricos (cuestionarios)
* Recomendar ejercicios personalizados
* Interactuar con voz o video

---

##  Cierre

