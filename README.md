# CSS 3D Images — Demo & Utilities ✅

¡Proyecto pequeño para probar efectos 3D con imágenes y un ejemplo de modelo recortado! 🎛️

---

## 🔎 Contenido del proyecto
- `index.html` — Página principal con:
  - Carrusel 3D de imágenes (rotando en el eje Y)
  - Área `model` que muestra un modelo recortado (`images/model.png`)
- `style.css` — Todos los estilos: carrusel 3D, flip-cards (si se usan), y estilos del `model`.
- `images/` — Imágenes usadas (stack images y variantes de `model`):
  - `stack1.jpg` … `stack4.jpg`
  - `model.png` 


---

## ▶️ Cómo lanzar la página (local)
Recomendado: servidor HTTP simple con Python.

```powershell
cd D:\Trabajo\CSS_3D
# inicia servidor en puerto 8000
python -m http.server 8000
# abre en navegador
start http://localhost:8000
```

Alternativa: en VS Code usa la extensión **Live Server** y abre `index.html` con "Open with Live Server".

---

## 🧪 Comprobaciones / Debugging
- Si no ves la imagen o las imágenes del carrusel:
  - Abre Developer Tools (F12) → pestaña **Network** → busca 404.
  - Asegúrate de servir desde la carpeta del proyecto (ver comando arriba).
- Si el servidor no arranca por permisos o path usa la ruta completa a Python (ej.: `C:\Python314\python.exe -m http.server 8000`).

---

## ✨ Tips y opciones
- Ajusta la variable CSS `--radius` en `.banner .slider` para separar más/menos las imágenes del carrusel.
- Cambia el tamaño del `model` editando `.banner .content .model { height: ... }`.
- Añade controles (pausa, velocidad) a la animación modificando la regla `animation: autoRun ...` en `style.css`.


