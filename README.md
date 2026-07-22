# Gestor de Prospectos · EmocionArteStudio / BodasPro

**Proyecto:** Herramienta web para gestión de prospectos y proveedores  
**Autor:** Luciano CM  
**Descripción:** Interfaz ligera (HTML/CSS/JS) para añadir, editar, importar y exportar fichas de prospectos y proveedores. Permite edición inline, búsqueda, duplicado, eliminación y exportación/importación en formato Excel (.xlsx). Los datos se guardan localmente en el navegador (localStorage) y pueden exportarse para integrarse en la base de datos interna de la empresa.

---

## Estructura del repositorio
- `index.html` — Interfaz principal y carga de librerías (SheetJS, FileSaver).
- `styles.css` — Estilos responsivos y accesibles.
- `app.js` — Lógica: CRUD, import/export XLSX, persistencia en localStorage, búsqueda y validaciones básicas.
- `README.md` — Este archivo.
- `.gitignore` — Recomendado (node_modules, .DS_Store, etc.).

---

## Funcionalidades principales
- Añadir, editar y eliminar registros directamente en la tabla.
- Duplicar filas para acelerar la captura.
- Búsqueda en tiempo real sobre todos los campos.
- Importar desde archivos `.xlsx` (mapeo por encabezados o por orden de columnas).
- Exportar la tabla visible a `.xlsx`.
- Persistencia local mediante `localStorage`.
- Campos estándar incluidos: Nombre empresa, Responsable, Categoría/Servicios, Web, Instagram, Email, Teléfono, Provincia/Ciudad, Estimación presupuestal, Observaciones, Fuente, Fecha captura, Estado.

---

## Requisitos
- Navegador moderno (Chrome, Edge, Firefox).
- Conexión a internet para cargar las librerías CDN (opcional: descargar librerías y servir localmente).
- Para colaboración en equipo y control de versiones: Git y un repositorio remoto (GitHub).

---

## Instalación y uso local
1. Clona o descarga el repositorio y sitúate en la carpeta del proyecto.
2. Abrir `index.html` en el navegador (doble clic) o servir con un servidor local:
   ```bash
   # Opcional: servir con Python (puede ser útil para evitar restricciones de CORS)
   # Python 3
   python -m http.server 8000
   # Luego abrir http://localhost:8000
