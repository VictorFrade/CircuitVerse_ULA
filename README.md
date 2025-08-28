# Link para projeto no CircuitVerse
https://circuitverse.org/users/328310/projects/circuitos_aula_8-0ef92a78-c6f4-412a-ad0f-ebebc1c09d4b

# Autores
Victor Frade e Eduardo Demeneghi - Turma 010 - Fundamentos de Sistemas Computacionais - 2025/2 - PUCRS

# Circuitos
<p>Circuitos feitos com a plataforma CircuitVerse, incluindo uma Unidade Lógica Aritmética.</p>

## Demultiplexador
![image_alt](Captura%20de%20tela%202025-08-28%20090819.png)
<p>Uma input (A) e um controle (op), duas outputs.</p>

### Casos
A = 0, op = 0, output1 = 0, output2 = 0;<br>
A = 1, op = 0, output1 = 1, output2 = 0;<br>
A = 0, op = 1, output1 = 0, output2 = 0;<br>
A = 1, op = 1, output1 = 0, output2 = 1.

## Comparador de 6 bits
![image_alt](Captura%20de%20tela%202025-08-28%20090958.png)
<p>Usa XNOR para comparar 6 bits, bit a bit, de dois binários.</p>

### Casos
Bit x de A = 0, Bit x de B = 0, compare = 1;<br>
Bit x de A = 1, Bit x de B = 1, compare = 1;<br>
Bit x de A = 0, Bit x de B = 1, compare = 0;<br>
Bit x de A = 1, Bit x de B = 0, compare = 0.
 - Os bits x de A e de B são bits de mesma posição em ambos números. Ex: A = 111110, B = 111110. Os zeros estão na mesma posição. <br>
 
## Somador 6 bits
![image_alt](Captura%20de%20tela%202025-08-28%20091423.png)
<p>Faz a soma de 6 bits, bit a bit, com carrys, de dois binários. Inicialmente, há um carry-in padrão 0.</p>

### Casos
A = 0, B = 0, carry-in = 0, sum = 0, carry-out = 0;<br>
A = 1, B = 0, carry-in = 0, sum = 1, carry-out = 0;<br>
A = 0, B = 0, carry-in = 1, sum = 1, carry-out = 0;<br>
A = 0, B = 1, carry-in = 0, sum = 1, carry-out = 0;<br>
A = 1, B = 1, carry-in = 0, sum = 0, carry-out = 1;<br>
A = 1, B = 0, carry-in = 1, sum = 0, carry-out = 1;<br>
A = 0, B = 1, carry-in = 1, sum = 0, carry-out = 1;<br>
A = 1, B = 1, carry-in = 1, sum = 1, carry-out = 1.

## Multiplexador 
![image_alt](Captura%20de%20tela%202025-08-28%20091643.png)
<p>Duas inputs (A e B) e um controle (op), uma output.</p>

### Casos
A = 0, B = 0, op = 0, output = 0;<br>
A = 1, B = 0, op = 0, output = 1;<br>
A = 0, B = 1, op = 0, output = 0;<br>
A = 0, B = 0, op = 1, output = 0;<br>
A = 1, B = 0, op = 1, output = 0;<br>
A = 1, B = 1, op = 0, output = 1;<br>
A = 0, B = 1, op = 1, output = 1;<br>
A = 1, B = 1, op = 1, output = 1.

## Somador
![image_alt](Captura%20de%20tela%202025-08-28%20091512.png)
<p>Faz uma soma simples de um bit com outro. Usado na ULA.</p>

### Casos
Idênticos ao somador de 6 bits.

## ULA
![image_alt](Captura%20de%20tela%202025-08-28%20091824.png)
<p>Realiza as operações and, or, compare e soma. Apresenta dois controles (op's).</p>
<p>Imagem mais aproximada:</p>

![image_alt](Captura%20de%20tela%202025-08-28%20091916.png)
<p>Essa imagem relaciona dois bits de dois binários distintos, com o primeiro op entrando nos dois multiplexadores iniciais e o segundo op
  no multiplexador final. Esse é o padrão para cada um dois 6 "blocos" da ULA.</p>
  
### Operações (ULA):
op 0-0: operação 'soma';<br>
op 0-1: operação 'or';<br>
op 1-0: operação 'compare';<br>
op 1-1: operação 'and'.<br>
 - Essas operações seguem a tabela-verdade das operações lógicas padrões correspondentes.

