Índice
1. Introdução	8

1.1	Proposta	12

1.2	Escopo	20

1.4	Visão Geral 24	


Introducão

Esse documento é o início da documentação completa para o site de apostas “Dona da Sorte”. Essa introdução vai explicar os principais conceitos e ferramentas que o site irá utilizar no seu funcionamento.


Proposta

Fazer um site de apostas com o foco principal sendo em apenas máquinas caça níqueis e “Lootboxes”.

Irá funcionar como qualquer máquina de caça níqueis genéricas em casinos: O usuário vai apostar uma certa quantidade de dinheiro na "máquina", e clicar para jogar. Irá ter várias máquinas com regras um pouco diferentes, mais a comum, a base/mãe de todas as máquinas que serão baseadas nela, terá 3 rodas com 8 combinações diferentes vencedoras, com a aposta mínima de 15 reais e a máxima de 200 reais.

O Modo “Lootbox” seria uma versão mais simplificada das máquinas de caça níqueis. Tem uma aposta fixa estática, com apenas uma roda de vários prêmios. Maior a raridade, Maior o prêmio. A comum, que será baseada para todas “Lootboxes”, terá 17 itens que podem ser rolados, com um preço para abrir uma sendo 25 reais.


Escopo

Planejamos um grande influxo de usuários pelo uso de anúncios e nosso sistema exclusivo de apostas comparado com nossos outros competidores.


Visão Geral

Em geral, Dona da Sorte é um site de apostas focando em um nicho que outros sites tentam se focar em vários e não são mestres de nenhum. Esperamos que com essa nossa mentalidade, consigamos fazer o melhor site de apostas focado em caça níqueis.

Caso de Uso

@startuml
actor Usuario as User
actor Admin as Admin
package DonaDaSorteWebSite {
usecase "Fazer Login/Sair da Conta/Criar Conta" as UC1
usecase "Selecionar Caça-Nique" as UC2
usecase "Selecionar Lootbox" as UC3
usecase "Colocar depositos/saldo" as UC4
usecase "Tirar depositos/saldo" as UC5
usecase "Configurações" as UC6
usecase "Apostar Um" as UC7
usecase "Apostar Maximo" as UC8
usecase "Tabela de Premios" as UC9
usecase "Resetar Aposta" as UC10
usecase "Girar roleta" as UC11
usecase "Comprar e Usar Lootbox" as UC12
usecase "Tabela de Premios" as UC13
usecase "Ver outras Lootboxes" as UC14
usecase "Recuperar senhar" as UC15
usecase "Ver lista de usuarios offline e online" as UC16
usecase "Historico de transações" as UC17
usecase "Ver dados dos usuarios" as UC18
usecase "Ver saldo restante do site" as UC19
usecase "Tirar site do ar para manutenção" UC20
}

User -> UC1
User -> UC2
User -> UC3
UC1 --> UC4
UC1 --> UC5
UC1 --> UC6
UC1 --> UC15
UC1 --> UC17
UC2 --> UC7
UC2 --> UC8
UC2 --> UC9
UC2 --> UC10
UC2 --> UC11
UC3 --> UC12
UC3 --> UC13
UC3 --> UC14
User -> Admin
Admin --> UC16
UC16 -> UC18
Admin --> UC19
Admin --> UC20
@enduml
