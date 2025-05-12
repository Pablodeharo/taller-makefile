# Crear una variable
VARIABLE = hello
# Crear una regla para que ejecute un hello world
run:
	echo $(VARIABLE)
# Crear un directorio y un archivo
create:
	mkdir folder
	touch folder/file
# Establecer el contenido de un archivo (sobreescribir)
cat:
	echo "Hello world" > folder/file

# Añadir contenido a un archivo (sin sobreescribir)
append:
	echo "Hello Word" >> folder/file
# Mostrar el contenido de un archivo
show:
	cat folder/file
# Limpiar los archivos y directorios creados
rm:
	rm -rf folder
# Ejecutar clean y luego create
re: rm create
# Declarar PHONY
.PHONY: run create set append show rm re

