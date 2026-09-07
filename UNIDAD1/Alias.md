# Explicación de las capturas: creando un alias en Bash

## Captura 1
<img src="1.png" alt="Captura 1">

Busco con `grep` si el alias `ll` ya existe en `~/.bashrc`; el primer intento falla por las comillas, el segundo encuentra uno viejo en la línea 81.

## Captura 2
<img src="2.png" alt="Captura 2">

Con `printf` y `>>` agrego al final de `~/.bashrc` un nuevo alias `ll='ls -lah --color=auto'`.

## Captura 3
<img src="3.png" alt="Captura 3">

Uso `source ~/.bashrc` para que la terminal actual cargue el cambio sin tener que reiniciarla.

## Captura 4
<img src="4.png" alt="Captura 4">

Con `type ll` confirmo que el alias ya apunta a `ls -lah --color=auto`, el nuevo.

## Captura 5
<img src="5.png" alt="Captura 5">

Con `alias` veo todos los alias activos y confirmo que `ll` quedó bien definido junto a los demás.