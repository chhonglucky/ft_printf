# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: chanhhon <chanhhon@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/10/20 16:33:02 by chanhhon          #+#    #+#              #
#    Updated: 2023/12/14 17:06:30 by chanhhon         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = cc
CFLAGS = -Wall -Wextra -Werror
NAME = libft.a
SRCS = ft_itoa.c ft_strlen.c
OBJS= $(SRCS:.c=.o)

all :	$(NAME)

$(NAME) : $(OBJS)
	ar -rcs $(NAME) $^
	@touch $@

%.o :	%.c
	@$(CC) $(CFLAGS) -c $< -o $@

clean :
	@rm -f $(OBJS)

fclean :	clean
	@rm -f $(NAME)

re :
	$(MAKE) fclean
	$(MAKE)	all

.PHONY : re fclean clean all