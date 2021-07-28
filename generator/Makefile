##
## EPITECH PROJECT, 2020
## giantman
## File description:
## Makefile
##

CC	= gcc

SRC		=	src/initialize_cells.c	\
			src/err_handling.c		\
			src/utils.c				\
			src/create_imperfect.c	\

OBJ		=	$(SRC:.c=.o)

NAME		=	generator

CPPFLAGS	=	-I include/

CFLAGS =	-W -Wall -Wextra -Werror

all:	$(NAME)

$(NAME): $(OBJ)
	$(CC) -o $(NAME) $(SRC) $(CPPFLAGS) $(CFLAGS)

clean:
	$(RM) *.o
	$(RM) *~
	$(RM) *.gcda
	$(RM) *.gcno
	$(RM) src/*.o

fclean: clean
	$(RM) $(NAME)

re:	fclean all

.PHONY: all clean fclean re