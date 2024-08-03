<div name="#top-readme" align=center>
  <h1>Tributação para Programadores</h1>
</div>

Casa do Desenvolvedor | Tributacao para Programadores

> Tudo o que um programador de software precisa entender sobre tributação fiscal e documentos fiscais eletrônicos.

---

# Módulo 2 - Códigos Fiscais

> [PDF Módulo 2](assets/Modulo2.pdf)

## 📌 Table of Contents

- [Aula 01. CFOP](#aula-01-cfop)
  - [Primeiro Dígito](#primeiro-dígito)
  - [Segundo Dígito](#segundo-dígito)
  - [Terceiro e Quarto Dígito](#terceiro-e-quarto-dígito)
  - [Observações](#observações)
  - [Exemplos](#exemplos)
- [Aula 02. CRT](#aula-02-crt)
  - [Onde é informado o CRT? Qual campo?](#onde-é-informado-o-crt-qual-campo)
  - [Exemplo](#exemplo)
- [Aula 03. CST/CSOSN Tabela A](#aula-03-cstcsosn-tabela-a)
- [Aula 04. CST/CSOSN Tabela B](#aula-04-cstcsosn-tabela-b)
- [Aula 05. CSOSN](#aula-05-csosn)
- [Aula 06. NCM](#aula-06-ncm)

---

Códigos fiscais de preenchimento dos documentos fiscais.

- CFOP | Código Fiscal da Operação e Prestação de Serviço
- CRT | Código de Regime Tributário
- CST | Código de Situação Tributária
- CSOSN | Código de Situação da Operação no Simples Nacional
- NCM | Nomenclatura Comum do Mercosul
- CEST | Código Especificador da Substituição Tributária

# Aula 01. CFOP

> Código Fiscal da Operação e Prestação de Serviços

O **Código de Operações e Prestações** das entradas e saídas de produtos, nas operações internas, interestaduais e exterior, é representado por um código numérico que identifica a natureza de circulação da mercadoria ou a prestação de serviço de transporte.

Esse código obrigatoriamente deve ser informado em todos os documentos fiscais, tais como a **NF-e**, **CT-e**, **NFC-e**, **escrituração de livros** e **SPED Fiscal**, o que torna um fator determinante a respeito da tributação nas operações fiscais.

## Primeiro Dígito

Primeiro dígito evidencia o produto ou a atividade de entrada ou saída, e se a operação é interna, interestadual ou destinada ao exterior.

Para NF-e de Entrada:

  - 1000 | Entradas ou Prestações de Serviços para o Estado
  - 2000 | Entradas ou Prestações de Serviços para outros Estados
  - 3000 | Entradas ou Prestações de Serviços para o Exterior

Para NF-e de Saída:

- 5000 | Saídas ou Prestações de Serviços para o Estado
- 6000 | Saídas ou Prestações de Serviços para outros Estados
- 7000 | Saídas ou Prestações de Serviços para o Exterior

| Local Destinatário | Entrada | Saída |
|:------------------:|:-------:|:-----:|
|  Dentro do Estado  |    1    |   5   |
|   Fora do Estado   |    2    |   6   |
| Comércio Exterior  |    3    |   7   |

## Segundo Dígito

Segundo dígito evidencia qual é o grupo ou a operação referida no documento fiscal (qual o grupo que se enquadra).

## Terceiro e Quarto Dígito

Terceiro e quarto dígitos especificam o tipo de operação e/ou prestação.

## Observações

Num mesmo documento fiscal é possível ter mais de um CFOP, desde que sejam de **mesma natureza** (primeiro número).

A descrição da operação deve estar de acordo com o CFOP informado no item da nota.

O CFOP colocado na operação (<CFOP>) deve ser o mesmo da natureza da operação (<natOp>).
Se é dado como saída (venda), toda operação, todos os itens devem ser tratados como saída (venda).

## Exemplos

![img.png](assets/images/img.png)

![img.png](assets/images/img_2.png)

![img_1.png](assets/images/img_1.png)

<p>(<a href="#top-readme">back to top</a>)</p>

# Aula 02. CRT

> Código de Regime Tributário
 
Define a tributação de cada estabelecimento que está emitindo o documento fiscal eletrônico.

Estabelecimentos poderão ser:
- Simples Nacional
- Lucro Presumido
- Lucro Real

Se a empresa é contribuinte do Simples Nacional:
- **1** | Simples Nacional - Será preenchido pelo contribuinte quando for optante pelo Simples Nacional
- **2** | Simples Naciona - Excesso sublimite de receita bruta, será preenchido pelo contribuinte optante pelo Simples nacional que tiver ultrapassado o sublimite de receita bruta fixado pelo estado/DF e estiver impedido de recolher ICMS/ISS por esse regime (conforme art. 19 e 20 da Lei Complementar 123/06)
- **3** | Regime Normal - Será preenchido pelo contribuinte que não estiver na situação 1 ou 2.

## Onde é informado o CRT? Qual campo?

Campo **<CRT>**, colocando a classificação da empresa que está emitindo o documento fiscal (1, 2 ou 3).

- CRT 1 | Deve utilizar situação tributária informando CSOSN
- CRT 2, CRT 3  | Deve utilizar situação tributária informando CST

## Exemplo

![img.png](assets/images/img_3.png)

![img_1.png](assets/images/img_4.png)

<p>(<a href="#top-readme">back to top</a>)</p>

# Aula 03. CST/CSOSN Tabela A

> Código de Situação Tributária

Composto por dois números, mas recebe obrigatóriamente um número inicial.

- Primeiro Número | Origem da mercadoria ([Tabela A](#tabela-a-origem-da-mercadoria))
- Segundo e Terceiro Número | Tributação do ICSM

## Tabela A | Origem da Mercadoria

| Código | Descrição                                                                                                             |
|:------:|:----------------------------------------------------------------------------------------------------------------------|
|   0    | Nacional, exceto as indicadas nos códigos 3, 4, 5 e 8                                                                 |
|   1    | Estrangeira - Importação Direta, exceto a indicada no código 6                                                        |
|   2    | Estrangeira - Adquirida no Mercado Interno, exceto a indicada no código 7                                             |
|   3    | Nacional, Mercadoria ou Bem com Conteúdo de Importação superior a 40% e infoerior ou igual a 70%                      |
|   4    | Nacional, cuja produção tenha sido feita em conformidade com os processos produtivos de acordo com o Decr. Lei 288/67 |
|   5    | Nacional, Mercadoria ou Bem com Conteúdo de Importação Inferior ou Igual a 40%                                        |
|   6    | Estrangeira - Importação Direta, sem similar nacional, constante em lista de Resolução CAMEX e gás natural            |
|   7    | Estrangeira - Adquirida no Mercado Interno, sem similar nacional, constante em lista de Resolução CAMEX e gás natural |
|   8    | Nacional, Mercadoria ou BEm com Conteúdo de Importação Superior a 70%                                                 |

## Exemplo

![img.png](assets/images/img_5.png)

# Aula 04. CST/CSOSN Tabela B

# Aula 05. CSOSN

# Aula 06. NCM

<p>(<a href="#top-readme">back to top</a>)</p>
