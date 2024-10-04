<div align="justify">

# Vincular un repositorio local de git en github

## Paso 1: Importar la máquina virtual

   ![<importar>](<Imagenes\Importar.png>)

## Paso 2: Crear un repositorio en GitHub

   ![<importar>](<Imagenes\CrearRepositorio.png>)

   ![<importar>](<Imagenes\Repositorio.png>)


## Paso 3: Clonar el repositorio en local
   ```
   Pro@jpexposito-VirtualBox:-$ git clone https://github.com/nexphernandez/repositorio-ejercicio-1
   Cloning into 'repositorio-ejercicio-1'...
   remote: Enumerating objects: 3, done.
   remote: Counting objects: 100% (3/3), done.
   remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
   Receiving objects: 100% (3/3), done.
   ```
## Paso 4: Modificar el archivo README.md
   ```
   Pro@jpexposito-VirtualBox:-$ gir add READMe.md

   Pro@jpexposito-VirtualBox:-$ git comit -m "Añadir título y descripcion al README"
   [main 63d092e] Añadir titulo y descripción al README
   1 file changed, 3 insertions(+), 1 deletion(-)

   Pro@jpexposito-VirtualBox:-$ git push origin main
   fatal: User canceled device code authetication
   Username for 'https://github.com': git push origin main
   Password for 'https://git push origin main@github.com':
   Pro@jpexposito-VirtuallBox:-$ git push origin main
   Enumerating object: 5, done.
   Counting objects: 100% (5/5), done.
   Delta compression using up to 24 threads
   Compressing objects: 100% (2/2), done.
   Writing objects: 100% (3/3), 365 bytes | 365.00 KiB/s, done.
   Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
   To https://github.com/nexphernandez/repositorio-ejercicio-1
      e404d24..63d092e  main -> main
   ```

   ![<importar>](<Imagenes\RepositorioModificado.png>)

## Paso 5: Editar el README.md desde GitHub

   ![<importar>](<Imagenes\EditGitHub.png>)

## Paso 6: Actualizar el repositorio local con los cambios remotos
```
   Pro@jpexposito-VirtualBox:-$ git pull origin main
   remote: Enumerating objects: 5, done.
   remote: Counting objects: 100% (5/5), done.
   remote: Compresing objects: 100% (2/2), done
   remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
   Unpacking objects: 100% (3/3), 1.02 KiB | 261.00 KiB/s, done.
   From https://github.com/nexphernanndez/repositorio-ejercicio-1
   * branch            main        -> FETCH_HEAD
      63d092e..c230584  main        -> origin/main
   Updating 63d092e..c230584
   Fast-forward
   README.md | 4 +++-
   1 file changed, 3 insertions(+), 1 deletion(-)

   ````

## Paso 7: Añadir un nuevo cambio en local y subirlo a GitHub

   ![<importar>](<Imagenes\UltimoPaso.png>)

   ```
   Pro@jpexposito-VirtualBox:-$ gir add READMe.md

   Pro@jpexposito-VirtualBox:-$ git comit -m "Añadir última línea al README desde local"
   [main 63d092e] Añadir última línea del README desde local
   1 file changed, 2 insertions(+)

   $ git push origin main
   Enumerating object: 5, done.
   Counting objects: 100% (5/5), done.
   Delta compression using up to 24 threads
   Compressing objects: 100% (2/2), done.
   Writing objects: 100% (3/3), 365 bytes | 365.00 KiB/s, done.
   Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
   remote: Resolving deltas: 100% (1/1), completed with 1 local objects.
   To https://github.com/nexphernandez/repositorio-ejercicio-1
      c230584..3a9852e  main -> main

   ```
</div>