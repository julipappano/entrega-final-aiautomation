# Entrega Final (AI Automation, Coderhouse)

Corrector automático de ejercicios de alemán A1, con revisión humana (HITL) y dashboard de KPIs.

## Enlaces

| Recurso | Link | Acceso |
|---|---|---|
| Base de datos (Airtable, modo lectura) | https://airtable.com/appWDDplHIYZS05US/shr8rIVyPkIJCg2o1 | Público |
| Dashboard de KPIs (Airtable Interface) | https://airtable.com/appWDDplHIYZS05US/pag69nPeQm4zZKjdY | Solo colaboradores de la base (no publicado a la web por limitaciones de plan gratuito) |

## Contenido del repositorio

- `entrega_final_entregables1a5.pdf` — documento con los 5 entregables
- `workflow.json` — export del flujo de n8n
- `screenshots/` — evidencia del flujo en ejecución:
  - Historial de ejecuciones en n8n mostrando las 5+ corridas exitosas (reutilizada del Entregable 1)
  - Mensaje de Slack con el HITL en acción (notificación al docente con botones Aprobar/Rechazar)
  - Email de Gmail enviado al alumno con la corrección
  - Registro en Airtable mostrando el estado final (Finalizado) de un ejercicio
- `video-demo` — video con breve demostración del flujo

Toda esta explicación, junto con las capturas correspondientes, está también incluida dentro del PDF.

## Índice del PDF 
| # | Criterio (rúbrica) | Sección en el PDF | Páginas |
|---|---|---|---|
| 1 | Mapa de Arquitectura del Sistema | **Entregable 1: Diagrama y Arquitectura de Proceso**<br>— Propuesta de Automatización<br>— Diagrama de Arquitectura<br>— Descripción del Proceso con Capturas (Parte A: alumno, Parte B: IA, Parte C: HITL)<br>— Links y Evidencia Adicional (incluye evidencia de 5+ corridas) | 1–13 |
| 2 | Manual Operativo de Estructuras de Datos | **Entregable 2: Manual operativo de datos**<br>— 1. Esquema de tablas vinculadas de Airtable<br>— 2. Esquemas JSON de transferencia entre integraciones (2.1 a 2.14, incluye Split Out, búsqueda de regla gramatical, creación en Error log, Loop Over Items)<br>— 3. Resumen del flujo de datos (diagrama) | 14–26 |
| 3 | Estrategia de Optimización de Costos y Recursos | **Entregable 3: Costos**<br>— Cuadro comparativo de modelos (Gemini Flash-Lite, GPT-4o-mini, Claude Haiku, GPT-4o, Claude Sonnet, Batch API)<br>— Cálculo base de la estimación<br>— Ahorro estimado | 27–28 |
| 4 | Malla de Seguridad, Privacidad y Resiliencia | **Entregable 4: Documentación de Seguridad y Resiliencia**<br>— 1. Minimización de datos<br>— 2. Manejo de errores (Retry On Fail diferenciado por tipo de nodo)<br>— 3. Puntos de Human-in-the-loop<br>— 4. Test de estrés (5+ corridas, camino infeliz, caso de dos alumnos simultáneos) | 29–31 |
| 5 | Dashboard de Control Ejecutivo | **Entregable 5: Dashboard de KPIs**<br>— Volumen total de ejercicios<br>— Distribución de ejercicios por estado<br>— Corrección IA vs. docente<br>— Errores gramaticales más comunes | 32–33 |

**Nota sobre el Entregable 5:** el dashboard está publicado en Airtable pero no compartido a la web (requiere plan Team). El acceso es solo para colaboradores de la base. Las capturas de pantalla dentro del PDF sirven como evidencia visual del panel.
