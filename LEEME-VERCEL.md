# Sitio académico de Geovanny Ortiz Mosquera — versión para Vercel

## Publicar con Vercel + GitHub (recomendado)
1. Descomprimir el ZIP. Los archivos `index.html`, `styles.css`, `script.js`, `vercel.json` y `assets/` deben estar en la raíz del repositorio (no dentro de otra carpeta adicional).
2. Crear un repositorio en GitHub, por ejemplo `web-academica-geovanny-ortiz`, y cargar allí **el contenido** de la carpeta descomprimida.
3. Entrar en https://vercel.com/new, iniciar sesión y seleccionar **Import Git Repository**. Autorizar GitHub si se solicita.
4. Importar el repositorio. Elegir **Framework Preset: Other**. En **Root Directory** usar `./`. Si el sitio no requiere compilación, dejar **Build Command** vacío (Override activado), e **Output Directory** como `.` o sin modificar si detecta la raíz. No se necesita instalación ni variables de entorno.
5. Pulsar **Deploy**. Vercel mostrará la URL asignada al finalizar.
6. Para actualizar el sitio, modificar y subir los archivos al mismo repositorio. Vercel desplegará los nuevos cambios automáticamente.

## Publicar mediante línea de comandos (alternativa)
Con Node.js instalado, situarse dentro de la carpeta del proyecto y ejecutar:
```
npm install -g vercel
vercel login
vercel --prod
```
Seguir las preguntas en pantalla. Esto requiere autorización de tu cuenta Vercel.

## Contenido y funcionamiento
- La web es **estática** y no necesita PHP, base de datos ni compilación.
- Los 20 registros de ponencias están en el arreglo `ponencias` de `script.js` (hay posibles registros repetidos, conservados según las capturas).
- La fotografía es `assets/geovanny-ortiz.png`. El contorno está fijo y el movimiento suave se aplica a la imagen interna, respetando la preferencia del sistema para reducir animaciones.
- Los enlaces a Google Académico, ORCID y ResearchGate están preparados.
- El aula académica y los recursos descargables no se publican por ahora.
- La imagen del proyecto es una ilustración referencial (`assets/proyecto-mipymes.svg`), no evidencia de resultados del estudio.
- Deben verificarse los detalles bibliográficos de las publicaciones antes de incorporarlos como citas completas.
- Antes de divulgar públicamente la web, revisar nombres, textos, enlaces y permisos de fotografía.

## Personalización
- `index.html`: contenidos principales, presentación, enlaces y secciones.
- `styles.css`: apariencia, colores, espaciados y animaciones.
- `script.js`: buscador, filtros, menú y tema claro/oscuro.
- `assets/`: fotografía, ilustración y símbolos de perfiles académicos.

**Importante:** esta entrega es un paquete preparado para despliegue; no se ha publicado en una cuenta Vercel.
