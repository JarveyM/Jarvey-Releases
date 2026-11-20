# Jarvey Para Windows

Distribucion oficial de instaladores y avisos de actualizacion. Este repositorio
no contiene el codigo fuente, cuentas, claves ni proyectos BIM de los usuarios.

## Descargar

[Ultima version estable: Jarvey 1.0.24](https://github.com/JarveyM/Jarvey-Releases/releases/tag/v1.0.24)

[Instaladores y versiones publicadas](https://github.com/JarveyM/Jarvey-Releases/releases)

- Windows 10 21H1 / Windows 11, x64.
- Complemento opcional: Revit 2026.5 o posterior dentro de Revit 2026.
- Para actualizar una version anterior a 1.0.0-rc.2, instala manualmente una vez.
- Desde rc.2: Ayuda > Buscar actualizaciones, o aviso automatico en Jarvey.
- Jarvey 1.0.24 se ofrece tanto en el canal estable como en el de pruebas.
- Cierra Revit y termina de sincronizar antes de instalar. No se fuerza el cierre.
- Proyectos locales, Inbox y preferencias se conservan.

La version 1.0.24 reconoce parametros compartidos por su GUID de Revit entre
modelos y distingue homonimos de distinta identidad con etiquetas de variante.
Actualiza Jarvey y el publicador incluido; cierra y vuelve a abrir Revit, y
publica nuevamente los modelos para incorporar los GUID ausentes. No borres
ni recrees proyectos. Las condiciones numericas antiguas no se convierten
automaticamente: vuelve a elegir su propiedad para usar la identidad unificada.

Conserva el cierre corregido al actualizar desde Jarvey. Si el
instalador indica que Jarvey sigue abierto, cancela el instalador, sincroniza y
cierra Jarvey normalmente. Luego ejecuta el instalador descargado, sin
desinstalar ni borrar proyectos. Esto puede ser necesario la primera vez al
actualizar desde una version anterior a 1.0.23.

## Canales

`updates/stable.xml`: versiones aprobadas para uso general. No incluye candidatas.
`updates/preview.xml`: candidatas para pruebas. Se activa desde Ayuda en Jarvey;
el cambio se aplica al reiniciar. Instalar una candidata no la convierte en estable.

## Verificacion

Los instaladores de actualizacion se verifican con Ed25519 en Jarvey antes de
ejecutarse. Clave publica:

```text
keA1/LvkCxnAlfdGawTwVuUJG079Y2/c7XnWKBdYuuU=
```

Cada version incluye su SHA-256 y firma Ed25519. Esta firma no es un certificado
Windows Authenticode: Windows puede mostrar editor desconocido y pedir permisos
de administrador. No compartas contrasenas ni claves para instalar Jarvey.
