# ft_isacii

A função __*ft_isascii*__ (_isascii_ na Biblioteca Padrão do C) testa se o argumento passado corresponde a um caractere da Tabela ASCII. Um caractere pertencente à Tabela ASCII tem como representação decimal um número entre 0 e 127 (contando ambos os extremos).

###### Para utilizar a função "_isascii_" da Bibliotecaa Padrão do C:
~~~c
#include <ctype.h>
~~~

#
#### Cabeçalho:
~~~c
int	ft_isascii(int c);
~~~

#
#### Parâmetros:
 * **c** : Repesentação inteira (**int**) do caractere a ser testado.

#
#### Valor de Retorno:
A função *ft_isascii* retorna **zero** se o caracter testado for um caractere pertencente a Tabela ASCII, e um **valor diferente de zero** (*non-zero*) caso este não seja um caractere ascii.

	obs.: É importante notar que um "non-zero value" pode assumir diferentes valores a depender da função
	considerada e do sistema operacional utilizado. Para o nosso projeto "libft", que será executado
	remotamente em um MAC da 42 são Paulo, utilizando o Apache Guacamole, um "non-zero" assumirá o valor 1.

Assim, temos para o retorno da função *ft_isascii*:
* **0** : Caso o caractere testado não seja um caractere ascii.
* **1** : Caso o caractere testado seja um caractere ascii.
