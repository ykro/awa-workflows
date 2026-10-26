# awa-workflows

Workflow reutilizable del curso «Crea tu backend con FastAPI y Python asistido por IA» (AWA 2027).

`estatehub-cloudrun.yml` construye la imagen de EstateHub Cloud, se autentica en Google Cloud con Workload Identity Federation (sin llaves JSON) y despliega en Cloud Run por digest con los límites de costo del curso. Lo llama el `deploy.yml` de la plantilla de la Unidad 3:

```yaml
uses: ykro/awa-workflows/.github/workflows/estatehub-cloudrun.yml@v1
```

No lo copies ni lo modifiques en tu repositorio: la condición del proveedor de WIF solo acepta este archivo en la etiqueta `v1`.
