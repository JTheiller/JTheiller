# pascal-format-string

Um texto pode ser formatado preenchendo em partes identificadas pelo caracter percentual `%`, seguido do um outro caracter que determina o `tipo`, passando por parametro um array dinâmico correspondente;

## Uso

- uses: `System.SysUtils`
- Sintaxe: `format( Texto, [ Array ] )`
- Code: `format( 'Parabéns %s, sua idade: $d.', [ varUserString, varIdadeInteger ] )`
- Result: `Parabéns Joathan Theiller, sua idade: 30.'`

## Tipos

- `%d` (decimal)
O valor inteiro correspondente é convertido para uma string de dígitos decimais
- `%x` (hexadecimal)
O valor inteiro correspondente é convertido para uma string de dígitos hexadecimais
- `%p` (ponteiro)
O valor inteiro correspondente é convertido para uma string expressa com dígitos decimais
- `%s` (string)
A string correnpondente, caractere, ou valor Pchar é copiado para uma string
- `%e` (hexadecimal)
O valor de ponto flutuante correspondente é convertido para uma string.
- `%f` (ponto flutuate)
O valor de ponto flutuante correspondente é convertido para uma string.
- `%g` (geral)
O valor de ponto flutuante correspondente é convertido para uma string decimal menor possível usando notação de ponto flutuante ou exponencial.
- `%x` (número)
O valor de ponto flutuante correspondente é convertido para uma string de ponto flutuante mas usa também separador de milhares.
- `%m` (moeda)
O valor de ponto flutuante correspondente é convertido para uma string representando uma quantidade em dinheiro. A conversão é baseada nas configurações regionais.
