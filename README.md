# Quantum Tarot Nexus — Landing

Esta carpeta está lista para publicarse gratuitamente con GitHub Pages.

## 1. Conectar el botón con Genially

Abre `index.html` con el Bloc de notas.

Busca:

```js
const CAMPUS_URL = "PEGA_AQUI_LA_URL_PUBLICA_DE_TU_GENIALLY";
```

Reemplaza el texto por el enlace público de tu Genially. Guarda el archivo.

## 2. Publicarla en GitHub Pages

1. Crea una cuenta en GitHub si todavía no tienes una.
2. Crea un repositorio público llamado `quantumtarotnexus`.
3. Sube:
   - `index.html`
   - la carpeta `assets`
4. En el repositorio, entra a:
   `Settings > Pages`
5. En “Build and deployment” selecciona:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
6. Pulsa `Save`.

GitHub generará una dirección parecida a:
`https://TU-USUARIO.github.io/quantumtarotnexus/`

## 3. Conectar quantumtarotnexus.com desde Porkbun

Cuando GitHub Pages ya funcione:

### En GitHub

1. Vuelve a `Settings > Pages`.
2. En “Custom domain” escribe:
   `quantumtarotnexus.com`
3. Guarda.

### En Porkbun DNS

Elimina únicamente los registros web actuales que apunten a `uixie.porkbun.com`
(ALIAS y CNAME comodín). No elimines los registros MX ni TXT del correo.

Agrega estos cuatro registros `A` para el dominio raíz:

- Host: vacío o `@` — Answer: `185.199.108.153`
- Host: vacío o `@` — Answer: `185.199.109.153`
- Host: vacío o `@` — Answer: `185.199.110.153`
- Host: vacío o `@` — Answer: `185.199.111.153`

Agrega un registro `CNAME`:

- Host: `www`
- Answer: `TU-USUARIO.github.io`

La propagación puede tardar desde algunos minutos hasta 24 horas.

## Contenido

La landing usa una imagen única en alta resolución y una zona invisible,
adaptable a cualquier pantalla, sobre el botón “COMENZAR EL VIAJE”.
