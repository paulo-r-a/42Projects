# ft_memset

A função __*ft_memset*__ (_memset_ na Biblioteca Padrão do C) escreve o valor __*c*__ (interpretado como um _unsigned char_) nos __*n*__ Bytes contados a partir do Byte apontado pelo ponteiro __*dest*__.

A função __*ft_menset*__ terá comportamento indefinido caso __*n*__ seja maior do que o comprimento do buffer __*dest*__. O comportamento também será indefinido se __*dest*__ for um ponteirp inválido.

###### Para utilizar a função "_memset_" da Biblioteca Padrão do C:
~~~c
#include <string.h>
~~~

#
#### Cabeçalho:
~~~c
void	*ft_memset(void *dest, int c, size_t n;
~~~

#
#### Parâmetros:
 * **dest** : Um ponteiro para o inicio do bloco de memória a ser preenchido com o "caractere" __c__.
 * **dest** : O valor (int) que (convertido para um unsigned char) será utilizado para preencher os __n__ Bytes a partir do endereço de memória apontado por __dest__.
 * **n** : O número de Bytes que serão preenchidos com o caractere __c__.

#
#### Valor de Retorno:
A função *ft_memset* retorna (__dest__) um ponteiro para o início do bloco de memória que foi preenchido com o caractere __c__.

#
#### Exemplo de Uso:
~~~c
#include <string.h>

int	main(void)
{
	char	str[] = "0123456789";
	memset(str, 80, 7);
	return (0);
}
~~~
	"str" antes da chamada da função "memset":

![memset00](https://github.com/paulo-r-a/42Projects/blob/main/Images/Libft_images/memset00.jpg?raw=true)

	"str" após a chamda da função memset:

![memset01](https://github.com/paulo-r-a/42Projects/blob/main/Images/Libft_images/memset01.jpg?raw=true)

Note que o caractere _'P'_ (__c__), que é o inteiro 80 convertido para unsigned char, preenche os _7_ (__n__) primeiros Bytes do bloco de memória apontado por _str_ (__dest__).
