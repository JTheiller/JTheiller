# REST (Representational State Transfer)
É um modelo a ser utilizado para se projetar arquiteturas de software distribuído, baseadas em comunicação via rede. Possui alguns princípios e restrições que devem ser utilizados para se garantir algumas características importantes em aplicações e serviços web, tais como: portabilidade, escalabilidade e desacoplamento.

## Comunicação Stateless
Requisições feitas por um cliente a um serviço REST devem conter todas as informações necessárias para que o servidor as interprete e as execute corretamente. Clientes não devem depender de dados previamente armazenados no servidor para processar uma requisição. Qualquer informação de estado deve ser mantida pelo cliente e não pelo servidor. Isso reduz a necessidade de grandes quantidades de recursos físicos, como memória e disco, e também melhora a escalabilidade de um serviço REST.

## Autenticação/autorização
Tokens de acesso são gerados pelo serviço REST e devem ser armazenados pelos clientes, via cookies ou HTML 5 Web Storage, devendo também ser enviados pelos clientes a cada nova requisição ao serviço.

Utilizar tecnologias e padrões como:
- `OAUTH`;
- `JWT` (JSON Web Token);
- `Keycloack`.

## Representações

Os três principais formatos suportados pela maioria dos serviços REST são:
- `HTML`;
- `XML`;
- `JSON`.

## Recursos
A identificação do recurso deve ser feita utilizando-se o conceito de URI (Uniform Resource Identifier).

Utilizar padrão de nomeclatura, minusculo, plural e estrutura.

Exemplo:
- `http://example.org/produtos/1`

## Verbos
- `GET`: Obter os dados de um recurso.
- `POST`: Criar um novo recurso.
- `PUT`: Substituir os dados de um determinado recurso.
- `PATCH`: Atualizar parcialmente um determinado recurso.
- `DELETE`: Excluir um determinado recurso.
- `HEAD`: Similar ao GET, mas utilizado apenas para se obter os cabeçalhos de resposta, sem os dados em si.
- `OPTIONS`: Obter quais manipulações podem ser realizadas em um determinado recurso.
- `CONNECT`: O método CONNECT estabelece um túnel para o servidor identificado pelo recurso de destino.
- `TRACE`: O método TRACE executa um teste de chamada loop-back junto com o caminho para o recurso de destino.

## HTTP - StatusCode

Existem inúmeros status de retorno para as requisições, seguem uma determinada classe e semantica, veja alguns exemplos:

- `2xx`: Indica que a requisição foi processada com sucesso.
  - 200: OK - GET, PUT e DELETE executadas com sucesso.
  - 201: Created - POST, quando um novo recurso é criado com sucesso.
  - 206: Partial Content - GET que devolvem apenas uma parte do conteúdo de um recurso.
- `3xx`: Indica ao cliente uma ação a ser tomada para que a requisição possa ser concluída.
  - 302: Found - Requisições feitas à URIs antigas, que foram alteradas.
- `4xx`: Indica erro(s) na requisição causado(s) pelo cliente.
  - 400: Bad Request - Requisições cujas informações enviadas pelo cliente sejam invalidas.
  - 401: Unauthorized - Em requisições que exigem autenticação, mas seus dados não foram fornecidos.
  - 403: Forbidden - Em requisições que o cliente não tem permissão de acesso ao recurso solicitado.
  - 404: Not Found - Em requisições cuja URI de um determinado recurso seja inválida.
- `5xx`: Indica que a requisição não foi concluída devido a erro(s) ocorrido(s) no servidor.
  - 500: Internal Server Error - Em requisições onde um erro tenha ocorrido no servidor.
  - 503: Service Unavailable - Em requisições feitas a um serviço que esta fora do ar, para manutenção ou sobrecarga.

## Fontes
- www.alura.com.br
- https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Methods
- https://pt.wikipedia.org/wiki/REST
