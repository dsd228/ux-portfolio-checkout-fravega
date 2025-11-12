# Caso de Estudio UX: Optimización del Flujo de Checkout de Frávega.com

Este es un proyecto de análisis y rediseño conceptual enfocado en optimizar el flujo de checkout del e-commerce Frávega.com, con el objetivo de reducir la fricción y mejorar la tasa de conversión.

  * **Rol:** UX Analyst / Product Designer
  * **Proyecto:** Rediseño conceptual (no solicitado por la empresa).
  * **Objetivo:** Identificar puntos de dolor en el proceso de pago y proponer soluciones de alta fidelidad (wireframes) basadas en heurísticas de usabilidad.
  * **Herramientas:** Análisis Heurístico, Proto-Personas, User Journeys, Figma (Wireframing).

-----

## 1\. El Desafío: Fricción en la Conversión

El flujo de checkout es la etapa más crítica de un e-commerce. Cada segundo de duda o punto de fricción incrementa exponencialmente la tasa de abandono del carrito.

Tras un análisis inicial del flujo de Frávega, se detectó que el formulario de "Datos Personales" contenía ambigüedades y patrones de diseño que aumentaban la carga cognitiva del usuario, generando oportunidades de mejora claras.

## 2\. Proceso de Análisis UX

### Paso 1: Auditoría Heurística

Se realizó una auditoría del flujo de compra, enfocada en los principios de Usabilidad de Jakob Nielsen. Se identificaron 3 hallazgos críticos:

  * **Hallazgo 1 (Prevención de Errores):** El campo de "Móvil" es ambiguo. No especifica el formato (ej. "sin 0 y sin 15"), lo que genera validación de errores *reactiva* (después de que el usuario se equivoca) en lugar de *proactiva*.
  * **Hallazgo 2 (Visibilidad y Claridad):** La opción para solicitar "Factura A" está oculta tras un enlace de texto pequeño. Esto rompe la jerarquía visual del formulario (cuyo título es "Datos... y Tipo de Factura") y es fácil de ignorar para usuarios de empresa.
  * **Hallazgo 3 (Control del Usuario):** Un pop-up agresivo solicita el "Código Postal" de forma repetitiva durante la navegación, interrumpiendo al usuario en momentos no contextuales (ej. "vidrieriando") y generando alta frustración.

### Paso 2: Definición de Proto-Persona

Para empatizar con el usuario afectado, se definió una Proto-Persona basada en los hallazgos.

  * **Nombre:** Mariano, "El Comprador Ocupado".
  * **Perfil:** 42 años, dueño de una pyme.
  * **Contexto:** Está comprando equipamiento para su oficina (ej. una cafetera, monitores).
  * **Necesidad Crítica:** Necesita imperativamente **Factura A** para registrar el gasto.
  * **Comportamiento:** Impaciente. Valora la eficiencia y abandona procesos si se siente "trabado" o si el sitio parece poco profesional.

### Paso 3: Mapeo de Puntos de Dolor (User Journey)

Al mapear el "viaje" de Mariano por el checkout, los hallazgos se convierten en puntos de dolor emocionales:

1.  **Formulario de Teléfono:** 😕 **Confusión.** *"¿Cómo pongo mi número? ¿Con 11? ¿Sin 15?"*
2.  **Búsqueda de Factura A:** 😒 **Ansiedad.** *"¿Dónde cargo el CUIT? No encuentro la opción... ah, este link."*
3.  **Pop-up de CP:** 😠 **Frustración.** *"¡Otra vez este cartel\! ¡Ya lo cerré\! Lo compro en otro lado."*

## 3\. Ideación y Soluciones Propuestas

Basado en el análisis, se propusieron tres soluciones enfocadas en la claridad y la proactividad.

| Hallazgo | Solución Propuesta |
| :--- | :--- |
| **1. Teléfono Ambiguo** | **Añadir Microcopy Proactivo:** Incluir un texto de ayuda simple (Ej: *11 5566 7788 (sin 0 ni 15)*) y una máscara de campo `(__) ____-____` para guiar al usuario. |
| **2. Factura A Oculta** | **Aumentar la Jerarquía Visual:** Reemplazar el enlace de texto por un **Control Segmentado (Radio Button)**. Esto presenta la opción de forma clara e inmediata. |
| **3. Pop-up Invasivo** | **Solicitud Contextual:** Eliminar el pop-up y solicitar el Código Postal únicamente dentro del paso "Método de Envío", donde el usuario *espera* ingresarlo para calcular costos. |

## 4\. Prototipado (Wireframes)

Para visualizar las soluciones 1 y 2, se crearon wireframes de baja fidelidad en Figma. Se diseñó un flujo de dos pasos para la selección del tipo de factura.

### Propuesta de Rediseño:

El diseño eleva la jerarquía de "Tipo de Factura", soluciona la ambigüedad del teléfono y solo muestra los campos de CUIT/Razón Social condicionalmente, manteniendo la interfaz limpia.

#### Frame 1: Estado por Defecto (Consumidor Final)

Muestra el campo de teléfono con microcopy de ayuda y la opción "Consumidor Final" seleccionada por defecto.

(URL_DE_TU_IMAGEN_1_AQUI)

#### Frame 2: Flujo de Interacción (Factura A)

Al seleccionar "Factura A", la interfaz revela de forma limpia los campos condicionales (CUIT y Razón Social) necesarios para ese flujo.

(URL_DE_TU_IMAGEN_2_AQUI)

## 5\. Conclusiones y Próximos Pasos

Mediante cambios sutiles pero fundamentados en principios de UX, es posible reducir significativamente la carga cognitiva y la frustración del usuario, impactando directamente en la conversión.

**Próximos Pasos (Si este fuera un proyecto real):**

1.  **Test de Usabilidad:** Validar estos wireframes con 5 usuarios reales (idealmente que coincidan con la persona "Mariano") para medir el tiempo en la tarea y la percepción de facilidad.
2.  **Test A/B:** Implementar la nueva versión del formulario y medirla contra la versión original para cuantificar el impacto en la tasa de conversión del checkout.
