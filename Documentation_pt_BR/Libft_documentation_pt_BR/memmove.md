# ft_memmove

A função __*ft_memmove*__ (_memmove_ na Biblioteca Padrão do C) copia __*n*__ Bytes da cadeia de Bytes __*source*__ para a cadeia de Bytes __*dest*__. Entende-se como _cadeia de Bytes_ qualque agrupamento de Bytes utilizado para armazenar informação, seja qual for o tipo de dado armazenado.

Pode haver sobreposição entre as cadeias de Bytes. A cópia será sempre realizada sem perda de informação.

![memmove](https://github.com/paulo-r-a/42Projects/blob/main/Images/Libft_images/memmove.jpg?raw=true)


A imagem acima resume o comportamento da função _memmove_ (e consequentemente de *ft_memmove*) no caso de sobreposição. No exemplo, ao contrário do que ocorre quando se faz a cópia simples (Byte a Byte) para subistituição dos 4 primeiros elementos de _dest_ pelos 4 primeiros elementos de _source_. Ao se utilizar a função _memmove_ não se perde infromação. Os elementos copiados para _dest_ são aqueles que originalmente ocupavam as posições correspondentes em _source_.

###### Para utilizar a função "_memmove_" da Biblioteca Padrão do C:
~~~c
#include <string.h>
~~~

#
#### Cabeçalho:
~~~c
void	*ft_memmove(void *dest, const void *source, size_t n);
~~~

#### Parâmetros:
* **dest** : A cadeia de Bytes para onde serão copiados os _n_ primeiros Bytes de _source_.
* **source** : A cadeia de Bytes da qual serão copiados os _n_ primeiros Bytes para _dest_.
* **n** : Número de Bytes que serão copiados de _source_ para _dest_.

#
#### Valor de Retorno:
A função *ft_memmove* retorna (__dest__) um ponteiro para o início do bloco de memória para onde foram copiados os _n_ primeiros Bytes de _source_ .
