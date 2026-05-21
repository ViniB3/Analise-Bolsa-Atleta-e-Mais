# 🏅 Data Science: Bolsa Atleta & O Cenário de Infraestrutura Esportiva e Educacional no Brasil

## ❓ Perguntas de Pesquisa
Para guiar a análise exploratória e a construção dos modelos preditivos, o projeto responde formalmente às seguintes questões:

Pergunta 1: Qual é o peso estatístico da infraestrutura esportiva das escolas locais (ex: presença de quadras cobertas e piscinas) na quantidade de beneficiários do Bolsa Atleta nas categorias Estudantil e de Base em um município, quando controlado pelo tamanho da população e IDH?

Pergunta 2: Em termos de distribuição espacial, existem agrupamentos geográficos (clusters) de "desertos de fomento esportivo" — isto é, regiões com alto volume de jovens em idade escolar, mas com severa escassez cumulativa de infraestrutura e de concessão de bolsas?

## 💡 Hipóteses TestáveisPara responder às perguntas acima utilizando testes estatísticos e algoritmos de Machine Learning, estabelecemos as seguintes hipóteses:
  Hipótese 1 ($H_1$ - Correlação Estrutural): Municípios que possuem um percentual de escolas públicas com quadras esportivas cobertas superior a 60% apresentam uma taxa de atletas contemplados na categoria Bolsa Estudantil (por 100 mil habitantes) significativamente maior do que municípios com infraestrutura inferior, independente do IDH local.
  
  Hipótese 2 ($H_2$ - O Gargalo da Elite): A presença de equipamentos esportivos especializados no Censo Escolar (como piscinas e pistas de atletismo) possui maior poder preditivo na transição de atletas para as categorias de elite (Nacional, Internacional e Pódio) do que variáveis puramente financeiras, como o PIB per capita do município.
  
  Hipótese 3 ($H_3$ - Assimetria Público-Privada): A dependência de infraestrutura da rede privada de ensino para a geração de atletas de base é significativamente maior nas regiões Norte e Nordeste do que nas regiões Sul e Sudeste, onde a rede pública absorve essa demanda.

## 🛠 2. Tecnologias, Bibliotecas e Fontes de Dados
### Fontes de Dados Utilizadas
Dados Abertos do Ministério do Esporte: Microdados dos contemplados pelo Programa Bolsa Atleta (2020-2026).

INEP / Censo Escolar: Infraestrutura das escolas de educação básica (presença de quadras esportivas, piscinas, etc.).

IBGE: Dados socioeconômicos dos municípios (PIB per capita, população e IDH).

# Descrição do Dataset: Bolsa Atleta Dezembro

## Fonte
O dataset "Bolsa Atleta Dezembro (Planilha1)" foi obtido a partir de dados públicos relacionados ao programa Bolsa Atleta, que visa apoiar financeiramente atletas brasileiros. A fonte original dos dados é https://dados.gov.br/dados/conjuntos-dados/folha-de-pagamento---bolsa-atleta-

## Estrutura
O arquivo está no formato CSV, com o seguinte nome:
- Bolsa Atleta Dezembro(Planilha1).csv

Principais colunas:
- **UF**: Unidade Federativa (estado brasileiro) do atleta.
- **Valor Pago**: Valor financeiro pago ao atleta, em reais.
- Modalidade: Esporte praticado pelo atleta
- Categoria: Categoria em que o atleta compete
- Outras colunas podem estar presentes, detalhando informações adicionais dos beneficiários.


## Tamanho Estimado
- O arquivo possui 9413 linhas, cada uma representando um atleta beneficiado no mês de dezembro.
- O tamanho do arquivo é 1,3 MB.

## Observações
- Os dados permitem análises por estado (UF), total de valores pagos e número de atletas beneficiados.




Desenvolvido por: [Vinícius R. Borges]

Contato: [vinicius.240598@alunos.utfpr.edu.br]

LinkedIn: linkedin.com/in/ViniB3
