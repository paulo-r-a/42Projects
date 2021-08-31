# ft_isdigit

A função __*ft_isdigit*__ (_isdigit_ na Biblioteca Padrão do C) testa se o argumento passado corresponde a um caractere numérico (decimal). Define-se como dígito decimal, para essa função, um caractere que corresponda a um número de 0 a 9 (contando o 9) usando como base a Tabela ASCII.

**Caractere** | **Decimal** |
--------------|-------------|
0 | 48
1 | 49
2 | 50
3 | 51
4 | 52
5 | 53
6 | 54
7 | 55
8 | 56
9 | 57

###### Para utilizar a função "_isdigit_" da Bibliotecaa Padrão do C:
~~~c
#include <ctype.h>
~~~


#
#### Cabeçalho:
~~~c
int	ft_isdigit(int c);
~~~

#
#### Parâmetros:
 * **c** : Repesentação inteira (**int**) do caractere a ser testado.

#
#### Valor de Retorno:
A função *ft_isdigit* retorna **zero** se o caractere testado não for um dígito decimal, e um **valor diferente de zero** (*non-zero*) caso este seja um dígito decimal.

	obs.: É importante notar que um "non-zero value" pode assumir diferentes valores a depender da função
	considerada e do sistema operacional utilizado. Para o nosso projeto "libft", que será executado
	remotamente em um MAC da 42 são Paulo, utilizando o Apache Guacamole, um "non-zero" assumirá o valor 1.

Assim, temos para o retorno da função *ft_isdigit*:
* **0** : Caso o caractere testado não seja um dígito decimal.
* **1** : Caso o caractere testado seja um dígito decimal.

