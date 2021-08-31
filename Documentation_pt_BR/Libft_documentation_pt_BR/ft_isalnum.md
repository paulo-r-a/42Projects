# ft_isalnum

A função __*ft_isalnum*__ (_isalnum_ na Biblioteca Padrão do C) testa se o argumento passado corresponde a um caractere alfabético ou a um dígito decimal. Em outras palavras *ft_isalnum* testa se *ft_isalpha* ou *ft_isdigit* (uma delas) é verdadeira.

###### Para utilizar a função "_isalnum_" da Bibliotecaa Padrão do C:
~~~c
#include <ctype.h>
~~~

#
#### Cabeçalho:
~~~c
int	ft_isalnum(int c);
~~~

#
#### Parâmetros:
 * **c** : Repesentação inteira (**int**) do caractere a ser testado.

#
#### Valor de Retorno:
A função *ft_isalnum* retorna **zero** se o caracter testado for não-alfabético e também não for um digito decimal, e um **valor diferente de zero** (*non-zero*) caso este seja uma caractere alfabético ou um dígito decfimal.

	obs.: É importante notar que um "non-zero value" pode assumir diferentes valores a depender da função
	considerada e do sistema operacional utilizado. Para o nosso projeto "libft", que será executado
	remotamente em um MAC da 42 são Paulo, utilizando o Apache Guacamole, um "non-zero" assumirá o valor 1.

Assim, temos para o retorno da função *ft_isalnum*:
* **0** : Caso o caractere testado seja um caractere não-alfabético e também não seja um dígito decimal.
* **1** : Caso o caractere testado seja um caractere alfabético ou um dígito decimal.
