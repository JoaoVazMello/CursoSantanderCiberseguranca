# 🤖 Introdução à Inteligência Artificial

> **Curso:** Cibersegurança — Santander + DIO  
> **Conteúdo:** Fundamentos de Inteligência Artificial  
> **Objetivo:** Registrar os conhecimentos adquiridos durante o curso, desde o surgimento da Inteligência Artificial até conceitos como Machine Learning, Deep Learning, LLMs e Transformers.

---

## 📌 1. O "início" da Inteligência Artificial — Alan Turing

Uma das primeiras grandes discussões sobre a possibilidade de máquinas apresentarem comportamentos inteligentes surgiu com **Alan Turing**, considerado um dos pais da Ciência da Computação. Em 1950, Turing publicou o artigo *Computing Machinery and Intelligence*, no qual apresentou uma questão muito importante: **"As máquinas podem pensar?"** Para explorar essa pergunta, ele propôs um experimento conhecido como **Teste de Turing**, também chamado de *Jogo da Imitação*.

### Como funcionaria o Teste de Turing?

A ideia consistia em colocar um avaliador humano para conversar, por meio de mensagens, com dois participantes:

- Um ser humano.
- Uma máquina.

O avaliador não saberia qual participante era a máquina e qual era o humano. O objetivo seria verificar se a máquina conseguiria manter uma conversa convincente o suficiente para dificultar sua identificação.

**O ponto principal:** Turing propôs uma maneira de avaliar o comportamento inteligente de uma máquina, em vez de tentar definir diretamente o que significa pensar. Isso não significa que ele tenha comprovado que máquinas pensam ou possuem consciência. O teste era uma proposta teórica que se tornou uma das principais referências para o desenvolvimento da Inteligência Artificial.

---

## 💬 2. ELIZA — Um dos primeiros chatbots da história

Anos depois, entre 1964 e 1966, o cientista da computação **Joseph Weizenbaum**, pesquisador do MIT, desenvolveu o programa ELIZA. ELIZA foi um dos primeiros programas capazes de simular uma conversa utilizando linguagem natural. Uma de suas implementações mais conhecidas simulava o comportamento de um psicoterapeuta, respondendo às mensagens dos usuários principalmente por meio de perguntas.

### Como ELIZA funcionava?

Diferentemente dos modelos modernos de Inteligência Artificial, ELIZA não utilizava grandes redes neurais ou aprendizado profundo. Seu funcionamento era relativamente simples:

1. O usuário digitava uma mensagem.
2. O programa procurava palavras-chave e padrões no texto.
3. Quando encontrava um padrão conhecido, aplicava uma regra previamente programada.
4. Uma resposta era construída, muitas vezes transformando a própria mensagem do usuário em uma pergunta.

**Exemplo ilustrativo:**

**Usuário:** "Estou preocupado com meu trabalho."

**ELIZA:** "Por que você está preocupado com seu trabalho?"

Embora parecesse estar compreendendo a situação, o programa apenas identificava padrões e aplicava regras de transformação de texto.

### O efeito ELIZA

Durante as interações com o programa, observou-se que algumas pessoas atribuíam compreensão, empatia e até sentimentos à máquina. Esse comportamento ficou conhecido como **Efeito ELIZA**. O fenômeno mostra nossa tendência de atribuir características humanas a sistemas computacionais, mesmo quando suas respostas são produzidas por mecanismos relativamente simples. Essa descoberta também levantou questões importantes sobre a relação entre seres humanos e máquinas.

---

## 🧠 3. Machine Learning — Aprendizado de Máquina

Dentro da Inteligência Artificial existem diferentes áreas, sendo uma das principais o **Machine Learning (Aprendizado de Máquina)**. Seu objetivo é permitir que sistemas computacionais aprendam padrões a partir de dados, em vez de depender exclusivamente de regras programadas manualmente. De maneira simplificada, um modelo recebe dados durante o treinamento e ajusta seus parâmetros matemáticos para conseguir realizar determinadas tarefas.

### Exemplo prático

Imagine que queremos desenvolver um sistema capaz de identificar mensagens de spam. Podemos fornecer milhares de exemplos de mensagens, incluindo:

- Mensagens legítimas.
- Mensagens classificadas como spam.

Durante o treinamento, o modelo aprende padrões que ajudam a diferenciar esses dois grupos. Posteriormente, ao receber uma mensagem que nunca viu, ele pode estimar a probabilidade de ela ser spam. Esse mesmo Machine Learning no entanto não se limita somente à classificação. Também pode ser utilizado para prever valores, descobrir agrupamentos, identificar anomalias e aprender estratégias de decisão.

