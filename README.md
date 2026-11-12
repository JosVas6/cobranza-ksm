# cobranza k.s.m.

app web para llevar el recorrido de cobranza, guardar el historial por días y bajar cada día el excel con el mismo formato de la planilla.

## cómo publicarla en github pages

1. entra a github.com y toca **new repository**. nombre sugerido: `cobranza-ksm`. puede ser público: el código no trae datos de clientes.
2. en el repositorio nuevo toca **uploading an existing file**, arrastra `index.html` y `README.md`, y toca **commit changes**.
3. ve a **settings → pages**. en **source** elige **deploy from a branch**, rama **main**, carpeta **/ (root)**, y toca **save**.
4. espera uno o dos minutos. el link queda así: `https://TU-USUARIO.github.io/cobranza-ksm/`
5. abre el link, inicia sesión con el correo y la contraseña que creaste en supabase.

## primer uso

1. en la pestaña **recorrido** toca **cargar clientes desde mi planilla** y elige tu excel (sirve el que está en blanco).
2. si quieres pasar un día que ya hiciste, ve a **historial → importar un día desde excel**.
3. cada día: abre el link, anota los montos y detalles, y al terminar toca **descargar excel de este día**.

## datos y seguridad

- los datos se guardan en supabase, en tablas protegidas: solo se leen con tu usuario y contraseña.
- la url y la clave `publishable` que están en `index.html` son públicas por diseño y no dan acceso a tus datos sin iniciar sesión.
- el registro de usuarios nuevos está desactivado en supabase.
- un proyecto gratis de supabase puede pausarse si pasa una semana sin usarse. se reactiva desde su panel.
