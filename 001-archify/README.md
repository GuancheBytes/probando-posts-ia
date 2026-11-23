# 1/100 · Archify

**El post:** "Diagramas de arquitectura con IA que dan gusto enseñar". Visto en Instagram (midudev).

**Qué promete:** convierte tu proyecto en un HTML interactivo con modo claro/oscuro, animación y exportación a PNG, SVG, PDF o vídeo.

**Repo oficial:** [tt-a1i/archify](https://github.com/tt-a1i/archify) · Apache-2.0 · Funciona en Claude Code, Codex, OpenCode y Cursor. Probado con la v3.3.0.

## ✅ Pasos

### 1. Instálalo pidiéndoselo a tu agente
En Claude Code (o Cursor, Codex, OpenCode), escribe:
```
Install Archify for me by reading https://raw.githubusercontent.com/tt-a1i/archify/main/llms.txt
Instálalo solo para Claude Code y de forma global.
```
Confirma el alcance cuando te lo pida y reinicia el agente.

### 2. Pídele el diagrama, y sé concreto
```
Usa Archify para crear un diagrama de arquitectura interactivo de este repositorio.
Incluye TODAS las features, las tablas de la base de datos y el flujo principal.
Textos en español, tema oscuro. Guárdalo en docs/arquitectura.html y ábrelo.
```

### 3. Explora y exporta
Abre el HTML: cambia de tema, pulsa un nodo para ver su fichero y sus líneas, y exporta a PNG, SVG o vídeo vertical.

## 🧪 Mi prueba

Proyecto: [Mi Jardín](https://github.com/GuancheBytes/mi-jardin), una PWA en React + Supabase.

- Diagrama de arquitectura y de secuencia del flujo de riego, en [docs/](https://github.com/GuancheBytes/mi-jardin/tree/main/docs).
- 0 nodos inventados: las 18 rutas de `src/` que cita existen.
- Cada regeneración tardó unos 7 minutos.

## ⚖️ Veredicto: 7/10. Útil, pero no magia

**Ventajas**
- ✅ Fiel a tu código: no inventa.
- ✅ Cada nodo enlaza a su fichero y sus líneas.
- ✅ Un HTML que funciona sin conexión y exporta a PNG, SVG y vídeo.

**Desventajas**
- ❌ Si no se lo pides explícitamente, no cubre toda la app (a mí me mostró 2 de 7 features).
- ❌ En móvil no se lee.
- ❌ Unos 7 minutos por regeneración y HTML de unos 950 KB.

**Consejo:** en el prompt, pídele explícitamente que incluya todas las features y tablas.

---
[← Volver a todos los episodios](../)
