# delphi-parameters

Uma `procedure` ou `function`, pode ou não possuir parametros na sua assinatura, e existem varia formas diferentes de como declarar a sua assinatura.

Parametros são variáveis recebidas forma externa, que poderá ser utilizada no processamento;

### Sem parâmetro:
```pascal
procedure TNewClass.ProcedureName;
procedure TNewClass.ProcedureName();

function TNewClass.FunctionName: TNewClass;
function TNewClass.FunctionName(): TNewClass;
```

### Com parâmetro simples
#### Quando a variável criada fora do seu escopo e sera utilizada apenas como valor (copia), se reescrita não afetara o ponteiro de memoria da variavel base.
```pascal
procedure TNewClass.FunctionName(AValue: String);
begin
  AValue := AValue + ' Theiller';
end;

procedure TNewClass.Execute;
var
  LText: String;
begin
  LText := 'Joathan';
  TNewClass.FunctionName(LText);
  
  // Result: LText = Joathan
end;
```

### Com parâmetro constante (`const`):
#### Quando a variável criada fora do seu escopo e sera utilizada apenas como leitura, não podera ser reescrita dentro do método que a recebe
```pascal
procedure TNewClass.FunctionName(const AValue: String);
```

### Com parâmetro por referência de entrada (`var`):
#### Quando a variável é criada fora do seu escopo e pode ser inicializada com algum valor, mas tambem pode ser reescrita dentro do método que a recebe por parâmetro.
```pascal
class procedure TNewClass.FunctionName(var: AObject: String);
begin
  AObject := AObject + ' Theiller';
end;

procedure TNewClass.Execute;
var
  LText: String;
begin
  LText := 'Joathan';
  TNewClass.FunctionName(LText);
  // Result: LText = 'Joathan Theiller' 
end;
```

### Com parâmetro por referência para saída (`out`):
#### Quando a variável é criada fora do escopo não sendo inicializada, e a responsabilidade é total do método que a recebe para uso da rotina que lhe enviou.
```pascal
procedure TNewClass.FunctionName(out: AObject: String);
begin
  AObject := 'Joathan Theiller';
end;

procedure TNewClass.Execute;
var
  LText: String;
begin
  TNewClass.FunctionName(LText);     
  // Result: LText = Theiller
end;
```
