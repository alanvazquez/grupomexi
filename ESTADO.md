# Estado de implementación Grupo Mexi / Aquapractika

## Fuente y copia

- Fuente original, conservada intacta: `F:\Backups\GRUPOMEXI_NEW_SITE\grupomexi_mockup`.
- Copia de trabajo: `C:\Users\carlo\OneDrive\AQUAPRACTIKA\GRUPOMEXI_IMPLEMENTACION\grupomexi_mockup`.
- La carpeta `mexi_test` se consultó como referencia histórica; no se modificó.
- Esta carpeta contiene el mockup y sus recursos estáticos, no el backend de cotización.

## L01-A — Marca y transición

Implementado en `index.html`, `contacto.html` y `css/grupomexi-transition.css`:

- Aviso visible: «Grupo Mexi ahora es Aquapractika» con enlace a `https://aquapractika.mx/`.
- Marca Aquapractika acompañada de «Antes Grupo Mexi».
- Se conserva el title de portada y el H1 exactos definidos por el usuario.
- La portada mantiene su identidad histórica y explica la continuidad del contenido.
- Los CTA de contacto dirigen directamente a WhatsApp (+52 921 274 2410); se retiraron los botones de formulario/correo porque la vía preferida de atención es WhatsApp.
- Contacto mantiene teléfono y dirección heredados de Grupo Mexi; el correo dejó de mostrarse como canal de contacto principal.

Estado: implementado en HTML/CSS; preview pública revisada en móvil y escritorio después del despliegue.

## L01-B — Contenido y navegación histórica

Implementado en `index.html`:

- Recuperados los bloques de alevines Stirling/Pargo UNAM, diseño de módulos, mojarra por kilogramo, equipos y trabajos.
- Restablecidos los IDs `#hero`, `#features`, `#pricing`, `#screenshots`; agregados alias `#servicios` y `#trabajos`.
- Añadida sección de productos y cotización, sin publicar precios antiguos como vigentes.
- Conservadas imágenes locales de trabajos Grupo Mexi.
- Retirados testimonios y FAQ comerciales provenientes del mockup Aquapractika cuya vigencia no estaba confirmada.

Estado: contenido y estructura implementados; aceptación visual/funcional pendiente de preview.

## Pruebas y preview

- Inspección de código: title y H1 coinciden con el valor acordado; recursos principales y fotos de trabajos existen en la copia.
- No se ejecutaron pruebas de accesibilidad, Lighthouse ni apertura de WhatsApp desde un navegador real.
- Verificación pública: `grupomexi.com.mx`, `www.grupomexi.com.mx` y `contacto.html` respondieron HTTP 200; el H1 histórico se conserva y no quedan enlaces `forms.gle`.
- Preview responsive: el CTA de portada muestra solo «Visitar Aquapractika» y «WhatsApp» sin encimarse; el botón flotante permanece disponible.
- La consulta externa no pudo confirmar `aquapractika.mx` ni `presupuesto.php`; ver INVENTARIO_ENLACES_L01.md.
- El servidor local fue rechazado por permisos de red del entorno y el navegador bloqueó el protocolo `file:`. No se usó una ruta alternativa para eludir el bloqueo. La preview visual sigue pendiente.

## Pendiente

- L01-C: revisar cada destino y terminar el inventario de enlaces.
- L01-D: revisión y entrega global de L01.
- L05: verificar e integrar el backend del cotizador si se requiere un flujo distinto a WhatsApp.
- L06: SEO técnico, sitio de prueba y quitar el ID ficticio `G-XXXXXXXXXX`.