---

## 🔬 4. Deep Learning — Aprendizado Profundo

O **Deep Learning (Aprendizado Profundo)** é uma subárea do Machine Learning que utiliza redes neurais artificiais compostas por várias camadas. Essas redes são inspiradas, de maneira bastante simplificada, na organização de neurônios biológicos. A principal diferença em relação a muitos métodos tradicionais de Machine Learning está na capacidade de aprender representações cada vez mais complexas dos dados.

### Como funciona?

Imagine que estamos treinando uma rede neural para reconhecer imagens de gatos.

Nas primeiras camadas, a rede pode aprender a identificar características mais simples, como:

- Bordas e linhas.
- Contrastes e texturas.
- Formas e padrões visuais.

Em camadas posteriores, essas informações podem ser combinadas para identificar características mais complexas, como orelhas, olhos e outras estruturas associadas ao animal. Ao final, o modelo utiliza essas informações para realizar uma previsão. O diferencial do Deep Learning é que grande parte dessas características pode ser aprendida automaticamente durante o treinamento. Além de reconhecer imagens, modelos de aprendizado profundo podem realizar tarefas como tradução, reconhecimento de voz, geração de textos e identificação de atividades suspeitas.

---

## 📚 5. LLMs — Grandes Modelos de Linguagem

Com os avanços das redes neurais e do poder computacional, surgiram modelos de linguagem cada vez maiores e mais sofisticados.Os **Large Language Models (LLMs)** são modelos treinados com grandes quantidades de dados, principalmente textos e códigos, para aprender padrões e relações presentes na linguagem.

Esses modelos conseguem realizar tarefas como:

- Responder perguntas e manter conversas.
- Resumir e traduzir textos.
- Gerar e explicar códigos.
- Produzir diferentes tipos de conteúdo.

### O que são tokens?

Os LLMs não processam textos exatamente da mesma maneira que os seres humanos. Antes do processamento, o texto passa por uma etapa chamada **tokenização**, na qual é dividido em unidades menores chamadas *tokens*. Um token pode representar uma palavra inteira, parte de uma palavra ou até um símbolo. Esses tokens são convertidos em representações numéricas para serem processados pelo modelo.

### Como um LLM aprende?

Uma das principais estratégias de treinamento dos LLMs generativos consiste em aprender a prever o próximo token de uma sequência. Por exemplo: "A capital do Brasil é" O modelo analisa os padrões aprendidos durante o treinamento e calcula probabilidades para os possíveis próximos tokens. Nesse contexto, a continuação "Brasília" teria uma probabilidade elevada. Esse processo é repetido sucessivamente durante a geração de uma resposta.

Entretanto, os LLMs não funcionam apenas memorizando frases. Durante o treinamento, suas redes neurais aprendem representações estatísticas complexas das relações entre palavras, conceitos e contextos. Porém gerar respostas convincentes não garante que todas as informações produzidas sejam verdadeiras. Modelos de linguagem também podem cometer erros e produzir informações incorretas.

---

## ⚙️ 6. Transformers — A arquitetura por trás de muitos LLMs

Um dos avanços mais importantes para os modelos modernos de Inteligência Artificial foi o surgimento da arquitetura **Transformer**, apresentada em 2017 no artigo *Attention Is All You Need*. Essa arquitetura utiliza mecanismos de atenção para identificar relações entre diferentes partes de uma sequência de informações. Os Transformers são modelos de Deep Learning e se tornaram a base de grande parte dos LLMs modernos.

### O que é o mecanismo de atenção?

O mecanismo de atenção permite que o modelo atribua diferentes níveis de importância às informações de uma sequência durante seu processamento. Considere estas duas frases:

**Frase 1:** "Fui ao banco retirar dinheiro."

**Frase 2:** "Sentei no banco da praça."

Embora a palavra "banco" apareça nas duas frases, seu significado muda dependendo do contexto. O mecanismo de **Self-Attention (Autoatenção)** permite que o modelo relacione uma palavra aos outros elementos da sequência.Na primeira frase, a relação com "retirar dinheiro" ajuda a identificar uma instituição financeira. Na segunda, a relação com "sentei" e "praça" indica um assento. Dessa maneira, a representação de cada palavra pode considerar o contexto em que ela aparece.

### Como o Transformer funciona?

De forma simplificada, o processamento pode ser entendido nas seguintes etapas:

