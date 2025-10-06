
# 🌱 BloomWatch – Flowering and Cultivation Simulator

**BloomWatch** es una aplicación web interactiva desarrollada como parte del **NASA International Space Apps Challenge**.  
Su objetivo es **visualizar y simular eventos de floración** de cultivos (café y plátano en Colombia) utilizando datos satelitales y modelos probabilísticos.

---

## ✨ Características

* 🗺️ **Mapa interactivo de departamentos**: Visualización del estado de floración en cada región.  
* 📅 **Selección por fecha**: Consultar probabilidades para un día específico.  
* 🌾 **Reportes detallados**: Tarjetas dinámicas con indicadores de floración por cultivo.  
* 🔍 **Consulta personalizada**: Selección de departamento y visualización de resultados.  
* 📊 **Clasificación por colores**:
  * 🟢 **>90%** – Óptimo  
  * 🟢 **75–90%** – Favorable  
  * 🟡 **60–75%** – Moderado  
  * 🔴 **<60%** – Bajo  

---

## 📂 Estructura del Proyecto

```

├── index.html        # Página principal (interfaz y lógica en JS)
├── dataStore.json    # Datos con probabilidades por fecha y departamento
├── mapdata.js        # Configuración del mapa (Colombia)
├── countrymap.js     # Motor de Simplemaps
├── /assets           # Recursos estáticos (iconos, estilos, etc.)

````

---

## 🚀 Cómo ejecutar

Debido a que el navegador no permite cargar archivos locales con `fetch()`, necesitas un **servidor local**:

### Opción 1 – Python

```bash
python -m http.server 8000
````

Abrir en: 👉 [http://localhost:8000](http://localhost:8000)

### Opción 2 – Node.js

```bash
npx http-server
```

### Opción 3 – VS Code

* Instalar la extensión **Live Server**
* Click derecho en `index.html` → *Open with Live Server*

---

## 🛰️ Fuente de datos

Los datos provienen de la **NASA POWER API** (2020–2025) y se procesan con reglas probabilísticas simples para estimar la floración de café y plátano.

---

## 👨‍💻 Equipo

Desarrollado para el **NASA International Space Apps Challenge** como parte de la solución **BloomWatch**.

