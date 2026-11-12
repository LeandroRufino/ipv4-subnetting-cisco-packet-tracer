Planejamento e Implementação de Sub-redes IPv4

Sobre o projeto

Projeto prático desenvolvido no Cisco Packet Tracer com o objetivo de dividir uma rede IPv4 "/24" em cinco sub-redes "/27", configurar o endereçamento IP e estabelecer comunicação entre diferentes redes.

Objetivos

- Aplicar subnetting IPv4.
- Calcular endereços de rede, hosts e broadcast.
- Configurar endereços IP e gateways.
- Configurar interfaces de roteador.
- Validar a comunicação entre sub-redes.

Tecnologias e conceitos

- Cisco Packet Tracer 9.0
- IPv4
- Subnetting
- Endereçamento IP
- Roteamento entre redes
- ICMP (Ping)

Topologia

A rede foi construída utilizando:

- 1 roteador central.
- 5 switches.
- 10 computadores.
- 5 sub-redes IPv4.

Endereçamento IPv4

Rede original: "10.20.30.0/24"

Máscara utilizada: "255.255.255.224 (/27)"

Sub-rede| Endereço de rede| Gateway| Broadcast
1| 10.20.30.64/27| 10.20.30.65| 10.20.30.95
2| 10.20.30.96/27| 10.20.30.97| 10.20.30.127
3| 10.20.30.128/27| 10.20.30.129| 10.20.30.159
4| 10.20.30.160/27| 10.20.30.161| 10.20.30.191
5| 10.20.30.192/27| 10.20.30.193| 10.20.30.223

Configuração do roteador

Foram configuradas cinco interfaces GigabitEthernet, cada uma com um endereço IP correspondente ao gateway de sua sub-rede.

Todas as interfaces apresentaram estado operacional "up/up".

O roteamento foi realizado por meio das redes diretamente conectadas ao roteador.

Testes de conectividade

Foram realizados testes ICMP (Ping) entre computadores de diferentes sub-redes.

Resultados:

- PC8 ("10.20.30.66") para "10.20.30.131": 4 pacotes recebidos, 0% de perda.
- PC7 ("10.20.30.98") para "10.20.30.163": 4 pacotes recebidos, 0% de perda.

Os testes confirmaram a comunicação entre os diferentes segmentos da rede.

Arquivo do projeto

"Subrede_10.20.30.0.pkt"

Arquivo desenvolvido no Cisco Packet Tracer, disponibilizado para análise da topologia e das configurações.

Competências demonstradas

- Planejamento de redes IPv4.
- Divisão de redes em sub-redes (Subnetting).
- Configuração de endereçamento IP.
- Configuração de interfaces de roteador.
- Roteamento entre redes diretamente conectadas.
- Testes e validação de conectividade.

Ferramenta: Cisco Packet Tracer 9.0
Categoria: Redes de Computadores
Tipo: Projeto prático acadêmico
