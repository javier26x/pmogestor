# PMO Gestor — Tracker Expansiones 5G Sitios Existentes

Dashboard PMO de una sola página (HTML autocontenido) para seguimiento de expansiones 5G en sitios existentes: FC, TSSR (4 disciplinas), RFI, Implementación, Asbuilt y Prioridades.

## Uso

1. Abrir `tracker-expansiones-5g.html` en el navegador (no requiere servidor).
2. Arrastrar el Excel `Proyectos_Expansiones_5G_Sitios_Existentes.xlsx` (usa la hoja `BASE`).
3. Navegar por las pestañas: Dashboard, TSSR, FC, RFI, Implementación, Asbuilt, Prioridad y Tabla.

Todo el procesamiento ocurre en el navegador; el Excel nunca se sube a ningún servidor (salvo que configures las integraciones).

## Integraciones opcionales (⚙️ Config)

Las credenciales **no están en el código**: se configuran con el botón ⚙️ del header y se guardan en `localStorage` del navegador.

| Integración | Para qué sirve |
|---|---|
| API Tracker | Sincroniza un snapshot para deltas día a día y reportes programados |
| WAHA | Envío de resúmenes por WhatsApp (manual y programado) |
| PocketBase | Historial de cambios campo a campo entre cargas |

Sin configurar, el tracker funciona completo en modo local y el header muestra `☁️ Sync off`.

## Columnas de la hoja BASE que consume

`ID_Sitio`, `Nombre`, `REGION`, `COMUNA`, `CLASIFICACIÓN`, `TIPO DE PROYECTO`, `Propietario Estructura`, `CONTRATISTA`, `PLAN`, `N°Prio.`, `Emisor TSSR`, `Fecha Emisión TSSR`, `Fecha Envío a Especialidades`, `EstatusIMPL`, `Fecha Apro IMPL`, fechas/estatus de RF, ECE y OOCC, `ESTATUS TSSR`, `ESTADO FC`, `ECE`, `RFI ACTUAL`, `FECHA RFI`, `ESTATUS IMPLE.`, `ESTATUS INT`, `FECHA INT`, columnas de Asbuilt y `COMENTARIO`.

Los responsables por disciplina se leen de la fila sobre los encabezados (fila 4).
