# `<Estudo de Caso: Síntese de Sinais de EEG para Imagética Motora>`
# `<Signal synthesis for eeg motor imagery>`

## Apresentação

O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação *IA376L - Deep Learning aplicado a Síntese de Sinais*, 
oferecida no segundo semestre de 2023, na Unicamp, sob supervisão da Profa. Dra. Paula Dornhofer Paro Costa, do Departamento de Engenharia de Computação e Automação (DCA) da Faculdade de Engenharia Elétrica e de Computação (FEEC).

> |Nome  | RA | Especialização|
> |--|--|--|
> | Joany Rodrigues  | 264440  | Eng. de Computação|
> | João Guilherme Prado Barbon  | 262760  | Eng. Físico|
> | Larissa Rangel de Azevedo  | 247008  | Eng. Eletricista|

## Descrição Resumida do Projeto
  Este projeto tem como objetivo sintetizar dados de eletroencefalografia (EEG) para uma interface cérebro-computador (BCI) utilizando o paradigma de imagética motora. A principal motivação da implementação de uma BCI é o estudo e a compreensão do cérebro, abrindo portas para aplicações na área da saúde e entretenimento. A abordagem do paradigma da imagética motora ocorre pela aquisição dos sinais cerebrais gerados pela imaginação ou realização do movimento de partes do corpo, como membros superiores (braços) ou inferiores (pernas). Assim, os dados sintéticos serão gerados a partir de uma Rede Generativa Adversária (GAN), que apresentará como saída séries temporais representativas dos sinais reais de EEG.  

> Incluir nessa seção link para vídeo de apresentação da proposta do projeto (máximo 5 minutos).

## Metodologia Proposta
- A base de dados que será utilizada é a [BNCI2014_001](https://moabb.neurotechx.com/docs/generated/moabb.datasets.BNCI2014_001.html#r55ebd47d0fe7-1), que consiste em dados de EEG de nove indivíduos, com quatro classes de movimento diferentes: movimento da mão esquerda (classe 1), da mão direita (classe 2), de ambos os pés (classe 3) e da lingua (classe 4). Este dataset foi utilizado no Review BCI Competition 4, sendo portanto bem documentado e testado.
- Como principal modelo generativo, serão utilizadas GANs para geração dos dados sintéticos. Como primeira abordagem, propomos uma DCGAN conforme o artigo [EEG-GAN](https://arxiv.org/abs/1806.01875).
- Outro artigo de referência que será utilizado - [Augmenting EEG with Generative Adversarial Networks Enhances Brain Decoding Across Classifiers and Sample Sizes](https://escholarship.org/uc/item/9gz8g908), em que os autores avaliam o impacto do aumento de dados sintéticos de EEG na avaliação dos classificadores.
-  As ferramentas utilizadas serão:
  - Linguagem:  Python,
  - Biblioteca: Pythorch
  - Ambiente: Google Colab e Kaggle
  
- Os resultados esperados serão distribuições de dados sintéticos de EEG que melhor se aproximam das distribuições reais. Para verificar se as distribuições são compatíveis, iremos mapear os dados para um manifold de menor dimensão utilizando técnicas como autoencoders, PCA ou tSNE. Como métrica de avaliação, serão utilizadas técnicas como distância Euclidiana, as divergências de Kullback-leibler e Jensen–Shannon e por fim uma análise comparativa de classificadores alimentados com dados sintéticos e dados reais.

## Cronograma
> Proposta de cronograma. Procure estimar quantas semanas serão gastas para cada etapa do projeto.

## Referências Bibliográficas
> Apontar nesta seção as referências bibliográficas adotadas no projeto.


-----------------------------------------------------------------------------------------------------------------

# Repositório para o projeto de  IA376 - Deep Learning aplicado em sinais de EEG

# Tutorial - Como usar git/github

- Tutorial com códigos -> (https://githowto.com/)
- Tutorial no YouTube -> (https://youtu.be/3RjQznt-8kE?si=awzuTqYfzZdM7xHZ)
- Tutorial prático de como usar git -> (https://learngitbranching.js.org/)
- Um jogo que ensina git -> (https://ohmygit.org/)

# Referênciais

- Tese Sarah Negreiros de Carvalho Leite - Contribuições ao desenvolvimento de interfaces cérebro-computador baseadas em potenciais evocados visualmente em regime estacionário

Tese: (https://doi.org/10.47749/T/UNICAMP.2016.970748)

- Augmenting EEG with Generative Adversarial Networks Enhances Brain Decoding Across Classifiers and Sample Sizes

Paper: (https://escholarship.org/uc/item/9gz8g908)
Git: (https://github.com/AutoResearch/EEG-GAN)

- EEG data augmentation for emotion recognition with a multiple generator conditional Wasserstein GAN

Paper: (https://link.springer.com/article/10.1007/s40747-021-00336-7)


- EEG-GAN: Generative adversarial networks for electroencephalograhic (EEG) brain signals

Paper: (https://arxiv.org/abs/1806.01875)
Git: (https://github.com/aung2phyowai/GAN)

