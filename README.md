# MuCloud Client Updates

Manifest y archivos del cliente del servidor MU Online privado **MuCloud** (Season 6 / OpenMU).

Este repo es consumido automaticamente por el **MuCloudLauncher.exe** para auto-actualizar el cliente de los jugadores. No es necesario hacer nada manualmente.

## Para jugadores

Descarga el cliente completo desde el link de MediaFire que te pasamos. El launcher se actualiza solo.

## Para el GM / mantenedor

Para publicar una actualizacion:

```powershell
.\publish-update.ps1 -Version "1.0.1" -Message "Descripcion breve del cambio"
```

El script:
1. Detecta archivos del cliente con cambios (vs el ultimo manifest)
2. Los sube como assets del Release de GitHub
3. Actualiza `manifest.json`
4. Hace git push

Los amigos veran el update la proxima vez que abran el launcher.
