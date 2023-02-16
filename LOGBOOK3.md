# Trabalho realizado na Semana #3

## Identificação

- O CVE escolhido é o CVE-2016-4656.

- Os sistemas afetados são sistemas iOS inferiores ou iguais ao 9.3.4.

- Existe uma vulnerabilidade no kernel devido a um problema de corrupção de memória. Um invasor remoto não autenticado pode explorar isso convencendo um usuário a executar um aplicativo especialmente criado para causar uma condição de negação de serviço ou execução de código arbitrário. 

- Estas informações recolhidas podem ser enviadas para um servidor ou entidade externa para fins maliciosos.

## Catalogação

- Esta vulnerabilidade em questão foi inicialmente detectada nos iPhones em 2016, que continham iOS 9.3.4 ou inferior.

- Foi explorado pela empresa israelita NSO Group, sendo vendido para por entidades governamentais, cartéis e etc. com fins maliciosos.

- É a primeira falha de segurança que permite jailbreak de um iPhone e obrigou a Apple a forçar um patch de emergência (9.3.5) para resolução do mesmo.

- De acordo com a NVD , tem um nível de severidade de 7.8.


## Exploit

- Pegasus spyware é um software mais conhecido por explorar esse CVE, conseguindo controle completo de Iphones a partir de um jailbreak.

- Jailbreak é um processo onde se quebra a segurança da Apple nos iphones onde permite apenas aplicativos autorizados pela compania, abrindo brecha para instalação de software malicioso.

- Depois do Jailbreak, o pegasus instala de maneira autônoma um software de espionagem continua que envia dados confidenciais, como senhas, mensagens trocados, fotos e outros.


## Ataques

- Esta vulnerabilidade continha muitos debug strings de uma vulnerabilidade mais antiga e conhecida publicamente como CVE-2016-4655, mas uma análise mais detalhada revelou um novo zero-day.

- Criado e vendido pela empresa israelita de espionagem, foi utilizado por diversos governos como forma de espionagem para opositores políticos.

- Isto, não só levou ao banimento de países que podem fazer negócios com Israel, como também gerou preocupação com a liberdade política, tendo sido, por exemplo, um tema sensível nas eleições de 2022 do Brasil. 

## Referências

- https://www.trendmicro.com/en_us/research/21/i/analyzing-pegasus-spywares-zero-click-iphone-exploit-forcedentry.html

- https://www.istoedinheiro.com.br/como-o-escandalo-pegasus-fez-brasil-ser-banido-de-negocios-com-israel/

- https://citizenlab.ca/2016/08/million-dollar-dissident-iphone-zero-day-nso-group-uae/

- https://www.newsclick.in/An-Explainer-Pegasus-Spyware

- https://nvd.nist.gov/vuln/detail/CVE-2016-4656 

- https://www.exploit-db.com/exploits/44836


**Desafio 1:**

Entramos no CTF, na aba das Rules, encontramos a flag
flag{cb995b2293cd7ce3138f7aa57529eb116199962d704e35db7758ed1586b6f9f0}




