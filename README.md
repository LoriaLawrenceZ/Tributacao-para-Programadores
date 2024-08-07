<div name="#top-readme" align=center>
  <h1>Tributação para Programadores</h1>
</div>

Casa do Desenvolvedor | Tributacao para Programadores

> Tudo o que um programador de software precisa entender sobre tributação fiscal e documentos fiscais eletrônicos.

---

# Módulo 3 - ICMS

> [PDF Módulo 3](assets/Modulo3.pdf)

## 📌 Table of Contents

- [CST Tabela A | Origem da Mercadoria](#cst-tabela-a--origem-da-mercadoria)
  - [Observação](#observação)
- [CST Tabela B | Tributação pelo ICMS](#cst-tabela-b--tributação-pelo-icms)
- [CST `00` | Tributada Integralmente](#cst-00--tributada-integralmente)
- [CST `10` | Tributada e com Cobrança do ICMS por Substituição Tributária](#cst-10--tributada-e-com-cobrança-do-icms-por-substituição-tributária)

---

# CST Tabela A | Origem da Mercadoria

| Código | 	Descrição                                                                                                             |  % ICMS   |
|:------:|:-----------------------------------------------------------------------------------------------------------------------|:---------:|
|  `0`   | 	Nacional, exceto as indicadas nos códigos 3, 4, 5 e 8                                                                 | 7% ou 12% |
|  `1`   | 	Estrangeira - Importação Direta, exceto a indicada no código 6                                                        |    4%     |
|  `2`   | 	Estrangeira - Adquirida no Mercado Interno, exceto a indicada no código 7                                             |    4%     |
|  `3`   | 	Nacional, Mercadoria ou Bem com Conteúdo de Importação superior a 40% e infoerior ou igual a 70%                      |    4%     |
|  `4`   | 	Nacional, cuja produção tenha sido feita em conformidade com os processos produtivos de acordo com o Decr. Lei 288/67 | 7% ou 12% |
|  `5`   | 	Nacional, Mercadoria ou Bem com Conteúdo de Importação Inferior ou Igual a 40%                                        | 7% ou 12% |
|  `6`   | 	Estrangeira - Importação Direta, sem similar nacional, constante em lista de Resolução CAMEX e gás natural            | 7% ou 12% |
|  `7`   | 	Estrangeira - Adquirida no Mercado Interno, sem similar nacional, constante em lista de Resolução CAMEX e gás natural | 7% ou 12% |
|  `8`   | 	Nacional, Mercadoria ou BEm com Conteúdo de Importação Superior a 70%                                                 |    4%     |

## Observação

A redução da alíquota do ICMS para `4%` aplica-se exclusivamente às **operações interestaduais** que envolvem **produtos importados** ou produtos que contêm partes importadas.

`7%` ou `12%`
-  `7%` | Aplicado para operações interestaduais com destino às regiões Norte, Nordeste, Centro-Oeste e o estado do Espírito Santo.
-  `12%` | Aplicado para operações interestaduais com destino às demais regiões (Sul e Sudeste, exceto Espírito Santo).

<p>(<a href="#top-readme">back to top</a>)</p>

# CST Tabela B | Tributação pelo ICMS

| Código | Descrição                                                                     |
|:------:|:------------------------------------------------------------------------------|
|   00   | Tributada Integralmente                                                       |
|   10   | Tributada e com cobrança do ICMS por substituição tributária                  |
|   20   | Com redução de base de cálculo                                                |
|   30   | Isenta ou não tributada e com cobrança do ICMS por substituição tributária    |
|   40   | Isenta                                                                        |
|   41   | Não tributada                                                                 |
|   50   | Suspensão                                                                     |
|   51   | Diferimento                                                                   |
|   60   | ICMS cobrado anteriormente por substituição tributária                        |
|   70   | Com redução da base de cálculo e cobrança do ICMS por substituição tributária |
|   90   | Outras                                                                        |

<p>(<a href="#top-readme">back to top</a>)</p>

# CST `00` | Tributada Integralmente

- `<orig>` | **Origem da Mercadoria** ([Tabela A](#cst-tabela-a--origem-da-mercadoria))
- `<CST>` | **Código de Situação Tributária** ([Tabela B](#cst-tabela-b--tributação-pelo-icms))
- `<modBC>` | **Modalidade da Base de Cálculo**
  - `0` | Margem Valor Agregado
  - `1` | Pauta
  - `2` | Preço Tabelado Máximo
  - `3` | Valor da Operação
- `<vBC>` | **Valor da Base de Cálculo**
  - Valor da Base de Cálculo do ICMS
- `<pICMS>` | **Alíquota do ICMS**
  - Percentual do Imposto (ICMS)
- `<vICMS>` | **Valor do ICMS**
  - Imposto (valor do ICMS)

![img.png](assets/images/img.png)

<p>(<a href="#top-readme">back to top</a>)</p>

# CST `10` | Tributada e com Cobrança do ICMS por Substituição Tributária

- `<orig>` | **Origem da Mercadoria** ([Tabela A](#cst-tabela-a--origem-da-mercadoria))
- `<CST>` | **Código de Situação Tributária** ([Tabela B](#cst-tabela-b--tributação-pelo-icms))
- `<modBC>` | **Modalidade da Base de Cálculo**
    - `0` | Margem Valor Agregado
    - `1` | Pauta
    - `2` | Preço Tabelado Máximo
    - `3` | Valor da Operação
- `<vBC>` | **Valor da Base de Cálculo**
    - Valor da Base de Cálculo do ICMS
- `<pICMS>` | **Alíquota do ICMS**
    - Percentual do Imposto (ICMS)
- `<vICMS>` | **Valor do ICMS**
    - Valor do Imposto (ICMS)
- `<modBCST>` | **Modalidade da Base de Cálculo do ICMS Substituição Tributária**
    - `0` | Preço Tabelado ou Máximo Sugerido
    - `1` | Lista Negativa (valor)
    - `2` | Lista Positiva (valor)
    - `3` | Lista Neutra (valor)
    - `4` | Margem Valor Agregado (%)
      - Fundamental para calcular o valor da Substituição Tributária
      - Percentual definido com base em convênios e/ou protocolos definidos entre os dois estados (origem e destino) da mercadoria
    - `5` | Pauta (valor)
    - `6` | Valor da Operação
- `<vBCST>` | **Valor da Base de Cálculo do ICMS Substituição Tributária**
    - Valor definido pela Margem de Valor Agregado
      - vBC * Margem de Valor Agregado
- `<pICMSST>` | **Alíquota do Imposto do ICMS Substituição Tributária**
    - Alíquota do ICMS Substituição Tributária
- `<vICMSST>` | **Valor do ICMS Substituição Tributária**
    - Valor do ICMS Substituição Tributária **retido**
    - Valor calculado por:
      - (vBCST * pICMSST) - vICMS

![img_1.png](assets/images/img_1.png)

<p>(<a href="#top-readme">back to top</a>)</p>
