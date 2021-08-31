# ft_memcpy

A função __*ft_memcpy*__ (_memcpy_ na Biblioteca Padrão do C) copia __*n*__ Bytes da cadeia de Bytes __*source*__ para a cadeia de Bytes __*dest*__. Entende-se como _cadeia de Bytes_ qualquer agrupamento de Bytes utilizados para armazenar informação, seja qual for o tipo de dado armazenado.

A função __*ft_memcpy*__ terá comportamento indefinido caso __*source*__ e __*dest*__ se sobreponham.

###### Para utilizar a função "_memcpy_" da Biblioteca Padrão do C:
~~~c
#include <string.h>
~~~

#
#### Cabeçalho:
~~~c
void	*ft_memcpy(void *dest, const void *source, size_t n);
~~~

#
#### Parâmetros:
* **dest** : A cadeia de Bytes para onde serão copiados os _n_ primeiros Bytes de _source_.
* **source** : A cadeia de Bytes da qual serão copiados os _n_ primeiros Bytes para _dest_.
* **n** : Número de Bytes que serão copiados de _source_ para _dest_.

#
#### Valor de Retorno:
A função *ft_memcpy* retorna (__dest__) um ponteiro para o início do bloco de memória para onde foram copiados os _n_ primeiros Bytes de _source_ .
