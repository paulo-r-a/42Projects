# ft_bzero

A função __*ft_bzero*__ (_bzero_ na Biblioteca Padrão do C) preenche com _0_ os __*n*__ Bytes contados a partir do Byte apontado pelo ponteiro __*b*__.

###### Para utilizar a função "_bzero_" da Biblioteca Padrão do C:
~~~c
#include <string.h>
~~~

#
#### Cabeçalho:
~~~c
void	bzero(void *b, size_t n);
~~~

#
#### Parâmetros:
* **b** : Um ponteiro para o início do bloco de memória a ser preenchido com _0_.
* **n** : O número de Bytes que serão preenchidos com _0_.

#
#### Valor de Retorno:
A função *ft_memset* não retorna nada (*void*).

#
#### Exemplos de uso:
~~~c
#include <string.h>

int	main(void)
{
	char	str[] = "0123456789";
	bzero(str, 7);
	return (0);
}
~~~
	"str" antes da chamada da função "bzero":

![bzero00](https://github.com/paulo-r-a/42Projects/blob/main/Images/Libft_images/bzero00.jpg?raw=true)

	"str" após a chamada da função "bzero":

![bzero01](https://github.com/paulo-r-a/42Projects/blob/main/Images/Libft_images/bzero01.jpg?raw=true)

Note que os _7_ (__n__) primeiros Bytes do bloco de memória apontado por _str_ (__b__) foram substituídos por _0_ ( _' \0 '_ ).
