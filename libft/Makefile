# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: clora-ro <clora-ro@student.42lyon.fr>      +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/11/22 16:50:37 by clora-ro          #+#    #+#              #
#    Updated: 2022/04/20 16:41:15 by clora-ro         ###   ########lyon.fr    #
#                                                                              #
# **************************************************************************** #

NAME = libft.a

SRCS = ft_atoi.c			\
		ft_bzero.c			\
		ft_calloc.c			\
		ft_isalnum.c		\
		ft_isalpha.c		\
		ft_isascii.c		\
		ft_isdigit.c		\
		ft_isprint.c		\
		ft_isspace.c		\
		ft_itoa.c			\
		ft_memchr.c			\
		ft_memcmp.c			\
		ft_memcpy.c			\
		ft_memmove.c		\
		ft_memset.c			\
		ft_putchar_fd.c		\
		ft_putendl_fd.c		\
		ft_putnbr_fd.c		\
		ft_putstr.c			\
		ft_putstr_fd.c		\
		ft_strchr.c			\
		ft_strcmp.c			\
		ft_strdup.c			\
		ft_striteri.c		\
		ft_strjoin_free.c	\
		ft_strjoin.c		\
		ft_strlcat.c		\
		ft_strlcpy.c		\
		ft_strlen.c			\
		ft_strmapi.c		\
		ft_strncmp.c		\
		ft_strnstr.c		\
		ft_strrchr.c		\
		ft_strtrim.c		\
		ft_split.c			\
		ft_substr.c			\
		ft_tolower.c		\
		ft_toupper.c

OBJS := $(SRCS:.c=.o)

CC = gcc -Wall -Werror -Wextra

all : $(NAME)

$(NAME) :	$(OBJS)
			ar rcs $(NAME) $(OBJS)

%.o : %.c libft.h Makefile
	$(CC) -c $< -o $@

clean :
	rm -rf objs
	rm -rf $(addprefix objs/, $(OBJS))

fclean : clean
	rm -rf $(NAME)

re : fclean all

.PHONY : all clean fclean
			