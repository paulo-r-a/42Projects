# ft_strlen

A função __*ft_strlen*__ (_strlen_ na Biblioteca Padrão do C) calcula o comprimento da string passada como parâmetro. Entende-se como comprimento de uma string o número de caracteres, contado do primeiro caractere, até o caractere nulo ('\0') que marca o fim da string (sem contar o caractere nulo).

###### Para utilizar a função "_strlen_" da Biblioteca Padrão do C:
~~~c
#include <string.h>
~~~

#
#### Cabeçalho:
~~~c
size_t	ft_strlen(const char *s);
~~~

	obs.: "size_t" é um tipo inteiro sem sinal que pode assumir tamanhos diferentes dependendo da arquitetura
	utilizada. Em um compilador de 32 bits syze_t terá 64 bits (4 Bytes) e será equivalente a um "unsigned int".
	Por outro lado, size_t terá 64 (8 Bytes) bits quando o compilador for de 64 bits. Isso seria o equivalente
	a um "unsigned long long". Dessa forma não podemos simplesmente substituir "size_t" por "unsigned int" no
	cabeçalho da função.

	Size_t é usado para representar tamanhos em Bytes (por isso um valor sempre positivo, uma vez que não
	existe tamanhos negativos.). É o tipo de retorno do operado "sizeof".

	Para utilizar o tipo "size_t" é necessário incluir uma das bibliotescas abaixo (lista não exaustiva):
	<stddef.h> , <stdio.h> , <stdlib.h> , <string.h>


#
#### Parâmetros:
 * **s** : Ponteiro para a string (endereço de memória do seu primeiro elemento), cujo comprimento deve ser calculado.

 #
#### Valor de Retorno:
A função *ft_strlen* retorna o número de caracteres (__*size_t*__) da string passada como argumento que precedem o caractere nulo (*\0*). Em outras palavras, retorna o comprimento da string.
