# Dulces Celis

Tienda estática Mobile-First para catálogo, pedidos por WhatsApp y administración básica.

## Configuración

Edita `SUPABASE_URL` y `SUPABASE_ANON_KEY` al inicio de `index.html` y `admin.html`. Solo debe usarse la clave publicable/anon; nunca una `service_role`.

El PIN inicial del panel es `2643`. Cambia `ADMIN_PIN` en `admin.html` antes de publicar si quieres otro.

## Supuestos

Los precios no aparecen en la ficha de marca; los valores semilla son iniciales y editables desde el panel. Los plazos sí se tomaron de la ficha: marquesas 24 horas, galletas y brownies 24 horas, tortas clásicas 48 horas y tortas temáticas 4 días. Las tortas temáticas piden porciones, sabor, motivo, nombre y edad. Las políticas RLS públicas se ajustan al flujo solicitado, pero el PIN en frontend no sustituye autenticación real para un entorno con información sensible.

## Archivos

- `index.html`: tienda y checkout por WhatsApp.
- `admin.html`: panel de productos y pedidos.
- `schema.sql`: esquema, RLS, permisos y datos semilla.
- `assets/`: logo y fotos copiadas del catálogo local.
