# Portal de distribuidores Amatu
Sitio estático (index.html) que usa Supabase (Auth + RLS) y se publica en Netlify.
1. Subir este directorio a un repositorio de GitHub.
2. En Netlify: Add new site > Import from Git > publish directory ".".
3. Supabase > Authentication: crear usuarios distribuidores y su fila en profiles.
La llave publicable de index.html es pública por diseño; la seguridad la dan las políticas RLS.
