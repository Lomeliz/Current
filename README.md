# **Current Jalisco: Plataforma Ambiental de Acción Ciudadana**

*Vigilancia, denuncia y predicción de la contaminación hídrica en Jalisco.*

---

## 📌 **Resumen del Proyecto**

**Current** es una aplicación que permite a los ciudadanos **reportar, visualizar y combatir en tiempo real** focos de contaminación hídrica en la Laguna de Chapala y el río Lerma-Santiago. A través de mapas interactivos, IA predictiva y un sistema de participación ciudadana, democratiza el monitoreo ambiental y potencia la colaboración entre usuarios, instituciones y autoridades.

---

## 🎯 **Objetivo**

Crear una plataforma que combine **denuncia ciudadana, tecnología móvil, ciencia de datos e inteligencia artificial** para:

* Detectar focos contaminantes
* Predecir zonas de riesgo
* Generar presión social y política para actuar
* Restaurar ecosistemas desde la raíz

---

## 📲 **Prototipos Visuales**

* **UI completa en Figma**: flujos, pantallas, mapa interactivo
* **App funcional con Glide**: puedes probar el prototipo en móvil
* **QRs disponibles** en el dosier físico
* **Imágenes adjuntas** del diseño de interfaz
* Incluye: mapa de reportes, formularios, historial, alertas y perfiles

---

## 💡 **Funciones principales**

* 📍 Mapa con reportes ciudadanos geolocalizados
* 🧪 Datos de calidad del agua (pH, color, velocidad, etc.)
* 🧑‍🤝‍🧑 Interacción: likes, comentarios, denuncias colaborativas
* ⚠️ Alertas por riesgo ambiental
* 📊 Historial de soluciones implementadas
* 🧠 Predicción de zonas contaminadas usando IA

---

## ⚙️ **Tecnología utilizada**

* **Frontend/Prototipo:** Glide + Figma
* **Backend previsto:** Node.js + Firebase / Supabase
* **Mapas:** Leaflet.js + OpenStreetMap
* **IA:** Python (scikit-learn, TensorFlow), Vision AI, NLP
* **Base de datos:** JSON estructurado, Firebase Realtime o PostgreSQL
* **Futuro:** Integración con sensores físicos IoT

---

## 🧠 **Integración Estratégica de IA**

> Aquí es donde *Current* piensa.

### Áreas donde usamos o planeamos usar IA:

1. **Predicción de zonas contaminadas**: modelos entrenados con reportes, geografía, lluvia, industria y patrones históricos.
2. **Clasificación automática de reportes**: NLP para interpretar texto y fotos (espuma, olores, cañerías, etc.).
3. **Detección de contaminantes en imágenes**: computer vision aplicado a fotos ciudadanas.
4. **Priorización inteligente**: IA decide qué reportes son más urgentes según impacto ambiental.
5. **Chatbot ecológico**: guía, educa y motiva a los usuarios a participar.
6. **Análisis de sensores (futuro)**: IA detecta anomalías industriales en tiempo real.

---

## 🔧 **Fragmentos de código representativo**

### Validación de reportes

```javascript
function validateReport(report) {
  const { photo, location, description } = report;
  if (!photo || !location || description.length < 20) return "Reporte inválido";
  return "Reporte válido";
}
```

### Predicción de riesgo (Python)

```python
def riesgo_por_distancia(dist_km):
    return "Alto" if dist_km < 0.5 else "Medio" if dist_km < 1.5 else "Bajo"
```

### Estructura JSON de API

```json
{
  "reportes": [
    {
      "usuario": "ciudadano_123",
      "ubicacion": { "lat": 20.124, "lng": -103.455 },
      "foto": "reporte1.jpg",
      "descripcion": "Vertido gris visible",
      "estado": "pendiente"
    }
  ]
}
```

### Carga dinámica en mapa (Leaflet.js)

```javascript
reportes.forEach(rep => {
  if (rep.estado === "validado") {
    L.marker([rep.lat, rep.lng]).addTo(mapa).bindPopup("Validado");
  }
});
```

---

## 🔮 **Visión a futuro**

* 🤖 IA que anticipa colapsos ecológicos locales
* 🤖 IA moderadora y analisis de datos
* 📡 Integración con sensores IoT flotantes
* 📈 Gamificación con recompensas por impacto real
* 📚 Modo educativo para escuelas: monitorea tu río
* 📣 Panel de rendición de cuentas para empresas e instituciones
* 🛜 Datos live
* 🌍 Replicabilidad internacional: Colombia, India, África
* 🏛️ Alianzas: Simapa, Archroma, Gob. de Jalisco, universidades

---


## 📎 **Anexos**
* App prototipo en Glide.         https://isjalisco.glide.page 
* Link a Figma con UI navegable. https://www.figma.com/design/S3tHJD6zV0lKw5fsSVCkim/Sin-t%C3%ADtulo?node-id=0-1&t=dVyUuM326GPbEcS0-1

