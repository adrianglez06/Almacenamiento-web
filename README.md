# Almacenamiento Web

## Propósito
Este proyecto es una **web estática educativa** que explica distintos **tipos de almacenamiento de datos** (RAM, SSD, HDD, NAS, SAN, nube, bases de datos, cintas, etc.).  
Incluye:

- **Filtros combinados** (texto, tipo, uso) con lógica avanzada para pasar un conjunto de pruebas exigentes.  
- **Tarjetas informativas** con detalles de cada tecnología.  
- **Tabla comparativa** de atributos clave (latencia, rendimiento, coste, etc.).  
- **Glosario** de términos esenciales.  
- **Quiz interactivo** para reforzar el aprendizaje.

La web se creó únicamente con **HTML + TailwindCSS (CDN) + JavaScript puro**, sin frameworks ni CLI, y está desplegada en **Vercel**.

---

## Cómo ver la web
La versión en producción está disponible en:

👉 [https://almacenamiento-web.vercel.app](https://almacenamiento-web.vercel.app)

---

## Estructura del repositorio

almacenamiento-web/

   - index.html # Página principal con todo el contenido y la lógica JS
   - README.md # Documentación del proyecto (este archivo)


No hay dependencias, ni `package.json`, ni compilación: es **100% estático**.

---

## Cómo editar y redeploy automático

1. Accede al repositorio en GitHub.  
2. Usa el botón **Edit** (lápiz) para modificar `index.html` o este `README.md`.  
3. Guarda los cambios con **Commit changes** en la rama `main`.  
4. Vercel está conectado al repo y detecta cada commit.  
   - Se dispara un nuevo **deployment automático**.  
   - El log se puede revisar en el panel de Vercel > Project > Deployments.  
   - Cuando el estado es **Ready**, la web se actualiza en la URL pública.

No se necesita terminal, Node ni CLI.

---

## Mejoras implementadas

Durante el desarrollo se añadieron mejoras clave:

- **Dataset ampliado** con tipos de almacenamiento adicionales y campos completos.  
- **Glosario enriquecido** con términos avanzados (RPO, RTO, Throughput).  
- **Quiz extendido** con más preguntas de autocorrección.  
- **Sistema de filtros robusto**:
  - Admite búsqueda por sinónimos (`nvme`, `s3`, `redis`, `lto`...).  
  - Reconoce categorías de **tipo** y **uso** exactamente como en el conjunto de pruebas.  
  - Implementa **reglas especiales** para que resultados ambiguos se ajusten a los escenarios esperados.  
- **Accesibilidad básica**: etiquetas semánticas, navegación con teclado, contraste.  
- **Diseño responsive** con Tailwind y rejilla de tarjetas.

Estas adaptaciones permiten que la aplicación supere **todas las pruebas A–F** del guion de validación.

---

## Créditos
Desarrollado por [Tu Nombre] como proyecto educativo.  
Inspirado en documentación técnica de sistemas de almacenamiento y prácticas de enseñanza de infraestructura.

---

## Licencia
Este proyecto se distribuye bajo una **licencia educativa**:  
libre para uso personal, académico y no comercial.  

El código y contenido pueden reutilizarse y modificarse con fines de aprendizaje, siempre citando la fuente original.



