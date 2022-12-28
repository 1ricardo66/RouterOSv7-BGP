# RouterOS v7 BGP
______________
#### Este repositório tem o foco de explanar brevemente as principais mudanças que ocorreram no BGP do sistema ROv6 & ROv7.

- __BGP-Networking__
  - __RO's v6:__ _Na versão 6 você consegue informar os prefixos originados por seu ASN através do caminho_ __Routing > BGP > Networks__
  - __RO's v7:__ _Já na versão 7 para informar os prefixos que serão originados por seu ASN, é necessário criar uma address list, contendo a respectiva quebra do ASN, segue o caminho:_ __IP > Firewall > Address Lists.__
- __Anuncio dos Prefixos__
  - __RO's v6:__ _Na versão 6 é possível anunciar seu prefixo através da função **Synchronize**, sem que seja necessário adicionar de forma estática os prefixos que serão anunciados!_
  - __RO's v7:__ _Já na versão 7, você precisa ter os prefixos que serão anunciados instalado em sua FIB de forma manual, pois não há mais a opção de Synchronize._
- __Configuração de instancia__
  - __RO's v6:__
  - __RO's v7:__
- __Configuração de Local AS__
  - __RO's v6:__
  - __RO's v7:__




### Tabela de comandos úteis
______________
| Comando | Descrição |
| - | - |
| dst-len | Lorem ipsum |
| bgp-path-len | Quantidade atual de AS-Path |
| bgp-input-local-as |	Lorem ipsum |
| bgp-input-remote-as	| Lorem ipsum |
| bgp-output-local-as | Lorem ipsum |
| bgp-output-remote-as	| Lorem ipsum |
| ospf-metric	| Lorem ipsum|
| ospf-tag	| Lorem ipsum |
| rip-metric	| Lorem ipsum |
| rip-tag	| Lorem ipsum |

### Operadores Lógico
__________
| Operador | Descrição |
| - | - |
| && | - |
| \|\| | - |
| not | - |



______________

### Mudanças BGP RO's V7

- Configurar networks
- Configurar BlackRole
- Configurar Local AS
- Configurar Filtros (Input - Output)
  - Aplicar community
  - Aplicar AS-path
  - Aplicar Local-Preference
- Configurar peer EBGP  
