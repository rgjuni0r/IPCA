# IPCA
Este repositório apresenta uma integração do VBA com os dados do IPCA (Índice Nacional de Preços ao Consumidor Amplo) disponíveis através da API do IPEA. O IPCA é amplamente reconhecido como o principal indicador da inflação no Brasil.

# Descrição do Código
Este código fornece funcionalidades que permitem:

1. Calcular a variação percentual do IPCA com base em dois valores (um valor atual e um valor anterior).
2. Converter datas do formato padrão YYYY-MM-DD para o formato brasileiro DD/MM/YYYY.
3. Calcular um índice de correção com base na variação do IPCA.
4. Calcular uma correção acumulada usando uma série de valores do IPCA para um período específico.
5. Consultar o IPCA de um período específico diretamente da API do IPEA.
   
# Detalhamento das Funções e Sub-rotinas:
1. CalculateIPCA
• Objetivo: Calcular a variação percentual entre o valor atual e o valor anterior.
• Parâmetros:
- currentValue: Representa o valor mais recente do IPCA.
- previousValue: Representa o valor anterior do IPCA.

• Retorno: A função retorna a variação percentual calculada com base nos dois valores fornecidos.
  
2. ConvertDateFormat
• Objetivo: Converter datas do formato internacional YYYY-MM-DD para o formato brasileiro DD/MM/YYYY.
• Parâmetros:
- dataStr: Representa uma string contendo a data no formato YYYY-MM-DD.
• Retorno: A função retorna a data convertida no formato DD/MM/YYYY.
  
3. CalculateCorrectionIndex
• Objetivo: Derivar um índice de correção com base na variação do IPCA.
• Parâmetros:
- IPCA: Variação percentual do IPCA.
• Retorno: Retorna um índice de correção calculado com base na variação fornecida.

4. CalculateAccumulatedCorrection
• Objetivo: Determinar a correção acumulada usando uma série de valores mensais do IPCA.
• Parâmetros:
- dataValues: Array contendo as datas dos registros do IPCA.
- IPCAValues: Array contendo os valores mensais do IPCA correspondentes às datas.
• Retorno: Retorna um valor que representa a correção acumulada durante o período das datas fornecidas.

5. LerIpeadataComAPI
• Objetivo: Consultar os valores do IPCA de um período específico usando a API do IPEA.
• Nota: Esta função foi projetada para se comunicar diretamente com a API do IPEA e extrair os dados do IPCA para um período específico. A data inicial e final estão fixas no código, mas podem ser facilmente adaptadas para aceitar parâmetros.

# Conclusão
Este código oferece uma solução robusta e eficiente para os profissionais que desejam integrar dados do IPCA em seus projetos VBA, permitindo análises financeiras e econômicas mais precisas. A integração direta com a API do IPEA garante que os dados sejam atualizados e precisos.

# Contribuições
Sinta-se à vontade para contribuir com este projeto, fazendo fork e enviando pull requests, ou abrindo uma issue para discutir possíveis melhorias ou correções no código.

Obrigado por visitar este repositório! Seu feedback é sempre bem-vindo.

# Sobre o Autor
- Desenvolvido por Rogério Moreira Alves Júnior.

- Possui expertise avançada em linguagens de programação, destacando-se em C, C++, Python e Java, e demonstra aptidão em análises numéricas com Octave e MatLab. No domínio do desenvolvimento web, tem proficiência em JavaScript, HTML e CSS. Em relação às ferramentas, apresenta domínio em Excel Avançado e VBA, evidenciando suas capacidades analíticas e de automação. Sua familiaridade com Arduino atesta competência em automação eletrônica, e sua destreza em AutoCAD e SOLIDWORKS sublinha habilidades em modelagem e design técnico na engenharia.

- Estudou Engenharia Mecânica na Universidade Federal de Santa Maria, Rio Grande do Sul, de 2019 a 2022 e atualmente é graduando em Engenharia Elétrica pela Universidade de Goiás, Goiânia, desde 2022. Destaca-se por sua experiência nas áreas de Engenharia Mecânica e Engenharia Elétrica, particularmente no desenvolvimento de programas computacionais e na elaboração de sistemas de automação com Arduino. Integrou o grupo de pesquisa Núcleo de Inovação e Competitividade (NIC) de 2021 a 2022, voltado para pesquisas em soluções de gestão empresarial, e participou de projetos focados no desenvolvimento de conteúdo técnico-gerencial através de modelos matemáticos para mensuração da competitividade da geração distribuída no Brasil. Além disso, colaborou no Projeto BAJA SAE pela UFSM, contribuindo para a construção e teste de um protótipo de veículo off-road em competições da SAE Brasil. Em 2023, fez parte da Equipe RoboCup Humanoid League no Núcleo de Robótica Pequi Mecânico da UFG, trabalhando no desenvolvimento de robôs humanoides autônomos e, sob sua atuação, a equipe conquistou o 1° e 2° lugares em duas categorias na Latin American Competition Of Robotics (LARC). Como desenvolvedor, assinou projetos relacionados à Engenharia Elétrica, como eficientização de iluminação e cálculo de fatura de energia para o Grupo B. Sua contribuição acadêmica se reflete em publicações em eventos como ICPR, SEPOC, CBENS e JAI-UFSM.
