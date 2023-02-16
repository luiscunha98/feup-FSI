# FSI - Environment Variable and Set-UID Program Lab

## Task 1: Manipulating Environment Variables

Variavéis Ambiente e o seus significados :

- printenv => imprime os valores de todas as variáveis de ambiente por default. podemos usá-la para imprimir o valor de apenas uma
- env => imprime todas as variáveis ​​de ambiente definidas antes da execução de um utility. podemos usá-la para imprimir o valor de apenas uma
- export => permite definir novas variáveis de ambiente, bem como modificar o valor das existentes
- unset => a variável de ambiente deixa de estar definida


## Task 2: Passing Environment Variables from Parent Process to Child Process

Foi observado que quando fork() é realizado num programa , não há diferença porque o processo filho copiou tudo do processo pai.
Um processo filho usa o mesmo Program Counter e os mesmos registos do CPU

## Task 3: Environment Variables and execve()

Variavel:
- execve() => necessita de ter as variáveis de ambiente como parâmetro. executa diretamente
vai imprimir todas as variáveis de ambiente, bem como os seus respetivos valores

## Task 4: Environment Variables and system()

system() => não precisa de ter as variáveis de ambiente como parâmetro. no entanto, chama a shell para executar o comando
vai imprimir todas as variáveis de ambiente, bem como os seus respetivos vaores

##  Task 5: Environment Variable and Set-UID Programs

Definimos um programa Set-UID , que permitiu correr certos programas com previlégios escalonados.
As variáveis de ambiemte não sofreram alterações

## Task 6: The PATH Environment Variable and Set-UID Programs

Executou-se o programa da Tas 6 com setUID e executamos o comando "ls" através de um system() o código executará com permissões de administrador, uma vez que definimos que o dono do ficheiro era o próprio administrador.

# CTF

## Desafio 2

**Desafio 2:**

1º Fizemos o reconhecimento para descobrir como deviamos proceder:
WordPress: 5.8.1

Plugins : 
WooCommerce Plugin 5.7.1
Booster for WooCommerce plugin 5.4.3

Usuarios: (Usamos a reviwes)
Orval Sanford
admin (Administrador)

2º Com o reconhecimento feito decidimos utilizar o CVE-2021-34646

3º Corremos o script python do CVE-2021-34646
Imagem Flag2_1

4º Conseguimos entrar na conta admin e fomos aos posts para encontrar o post com a flag:
flag{please don't bother me}
Imagem Flag2_2
