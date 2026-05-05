# Consulta de líneas telefónicas por CURP 🇲🇽

Herramienta web para verificar qué compañías de telefonía móvil tienen líneas registradas a nombre de una CURP en México, conforme al Registro Nacional de Usuarios (RENU).

## ¿Para qué sirve?

En México es obligatorio registrar las líneas telefónicas vinculadas a una CURP. Sin embargo, es posible que terceros registren líneas a tu nombre sin tu conocimiento. Esta app te permite revisar **todos los portales de las operadoras** de forma ordenada y llevar un control de cuáles ya revisaste.

## Características

- Lista completa de operadoras registradas ante el IFT / CRT
- Operadoras agrupadas por plataforma compartida (una sola visita cubre varias)
- Badge interactivo: haz clic para ver todas las operadoras de un grupo
- Filtros: todas / populares / pendientes / revisadas
- Buscador por nombre de operadora
- Progreso guardado automáticamente en el navegador (`localStorage`)
- Compatible con modo oscuro
- Sin dependencias externas — un solo archivo HTML

## Cómo usar

1. Abre `index.html` en tu navegador (o visita la versión publicada en GitHub Pages)
2. La vista inicia en **Pendientes** — las operadoras que aún no has revisado
3. Haz clic en **Ir al portal** para abrir la página de cada operadora
4. En cada portal ingresa tu CURP para consultar si hay líneas registradas
5. Si encuentras una línea que no reconoces, usa la opción de desvinculación dentro del mismo portal
6. Marca el ✓ al terminar de revisar cada portal — el progreso se guarda solo

## Operadoras incluidas

Se listan ~50 portales de consulta que agrupan más de 100 operadoras, incluyendo:

- **Populares**: Telcel, AT&T / Unefon / WIM, Movistar, Bait, Virgin Mobile, Izzi, Sky, OXXO CEL
- **Plataforma Altán Redes** (`rnu.altanredes.com/consulta`): cubre más de 80 OMVs en un solo portal
- **Otras plataformas independientes**: Oxio, Viasat, Tokamóvil, Red Aguila, MoBig, Mirlo, Newww, y más

> La lista se basa en el directorio publicado en [portal.crt.gob.mx](https://portal.crt.gob.mx/gestion-de-lineas-telefonicas-moviles). Si una operadora actualiza su URL o se agrega una nueva, puedes abrir un issue o PR.

## Instalación local

No requiere instalación. Descarga `index.html` y ábrelo directamente en cualquier navegador moderno.

```bash
git clone https://github.com/TU-USUARIO/consulta-curp.git
cd consulta-curp
open index.html   # macOS
# o simplemente arrastra el archivo a tu navegador
```

## Privacidad

- Esta app **no envía ningún dato a ningún servidor**
- Tu CURP nunca sale de tu navegador
- El progreso se guarda únicamente en el `localStorage` de tu dispositivo
- No tiene analíticas, cookies ni rastreadores

## Contribuir

¿Encontraste una URL desactualizada o falta una operadora? Abre un **issue** o manda un **pull request** editando el arreglo `G` dentro de `index.html`.

## Fuente oficial

Portal del IFT / CRT para gestión de líneas:  
[https://portal.crt.gob.mx/gestion-de-lineas-telefonicas-moviles](https://portal.crt.gob.mx/gestion-de-lineas-telefonicas-moviles)

---

Hecho con ayuda de [Claude](https://claude.ai) · Sin fines de lucro · Uso libre
