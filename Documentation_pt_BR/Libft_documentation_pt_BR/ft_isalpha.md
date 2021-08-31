# ft_isalpha

A função __*ft_isalpha*__ (_isalpha_ na Biblioteca Padrão do C) testa se o argumento passado corresponde a um caractere alfabético. Define-se como caractere alfabético, para essa função, um caractere que corresponda a uma letra maiúscula ou minúscula usando como base a Tabela ASCII.

**Caractere** | **Decimal** | | **Caractere** | **Decimal**
--------------|-------------|-|---------------|------------
A | 65 | | a | 97
B | 66 | | b | 98
C | 67 | | c | 99
D | 68 | | d | 100
E | 69 | | e | 101
F | 70 | | f | 102
G | 71 | | g | 103
H | 72 | | h | 104
I | 73 | | i | 105
J | 74 | | j | 106
K | 75 | | k | 107
L | 76 | | l | 108
M | 77 | | m | 109
N | 78 | | n | 110
O | 79 | | o | 111
P | 80 | | p | 112
Q | 81 | | q | 113
R | 82 | | r | 114
R | 83 | | s | 115
T | 84 | | t | 116
U | 85 | | u | 117
V | 86 | | v | 118
W | 87 | | w | 119
X | 88 | | x | 120
Y | 89 | | y | 121
Z | 90 | | z | 122

###### Para utilizar a função "_isalpha_" da Bibliotecaa Padrão do C:
~~~c
#include <ctype.h>
~~~

#
#### Cabeçalho:
~~~c
int	ft_isalpha(int c);
~~~

#
#### Parâmetros:
 * **c** : Repesentação inteira (**int**) do caractere a ser testado.

#
#### Valor de Retorno:
A função *ft_isalpha* retorna **zero** se o caracter testado for não-alfabético e um **valor diferente de zero** (*non-zero*) caso este seja uma caractere alfabético.

	obs.: É importante notar que um "non-zero value" pode assumir diferentes valores a depender da função
	considerada e do sistema operacional utilizado. Para o nosso projeto "libft", que será executado
	remotamente em um MAC da 42 são Paulo, utilizando o Apache Guacamole, um "non-zero" assumirá o valor 1.

Assim, temos para o retorno da função *ft_isalpha*:
* **0** : Caso o caractere testado seja um caractere não-alfabético.
* **1** : Caso o caractere testado seja um caractere alfabético.
