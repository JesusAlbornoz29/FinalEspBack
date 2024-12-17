
### En caso de error
#### Volver atrás cambios
Si necesitas revertir los últimos N cambios, puedes usar:

```bash
./scripts/drop_migration.sh down N 
```
Donde N es el número de migraciones que quieres revertir

Ejemplo:

```bash
# Revertir la última migración
./scripts/drop_migration.sh down 1

# Revertir las últimas 3 migraciones
./scripts/drop_migration.sh down 3
```
#### Forzar una versión específica
Si hay problemas graves con las migraciones, puedes forzar una versión específica:

```bash
./scripts/drop_migration.sh force VERSION
```
Donde VERSION es el número de la versión a la que quieres forzar la base de datos.

Ejemplo:

```bash
# Forzar a la versión 5
./scripts/drop_migration.sh force 5
```
> ⚠️ IMPORTANTE: Usar `force` solo en casos donde las migraciones están en un estado inconsistente y no se pueden resolver con `down`. Este comando puede causar pérdida de datos si no se usa correctamente.

### [Mas información aquí](https://github.com/PicadosYa/PicadosYa-App/pull/26)

<!-- hola mundo -->
