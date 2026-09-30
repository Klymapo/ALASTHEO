# Estructura del repositorio

## `assets/`
Material de entrada que ayuda a construir los modelos, pero no es el modelo editable.

- `references/characters/<personaje>/`: turnarounds, siluetas, estudios faciales, color y proporciones.
- `references/props/`: objetos usados como anclas de escala o diseño.
- `references/environments/`: referencias de escenarios.
- `references/ui/`: referencias visuales de interfaces.

Las referencias originales deben conservarse sin edición cuando sea posible. Si una imagen se deriva de otra, indícalo en el nombre o en un README local.

## `models/`

- `source/<personaje>/`: `.blend` u otros archivos editables.
- `exports/<personaje>/`: `.glb`, `.gltf` y otros entregables.
- `previews/<personaje>/`: renders, turnarounds, vistas ortográficas y comparativas.

No mezcles archivos fuente y exportados en una misma carpeta.

## `scripts/`

- `blender/`: generación, limpieza, rig, materiales, exportación y captura.
- `pipeline/`: automatización entre herramientas.
- `utilities/`: scripts auxiliares que no pertenecen exclusivamente a Blender.

Cada script importante debe indicar entrada, salida y forma de ejecución.

## `tests/`

- `validation/`: mediciones, comprobaciones de malla, nombres, escala, rig o exportación.
- `captures/`: evidencia visual generada por pruebas.
- `fixtures/`: datos pequeños usados por pruebas reproducibles.

La evidencia temporal pesada no debe confundirse con un entregable final.

## `docs/`

- `production/`: libro de producción, calendarios y control de entregables.
- `design/`: reglas visuales, proporciones, paletas y decisiones de likeness.
- `pipeline/`: flujo técnico y automatizaciones.
- `decisions/`: decisiones importantes que convenga conservar de forma explícita.

## `archive/`
Iteraciones históricas, experimentos descartados y material reemplazado que todavía convenga conservar.

Un archivo debe pasar a `archive/` cuando ya no forme parte del flujo activo, no simplemente porque sea antiguo.

## Flujo recomendado por personaje

```text
assets/references/characters/theo/
models/source/theo/theo_v010.blend
models/exports/theo/theo_v010.glb
models/previews/theo/theo_v010_front.png
models/previews/theo/theo_v010_side.png
tests/validation/theo/
```

La misma lógica aplica a Alastor, Detective y futuros personajes.