1. **Tokenização:** o texto é dividido em tokens.
2. **Representação numérica:** os tokens são convertidos em vetores numéricos, chamados *embeddings*.
3. **Informação posicional:** o modelo recebe informações sobre a posição dos tokens na sequência.
4. **Self-Attention:** são calculadas relações de importância entre os tokens.
5. **Camadas da rede neural:** as informações são processadas e transformadas para construir representações mais complexas.
6. **Produção da saída:** o modelo utiliza as representações resultantes para realizar sua tarefa, como gerar uma resposta.

### Por que os Transformers foram tão importantes?

Antes dessa arquitetura, muitos sistemas de processamento de linguagem utilizavam redes recorrentes, que processavam sequências de forma mais dependente de etapas anteriores. Os Transformers trouxeram vantagens importantes:

- Permitem maior paralelização durante o treinamento.
- Conseguem relacionar informações em diferentes posições de um texto.
- Apresentam boa capacidade de escalabilidade com grandes volumes de dados e recursos computacionais.
- Podem ser utilizados em tarefas envolvendo textos, imagens, áudio e outros tipos de dados.

**Atenção:** embora o treinamento possa aproveitar bastante processamento paralelo, a geração de texto nos LLMs autorregressivos normalmente continua acontecendo token por token. A arquitetura Transformer foi fundamental para o desenvolvimento de muitos dos sistemas modernos de Inteligência Artificial generativa.

---

## 🔐 7. Qual é a relação da IA com a Cibersegurança?

A Inteligência Artificial também possui diversas aplicações na área de Cibersegurança. Algumas possibilidades incluem:

- **Detecção de phishing:** análise de mensagens e e-mails para identificar características de tentativas de fraude.
- **Identificação de malware:** reconhecimento de padrões associados a softwares maliciosos.
- **Análise de logs:** identificação de eventos suspeitos em registros de sistemas e redes.
- **Detecção de anomalias:** reconhecimento de comportamentos que fogem do padrão esperado.
- **Apoio à análise de incidentes:** organização e interpretação de grandes quantidades de informações relacionadas a possíveis ataques.

Entretanto, os modelos também podem produzir falsos positivos, deixar passar ameaças e apresentar respostas incorretas. Por isso, a IA deve ser utilizada como ferramenta de apoio, e não como substituta completa da análise humana. Além disso, as mesmas tecnologias também podem ser utilizadas por agentes maliciosos, tornando importante conhecer tanto seus benefícios quanto seus riscos.

---

## 📝 8. Resumo dos conceitos

| Conceito | Descrição |
|---|---|
| Inteligência Artificial (IA) | Área da computação voltada ao desenvolvimento de sistemas capazes de realizar tarefas associadas à inteligência. |
| Teste de Turing | Proposta para avaliar se uma máquina consegue apresentar comportamento conversacional semelhante ao humano. |
| ELIZA | Um dos primeiros chatbots, baseado principalmente em regras e reconhecimento de padrões. |
| Machine Learning | Área da IA que desenvolve modelos capazes de aprender padrões a partir de dados. |
| Deep Learning | Subárea do Machine Learning que utiliza redes neurais artificiais com múltiplas camadas. |
| LLM | Grande modelo de linguagem treinado para processar e produzir linguagem natural. |
| Transformer | Arquitetura de Deep Learning baseada em mecanismos de atenção, utilizada em muitos LLMs modernos. |

### Relação entre as tecnologias

É importante entender que essas áreas não são completamente separadas:

**Inteligência Artificial → Machine Learning → Deep Learning → Transformers → Muitos dos LLMs modernos**

Ou seja, os Transformers são uma arquitetura utilizada dentro do Deep Learning, enquanto os LLMs são modelos de linguagem que frequentemente utilizam essa arquitetura.

---

## 📖 Referências para estudo

- [Alan Turing — Computing Machinery and Intelligence (1950)](https://doi.org/10.1093/mind/LIX.236.433)
- [Joseph Weizenbaum — ELIZA (1966)](https://doi.org/10.1145/365153.365168)
- [IBM — IA, Machine Learning e Deep Learning](https://www.ibm.com/br-pt/think/topics/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks)
- [IBM — Large Language Models](https://www.ibm.com/think/topics/large-language-models)
- [Google Research — Attention Is All You Need (2017)](https://research.google/pubs/attention-is-all-you-need/)

---

> **Observação:** estas anotações fazem parte do meu processo de aprendizado no curso de Cibersegurança do Santander em parceria com a DIO. O objetivo é registrar os principais conceitos apresentados e complementar o conteúdo com exemplos e explicações para facilitar revisões futuras.