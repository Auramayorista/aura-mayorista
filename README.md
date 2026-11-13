# AURA MAYORISTA - tienda web

Archivos iniciales para publicar una tienda estática y conectar Supabase.

## Antes de publicar
1. Abrí `config.js` y reemplazá `PEGAR_PROJECT_URL` y `PEGAR_SB_PUBLISHABLE_KEY` por la URL del proyecto y la Publishable key de Supabase. No uses nunca una `sb_secret_` en el navegador.
2. En Supabase SQL Editor, ejecutá `catalogo_inicial.sql`. El script deja el stock como NULL porque no se proporcionó inventario real.
3. La cuenta creada en Authentication debe estar incluida en `public.admin_users` (ya se hizo en el proceso guiado).
4. El bucket `productos` debe ser público para descargar las fotos; las políticas creadas restringen las operaciones de escritura a administradores.

## Archivos
- `index.html`: catálogo, búsqueda, carrito, WhatsApp y administración autenticada.
- `config.js`: configuración pública de Supabase (Project URL + Publishable key).
- `catalogo_inicial.sql`: carga de los 268 productos del archivo de catálogo disponible.

## Nota
Los precios se tomaron de la planilla/catálogo disponible y deben revisarse antes de vender. No se asignó stock ficticio. Esta primera versión es una base funcional para probar; antes de abrir ventas al público hay que completar las claves, ejecutar el SQL y probar inicio de sesión, lectura, edición y carga de imágenes.
