# Gestor de Almacén con Supabase y GitHub Pages

## 🚀 Cómo usar
1. Sube este proyecto a tu repositorio en GitHub.
2. Ve a **Settings → Pages**, selecciona:
   - Branch: `main`
   - Folder: `/ (root)`
3. Guarda y espera unos segundos.
4. Abre tu URL: `https://<tu-usuario>.github.io/<nombre-repo>/`.

## 🔥 Base de Datos
Este proyecto usa **Supabase**.
- URL: `https://vviflbcsksnecebtqady.supabase.co`
- API Key: Incluida en el HTML.

### Crear tablas en Supabase
Ejecuta en SQL Editor:
```sql
-- Catálogo
CREATE TABLE IF NOT EXISTS catalogo (
  id SERIAL PRIMARY KEY,
  nombre TEXT UNIQUE NOT NULL,
  precio NUMERIC NOT NULL
);

-- Registros
CREATE TABLE IF NOT EXISTS registros (
  id SERIAL PRIMARY KEY,
  nombre TEXT NOT NULL,
  cantidad INTEGER NOT NULL,
  precio NUMERIC NOT NULL,
  fecha TIMESTAMP NOT NULL,
  total NUMERIC NOT NULL
);
```
