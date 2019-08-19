# Semana 1: O que é a Internet?

> Oi galera, eu sou o Davy, sou estudante de Ciências da Computação e estarei aqui, toda semana, trazendo resumos sobre a disciplina de __Transmissão de Dados__ para vocês.
>
> A Internet é uma rede de redes que conectam milhares de dispositivos ao redor do mundo.

Temos dispositivos como:

- servidores, computadores de mesa, impressoras etc
- dispositivos celulares, videogames etc
- e dispositivos não convencionais, como uma lâmpada elétrica, cortinas inteligentes e outros aparelhos conectados a rede no contexto da __Internet das Coisas__

Esses dispositivos, também chamado de _hosts_ ou sistemas finais, são conectados entre si por enlaces (links) de comunicação e comutadores de __pacotes__.

Quando um host possui dados para serem transmitidos a outro sistema final, o sistema emissor segmente esses dados e adiciona _bytes_ de cabeçalho a cada segmento. Já usando o jargão de rede de computadores, tais pacotes, são enviados através da rede ao sistema final de destino, onde são reagregados aos dados originais.

Um comutador de pacotes encaminha o pacote que está chegando em um de seus enlaces de comunicação de entrada para um de seus enlaces de comunicação de saída. Dos diversos tipos de comutadores de pacotes, dois recebem destaque na Internet de hoje:
    - os roteadores
    - e os comutadores de camada (ou _switches_)

Esses dois tipos de comutadores encaminham pacotes a seus destinos finais.

> As redes comutadas por pacotes (que transportam pacotes) são, de muitas maneiras, semelhantes às redes de transporte de rodovias, estradas e cruzamentos (que transportam veículos).

## O que é um Protocolo?

> Uma analogia humana

Em uma comunicação humana, temos:

- emissor: aquele que transmite a mensagem, falada, escrita ou gestual
- receptor: aquele que recebe a mensagem

__Exemplos:__

- conversações em telefones
- conversas com outras pessoas
- solicitação de serviços em autarquias

__Ideia chave:__

- envio de _mensagens_ 
- _ações_ quando a mensagem é recebida

De modo semelhante, também aplica-se tais conceitos:

- emissor: dispositivo que envia a mensagem
- receptor: dispositivo que decodifica a mensagem enviada pelo transmissor
- mensagem: as informações
- meio físico
- protocolo: conjunto de regras que definem o que, para onde, de onde etc.

> Para que a comunicação entre duas ou mais máquina ocorra, as máquinas devem utilizar o mesmo protocolo

- máquinas envolvidas
- regras para comunicações entre as máquinas
- governam as comunicações na Internet

__Ideia chave:__

- _formato_ da mensagem
- _sequenciamento_ das mensagens
- _ações_

> Protocolo é o conjunto de regras sobre o modo como se dará a comunicação entre as partes envolvidas. Protocolo é a "língua" dos computadores, ou seja, uma espécie de idioma que segue normas e padrões determinados. É através dos protocolos que é possível a comunicação entre um ou mais computadores.[¹](https://pt.wikibooks.org/wiki/Redes_de_computadores/Protocolos_e_servi%C3%A7os_de_rede)

<!--
    | Modelo OSI | Modelo TCP/IP | Modelo Híbrido |
| --- | --- | --- |
| Aplicação | Aplicação | Aplicação |
| Apresentação | | |
| Sessão | | Transporte |
| Transporte | Transporte | Inter-rede |
| Rede | Internet | Host/Rede |
| Enlace de Dados | Interface Física | Enlace de Dados |
| Física | | Física | 

 -->

## Bibliografia

- KUROSE, J. F. e ROSS, K. - Redes de Computadores e a Internet - 5ª Ed., Pearson, 2010.
- Wikibooks: Redes de computadores/Protocolos e serviços de rede. Disponível em: <https://pt.wikibooks.org/wiki/Redes_de_computadores/Protocolos_e_serviços_de_rede>.
