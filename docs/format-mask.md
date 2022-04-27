Uma máscara é dividida em `três partes`, separados por ponto e virgula `;`.
- I: Estrutura da máscara literal, Ex: `!\(999\)000-0000;0;_`;
- II: Determina se os caracteres fixos devem ser p;ersistidos, Ex: `/`, `-`, `(`,`)`;
- III: Determina como os caracteres em branco devem ser representados, podendo ser subistituído por outro, Ex: `_`, `@`,` `;

## Caracteres especiais

- `!` Faz com que a digitação da máscara fique parada no primeiro caracter, fazendo com que os caracteres digitados que se movam. Ex: !;0;_
- `>` Todos os caracteres alfabéticos digitados após este símbolo serão convertidos para maiúsculos. Ex: >aaa;0;_
- `<>` Anula o uso dos caracteres > e <. Ex: >aaa<>aaa;0;_
- `\` Utilizado para marcar determinado caractere não especial como fixo, não podendo sobrescrevê-lo. Ex: !\(999\)000-0000;0;_
- `L` Caracteres alfabéticos (A-Z, a-z.) de preenchimento obrigatório. Ex: LLL;1;_
- `l` (Letra ele minúscula) Caracteres alfabéticos (A-Z, a-z.) de preenchimento opcional. Ex: lll;1;_
- `A` Caracteres alfanuméricos (A-Z, a-z, 0-9) de preenchimento obrigatório. Ex: AAA;1;_
- `a` Caracteres alfanuméricos (A-Z, a-z, 0-9) de preenchimento opcional. Ex: aaa;1;_
- `C` Exige preenchimento obrigatório com qualquer caractere para a posição. Ex: CCC;1;_
- `c` Permite qualquer caractere para a posição de preenchimento opcional. Ex: ccc;1;_
- `0` Caracteres numéricos (0-9) de preenchimento obrigatório. Ex: 000;1;_
- `9` Caracteres numéricos (0-9) de preenchimento opcional. Ex: 999;1;_
- `#` Caracteres numéricos (0-9) e os sinais de – ou + de preenchimento opcional. Ex: ###;1;_
- `:` Utilizado como separador de horas, minutos e segundos. Ex: !00:00:00;1;_
- `/` Utilizado como separador de dia, mês e ano. Ex: !99/99/9999;1;_
- `;` Separa os três campos da máscara.
- `_` Caractere usado normalmente nas posições do campo ainda não preenchidas.
