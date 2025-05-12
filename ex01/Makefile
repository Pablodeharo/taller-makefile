# Define el nombre del ejecutable
NAME=program

COMPILER = cc

# Define las flags del compilador
CFLAGS = -Werror -Wextra -Wall

# Lista de archivos fuente del proyecto
SRC = src/main.c src./utils.c

# Regla principal que compila el programa
all: $(NAME)

$(NAME):
	$(COMPILER) $(FLAGS) $(src) -O $(NAME)
# Elimina el archivo ejecutable
clean:
	rm -f $(NAME)

# Ejecuta clean y luego all para recompilar todo
re: clean all

# Ejecuta el programa
run: $(NAME)
	./$(NAME)
# Declara las reglas que no generan archivos
.PHONY: all clean re run