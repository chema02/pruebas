# PASOS A SEGUIR (2ª parte):
Recordad editar los ficheros que modifiqueis con Visual Studio Code
# Simular un conflicto

  Un conflicto aparece cuando en un mismo fichero existen versiones distintas en local y remoto.
  Vamos a simular uno y ver cómo lo podemos resolver:
1. En su repositorio de GitHub, edite el archivo carta_benvinguda.md
1. en la línea 4 añada: '* Añadimos esta línea para generar un conflicto'
    Ahora, en su repositorio local, con el Visual Studio Code, edite el mismo fichero, y añadirle el texto: "Archivo modificado por: Manel"
    Guarde (ctrl + s) haga commit y suba los cambios al repositorio remoto. * El conflicto está servido !!
    No nos deja, ya que hay contenidos diferentes en local y en remoto de fichero carta_benvinguda.md.
    Nos recomienda que bajamos los archivos que tenemos en remoto. 
    Haremos un pull desde origin hasta master.
    Visual Code Studio nos informa de la existencia del conflicto. Aparece una C sobre el fichero carta_benvinguda, en un apartado llamado 'Merge Changes'.
1. Editaremos el fichero, y aparecen las dos versiones. Tendremos que seleccionar 'manualmente' cuál es la versión correcta, o integrar nosotros los cambios.
    En este caso, yo he optado por aceptar los dos cambios.
1. Guardaremos el archivo resultante, haremos commit, y subiremos los cambios en el repo remoto.

# Crear una rama nueva, modificar ficheros, y juntarlos a master
Vamos a crear una rama nueva para programar una nueva funcionalidad y que no afecte a todo lo que ya llevamos hecho en la rama master. 
La llamaremos funcionalitat1. (Buscad el comando para crear una rama nueva)
Nos aseguramos que estamos a la nueva rama (Buscad el comando para cambiar a otra rama) y ...

1. Editamos el fichero carta_benvinguda.md y le añadimos el texto: "Texto añadido desde la rama funcionalitat1". Guardamos, y hacemos un commit.
1. Editamos el fichero Readme.md y le añadimos: "Texto añadido desde la rama funcionalitat1". Guardamos y hacemos un commit.
1. Ahora quisiéramos llevar estos cambios a la rama master:
        - haremos un checkout en la rama master.
        - desde master haremos un merge con funcionalitat1. De este modo llevaremos los cambios hechos en funcionalitat1 a la rama master.
1. Subiremos los cambios que hay en master a GitHub
1. Comprobaremos en github que se han subido correctamente los cambios.
