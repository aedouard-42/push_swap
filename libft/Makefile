SRCS = ft_free_strs.c ft_split_set.c ft_is_space.c ft_inset.c  ft_atoi.c ft_isdigit.c ft_memcmp.c ft_strchr.c ft_strncmp.c ft_isalnum.c ft_isprint.c ft_memcpy.c ft_strrchr.c ft_isalpha.c ft_memccpy.c ft_memmove.c ft_strlcpy.c ft_tolower.c ft_isascii.c ft_memchr.c ft_memset.c ft_strlen.c ft_toupper.c ft_bzero.c ft_strlcat.c ft_strnstr.c ft_calloc.c ft_strdup.c ft_substr.c ft_strjoin.c ft_strtrim.c ft_split.c ft_itoa.c ft_strmapi.c ft_putchar_fd.c ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c ft_is_only_digits.c ft_rgb_to_int.c

BONUS_SRCS = ft_lstnew.c ft_lstadd_front.c ft_lstsize.c ft_lstlast.c ft_lstadd_back.c ft_lstdelone.c ft_lstclear.c ft_lstiter.c ft_lstmap.c

GNL_SRCS = GNL/get_next_line.c GNL/get_next_line_utils.c

OBJS = ${SRCS:.c=.o}

GNL_OBJS = ${GNL_SRCS:.c=.o}

BOBJS =${BONUS_SRCS:.c=.o}

NAME = libft.a

CC = gcc

CFLAGS = -Wall -Wextra -Werror -Iincludes -g3

.c.o :
			${CC} ${CFLAGS} -c $< -o ${<:.c=.o}

$(NAME):	${OBJS} ${GNL_OBJS}
			ar rcs ${NAME} ${OBJS} ${GNL_OBJS}

all:	${NAME}

clean :
		rm -rf ${OBJS}
		rm -rf ${BOBJS}
		rm -rf ${GNL_OBJS}

fclean:	clean
		rm -rf ${NAME}
		rm -rf ${BOBJS}
		rm -rf ${GNL_OBJS}

re:		fclean all

bonus: $(NAME) $(BOBJS)
		ar rcs $(NAME) ${BOBJS}

.PHONY: all clean fclean re
