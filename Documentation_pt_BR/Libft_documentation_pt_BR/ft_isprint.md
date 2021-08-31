# ft_isprint

A função __*ft_sprint*__ (_isprint_ na Biblioteca Padrão do C) testa se o argumrnto passado corresponde a um caractere imprimível. Define-se como caractere imprimível, para essa função, um caractere pertencente a Tabela ASCII que possa se escrito na tela (inclui-se o espaço). A tabela abaixo resume esses caracteres:

**Caractere** | **Decimal** | | **Caractere** | **Decimal** | | **Caractere** | **Decimal**
--------------|-------------|-|---------------|------------ |-|---------------|------------
(espaço) | 32 | | ! | 33 | | " | 34
$ | 36 | | % | 37 | | & | 38
' | 39 | | ( | 40 | | ) | 41
\* | 42 | | + | 43 | | , | 44
\- | 45 | | . | 46 | | / | 47
0 | 48 | | 1 | 49 | | 2 | 50
3 | 51 | | 4 | 52 | | 5 | 53
6 | 54 | | 7 | 55 | | 8 | 56
9 | 57 | | : | 58 | | ; | 59
< | 60 | | = | 61 | | > | 62
? | 63 | | @ | 64 | | A | 65
B | 66 | | C | 67 | | D | 68
E | 69 | | F | 70 | | G | 71
H | 72 | | I | 73 | | J | 74
K | 75 | | L | 76 | | M | 77
N | 78 | | O | 79 | | P | 80
Q | 81 | | R | 82 | | S | 83
T | 84 | | U | 85 | | V | 86
W | 87 | | X | 88 | | Y | 89
Z | 90 | | [ | 91 | | \ | 92
] | 93 | | ^ | 94 | | _ | 95
` | 96 | | a | 97 | | b | 98
c | 99 | | d | 100 | | e | 101
f | 102 | | g | 103 | | h | 104
i | 105 | | j | 106 | | k | 107
l | 108 | | m | 109 | | n | 110
o | 111 | | p | 112 | | q | 113
r | 114 | | s | 115 | | t | 116
u | 117 | | v | 118 | | w | 119
x | 120 | | y | 121 | | z | 122
{ | 123 | | \| | 124 | | } | 125
~ | 126

###### Para utilizar a função "_isprint_" da Bibliotecaa Padrão do C:
~~~c
#include <ctype.h>
~~~

#
#### Cabeçalho:
~~~c
int	ft_isprint(int c);
~~~

#
#### Parâmetros:
 * **c** : Repesentação inteira (**int**) do caractere a ser testado.

#
#### Valor de Retorno:
A função *ft_isprint* retorna **zero** se o caracter testado não for um caractere imprimível, e um **valor diferente de zero** (*non-zero*) caso este seja uma caractere imprimível.

	obs.: É importante notar que um "non-zero value" pode assumir diferentes valores a depender da função
	considerada e do sistema operacional utilizado. Para o nosso projeto "libft", que será executado
	remotamente em um MAC da 42 são Paulo, utilizando o Apache Guacamole, um "non-zero" assumirá o valor 1.

Assim, temos para o retorno da função *ft_isalnum*:
* **0** : Caso o caractere testado não seja um caractere imprimível.
* **1** : Caso o caractere testado seja um caractere imprimível.
