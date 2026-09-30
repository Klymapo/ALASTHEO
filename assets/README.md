# Assets

Material de referencia y entrada del pipeline.

## Referencias visuales

El índice maestro está en [`assets/references/`](references/README.md). Ahí se muestran y enlazan las referencias originales de Theo, Detective/Alastor, escala y reconstrucciones auxiliares.

Las imágenes fuente se mantienen en `Klymapo/alth-meta/refs/` para no duplicar binarios y conservar una sola fuente de verdad. ALASTHEO funciona como catálogo y documentación central de cómo deben usarse.

```text
assets/
└─ references/
   ├─ README.md
   ├─ characters/
   │  ├─ theo/
   │  └─ detective/
   ├─ scale/
   └─ sam3d/
      └─ theo/
```

No coloques aquí `.blend` ni `.glb` de producción: los modelos viven en `models/`. Los GLB experimentales externos, como las reconstrucciones SAM 3D, deben permanecer en su repositorio/branch de origen y enlazarse desde el catálogo.