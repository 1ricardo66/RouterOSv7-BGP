# RouterOS v7 BGP
______________
#### Este repositório tem o foco de explanar brevemente as principais mudanças que ocorreram no BGP do sistema ROv6 P/ ROv7.

- **BGP-Networking**
  - **RO's v6:** *Na versão 6 você consegue informar os prefixos originados por seu ASN através do caminho* **Routing > BGP > Networks**
  - **RO's v7:** *Já na versão 7 para informar os prefixos que serão originados por seu ASN, é necessário criar uma address list, contendo a respectiva quebra do ASN, segue o caminho:* **IP > Firewall > Address Lists.**
- **Anuncio dos Prefixos**
  - **RO's v6:** *Na versão 6 é possível anunciar seu prefixo através da função __Synchronize__, sem que seja necessário adicionar de forma estática os prefixos que serão anunciados!*
  - **RO's v7:** *Já na versão 7, você precisa ter os prefixos que serão anunciados instalado em sua FIB de forma manual, pois não há mais a opção de Synchronize.*
- **Configuração de instancia**
  - **RO's v6:** *Na versão 6 é possível configurar uma nova instancia através do seguinte caminho:* **Routing > BGP > instances**
  - **RO's v7:** *Na versão 7 você pode configurar sua instancia diretamente em um peer, ou caso prefira, também é possível criar um template e associar o mesmo no peer desejado, através do seguinte caminho:* **Routing > BGP > Templates**

- **Configuração de Filtros**
  - **RO's v6:** *Na versão 6 possuimos uma GUI que nos permite manipular nossos anúncios*
  - **RO's v7:** *Na versão 7 os filtros devem ser configurados através de __CLI__, semelhante a um script*  

- **Configuração de Peer BGP**
  - **RO's v6:** *Na versão 6 há o campo __Routing > BGP > Peers__ onde possibilita estabelecer uma sessão*
  - **RO's v7:** *Já na versão 7 há o campo __Routing > BGP > Connection__*




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


![Configurar Networks](images/AS-Networks.png)
