# DIO INVEST: Simulador de Investimentos em FIIs

Este projeto foi desenvolvido como parte do curso Excel com Inteligência Artificial, com o objetivo de criar uma ferramenta automatizada em Excel que auxilia o investidor a simular aportes mensais, rentabilidade acumulada e distribuição de carteira em Fundos Imobiliários (FIIs), de acordo com o perfil de investimento.

A planilha DIO INVEST permite ao usuário inserir informações básicas como: salário, percentual destinado a investimentos e tempo de aplicação, e visualizar projeções de crescimento patrimonial, dividendos e cenários de longo prazo.
Além disso, o simulador adapta automaticamente as alocações por tipo de FII com base no perfil do investidor (Conservador, Moderado ou Agressivo).

## Objetivos do Projeto

- Aplicar fórmulas financeiras e de busca avançada no Excel.
- Criar um painel intuitivo para simulação de investimentos e rentabilidade.
- Automatizar o cálculo da distribuição da carteira conforme o perfil do investidor.
- Exercitar o uso de intervalos nomeados e chaves compostas para tornar as fórmulas mais dinâmicas e organizadas.

## ⚙️ Funcionalidades Principais
| Funcionalidade                                  | Descrição                                                                                     |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------- |
| 💸 **Simulação de Patrimônio**                  | Cálculo automático do valor acumulado com base no tempo e taxa de rendimento.                 |
| 📈 **Cenários de Longo Prazo**                  | Projeção de resultados em 2, 5, 10, 20 e 30 anos.                                             |
| 🏦 **Distribuição de Carteira por Tipo de FII** | Percentuais ajustados automaticamente conforme o perfil (Conservador, Moderado ou Agressivo). |
| 🔍 **Busca Dinâmica (PROCV)**                   | Retorna automaticamente os percentuais sugeridos por tipo de ativo.                           |
| 🧩 **Uso de Chave Composta**                    | Combina “Perfil + Tipo de FII” para garantir precisão nas buscas do PROCV.                    |
| 🧠 **Intervalos Nomeados**                      | Facilita a leitura das fórmulas e permite criar referências nominais dentro dos cálculos.     |


## 🧮 Principais Fórmulas Utilizadas
| Função                                          | Aplicação                                                                      |
| ----------------------------------------------- | ------------------------------------------------------------------------------ |
| `=VF(taxa; períodos; -pagamento; 0)`            | Cálculo do patrimônio acumulado ao longo do tempo.                             |
| `=PROCV(chave; tabela; coluna; FALSO)`          | Retorna o percentual ideal de investimento para o perfil selecionado.          |
| **Intervalos Nomeados**                         | Criados para facilitar o uso das variáveis e tornar as fórmulas mais legíveis. |
| **Concatenação de Chaves** (`=perfil&"-"&tipo`) | Gera uma chave composta para combinação de dados entre tabelas.                |

## 🧾 Estrutura da Planilha
| Aba          | Descrição                                                                              |
| ------------ | -------------------------------------------------------------------------------------- |
| **APP**      | Simulador principal com área de entrada de dados, cálculo de patrimônio e gráficos.    |
| **BASE_FII** | Tabela de referência com percentuais sugeridos por tipo de FII e perfil de investidor. |

## 🧠 Lógica de Funcionamento

O usuário informa salário, percentual investido e perfil.
A função PROCV busca os percentuais correspondentes na aba BASE_FII usando a chave composta.
Os valores são distribuídos automaticamente entre os tipos de FII.
A função VF calcula o patrimônio acumulado em diferentes horizontes de tempo.
Os resultados são apresentados visualmente no painel principal.

## 📚 Aprendizados e Aplicações

Aplicação prática de funções financeiras e de busca (VF, PROCV);
Criação de dashboards financeiros;
Uso de intervalos nomeados e chaves compostas;
Boas práticas de organização e visualização no Excel.

## 📸 Capturas de Tela

![Base de Perfis](images/1.jpg)
### Imagem 1 - Tela Principal do DIO Invest
Representa a aba APP, onde o usuário insere informações como salário, rendimento da carteira e valor a investir mensalmente. Exibe também projeções de patrimônio acumulado e dividendos mensais com base nas fórmulas aplicadas.

![Base de Perfis](images/2.jpg)
### Imagem 2 - Distribuição de Investimentos por Tipo de FII
Mostra a simulação do perfil de investidor agressivo, com a distribuição percentual e os valores destinados a cada tipo de FII (Papel, Tijolo, Híbridos, FOFs, Desenvolvimento e Hotelarias), acompanhados de um gráfico de pizza ilustrativo.

![Base de Perfis](images/3.jpg)
### Imagem 3 - Tabela de Perfis e Percentuais Sugeridos
Demonstra a aba de referência de perfis, onde é utilizada uma chave composta (Perfil + Tipo de FII) para definir o percentual sugerido. Essa estrutura é usada em conjunto com a função PROCV e intervalos nomeados para alimentar a aba principal.*

## 👩‍💻 Autora

Hevelyn Alves
📍 Projeto desenvolvido no curso Excel com Inteligência Artificial — DIO
📅 2025
🔗 LinkedIn
https://www.linkedin.com/in/hevelyn-alves/

```markdown


