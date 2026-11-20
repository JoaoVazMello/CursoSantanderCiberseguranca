# 🤖 Introdução à Inteligência Artificial

> **Curso:** Cibersegurança — Santander + DIO  
> **Conteúdo:** Fundamentos de Inteligência Artificial  
> **Objetivo:** Registrar os conhecimentos adquiridos durante o curso, desde o surgimento da Inteligência Artificial até conceitos como Machine Learning, Deep Learning, LLMs e Transformers.

---

## 📌 1. O início da Inteligência Artificial — Alan Turing

Uma das primeiras grandes discussões sobre a possibilidade de máquinas apresentarem comportamentos inteligentes surgiu com **Alan Turing**, considerado um dos pais da Ciência da Computação. Em 1950, Turing publicou o artigo *Computing Machinery and Intelligence*, no qual apresentou uma questão muito importante: **"As máquinas podem pensar?"** Para explorar essa pergunta, ele propôs um experimento conhecido como **Teste de Turing**, também chamado de *Jogo da Imitação*.

### Como funcionaria o Teste de Turing?

A ideia consistia em colocar um avaliador humano para conversar, por meio de mensagens, com dois participantes:

- Um ser humano.
- Uma máquina.

O avaliador não saberia qual participante era a máquina e qual era o humano. O objetivo seria verificar se a máquina conseguiria manter uma conversa convincente o suficiente para dificultar sua identificação. **O ponto principal:** Turing propôs uma maneira de avaliar o comportamento inteligente de uma máquina, em vez de tentar definir diretamente o que significa pensar.Isso não significa que ele tenha comprovado que máquinas pensam ou possuem consciência. O teste era uma proposta teórica que se tornou uma das principais referências para o desenvolvimento da Inteligência Artificial.

---

## 💬 2. ELIZA — Um dos primeiros chatbots da história

Anos depois, entre 1964 e 1966, o cientista da computação **Joseph Weizenbaum**, pesquisador do MIT, desenvolveu o programa ELIZA. Ela foi um dos primeiros programas capazes de simular uma conversa utilizando linguagem natural. Uma de suas implementações mais conhecidas simulava o comportamento de um psicoterapeuta, respondendo às mensagens dos usuários principalmente por meio de perguntas.

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

Imagine que queremos desenvolver um sistema capaz de identificar mensagens de spam.

Podemos fornecer milhares de exemplos de mensagens, incluindo:

- Mensagens legítimas.
- Mensagens classificadas como spam.

Durante o treinamento, o modelo aprende padrões que ajudam a diferenciar esses dois grupos. Posteriormente, ao receber uma mensagem que nunca viu, ele pode estimar a probabilidade de ela ser spam. **Importante:** Machine Learning não se limita à classificação. Também pode ser utilizado para prever valores, descobrir agrupamentos, identificar anomalias e aprender estratégias de decisão.

---

## 🔬 4. Deep Learning — Aprendizado Profundo

O **Deep Learning (Aprendizado Profundo)** é uma subárea do Machine Learning que utiliza redes neurais artificiais compostas por várias camadas. Essas redes são inspiradas, de maneira bastante simplificada, na organização de neurônios biológicos.A principal diferença em relação a muitos métodos tradicionais de Machine Learning está na capacidade de aprender representações cada vez mais complexas dos dados.

### Como funciona?

Imagine que estamos treinando uma rede neural para reconhecer imagens de gatos. Nas primeiras camadas, a rede pode aprender a identificar características mais simples, como:

- Bordas e linhas.
- Contrastes e texturas.
- Formas e padrões visuais.

Em camadas posteriores, essas informações podem ser combinadas para identificar características mais complexas, como orelhas, olhos e outras estruturas associadas ao animal. Ao final, o modelo utiliza essas informações para realizar uma previsão. O diferencial do Deep Learning é que grande parte dessas características pode ser aprendida automaticamente durante o treinamento. Além de reconhecer imagens, modelos de aprendizado profundo podem realizar tarefas como tradução, reconhecimento de voz, geração de textos e identificação de atividades suspeitas.

---

## 📚 5. LLMs — Grandes Modelos de Linguagem

Com os avanços das redes neurais e do poder computacional, surgiram modelos de linguagem cada vez maiores e mais sofisticados. Os **Large Language Models (LLMs)** são modelos treinados com grandes quantidades de dados, principalmente textos e códigos, para aprender padrões e relações presentes na linguagem.

Esses modelos conseguem realizar tarefas como:

- Responder perguntas e manter conversas.
- Resumir e traduzir textos.
- Gerar e explicar códigos.
- Produzir diferentes tipos de conteúdo.

### O que são tokens?

Os LLMs não processam textos exatamente da mesma maneira que os seres humanos. Antes do processamento, o texto passa por uma etapa chamada **tokenização**, na qual é dividido em unidades menores chamadas *tokens*. Um token pode representar uma palavra inteira, parte de uma palavra ou até um símbolo. Esses tokens são convertidos em representações numéricas para serem processados pelo modelo.

### Como um LLM aprende?

Uma das principais estratégias de treinamento dos LLMs generativos consiste em aprender a prever o próximo token de uma sequência. Por exemplo: **Entrada:** "A capital do Brasil é". O modelo analisa os padrões aprendidos durante o treinamento e calcula probabilidades para os possíveis próximos tokens. Nesse contexto, a continuação "Brasília" teria uma probabilidade elevada. Esse processo é repetido sucessivamente durante a geração de uma resposta. Entretanto, os LLMs não funcionam apenas memorizando frases. Durante o treinamento, suas redes neurais aprendem representações estatísticas complexas das relações entre palavras, conceitos e contextos.

**Uma observação importante:** gerar respostas convincentes não garante que todas as informações produzidas sejam verdadeiras. Modelos de linguagem também podem cometer erros e produzir informações incorretas.

---

## ⚙️ 6. Transformers — A arquitetura por trás de muitos LLMs

Um dos avanços mais importantes para os modelos modernos de Inteligência Artificial foi o surgimento da arquitetura **Transformer**, apresentada em 2017 no artigo *Attention Is All You Need*. Essa arquitetura utiliza mecanismos de atenção para identificar relações entre diferentes partes de uma sequência de informações. Os Transformers são modelos de Deep Learning e se tornaram a base de grande parte dos LLMs modernos.

### O que é o mecanismo de atenção?

O mecanismo de atenção permite que o modelo atribua diferentes níveis de importância às informações de uma sequência durante seu processamento. Considere estas duas frases:

**Frase 1:** "Fui ao banco retirar dinheiro."

**Frase 2:** "Sentei no banco da praça."

Embora a palavra "banco" apareça nas duas frases, seu significado muda dependendo do contexto. O mecanismo de **Self-Attention (Autoatenção)** permite que o modelo relacione uma palavra aos outros elementos da sequência. Na primeira frase, a relação com "retirar dinheiro" ajuda a identificar uma instituição financeira. Na segunda, a relação com "sentei" e "praça" indica um assento. Dessa maneira, a representação de cada palavra pode considerar o contexto em que ela aparece.

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

## 💬 7. Chatbots — Uso e conceito

Os **chatbots** são sistemas criados para conversar com usuários por texto ou voz. Eles podem responder dúvidas, oferecer orientações e ajudar na realização de atividades. Como vimos anteriormente, **ELIZA** foi um dos primeiros exemplos desse tipo de sistema. Entretanto, nem todo chatbot funciona da mesma maneira: alguns utilizam regras predefinidas, enquanto outros, como o ChatGPT, utilizam **modelos de linguagem (LLMs)**.

### A importância de um bom prompt

Nos chatbots baseados em LLMs, a maneira como fazemos uma pergunta pode influenciar bastante a resposta. Chamamos de **prompt** a instrução ou mensagem enviada ao modelo. Quanto mais claro for o objetivo, o contexto e o formato desejado, mais fácil será orientar a resposta. Durante o curso, uma das práticas foi criar um prompt para organizar os estudos em cibersegurança.

**Exemplo prático:**

```text
Estou cursando Ciência da Computação, concluí seis períodos da graduação
e quero começar a estudar cibersegurança. Tenho três horas por dia disponíveis.

Ajude-me a decidir por onde começar. Responda assim:

1. Conhecimentos necessários para entender a teoria da área.
2. Conceitos que devo estudar e uma ordem sugerida.
3. Plataformas e ambientes nos quais posso praticar.

Use linguagem simples, como em uma conversa com um amigo.
```

Esse exemplo mostra que um prompt bem estruturado não precisa ser complicado. Basta apresentar as informações importantes e explicar o resultado esperado. **Importante:** bons prompts ajudam a direcionar a resposta, mas não garantem que ela esteja completamente correta. Sempre que necessário, é importante verificar as informações.

> **Referência da prática:** [DIO — Potencializando seus estudos e carreira com IA](https://github.com/digitalinnovationone/potencializando-estudos-carreira-com-ia).

---

## 👨‍💻 8. Copilotos — Assistentes durante as atividades

Os **copilotos de IA** são assistentes que trabalham junto com o usuário durante uma atividade, geralmente integrados a programas, editores de código ou ferramentas de produtividade. Imagine que você está programando e uma ferramenta consegue sugerir a continuação de uma função, explicar um erro ou ajudar a revisar seu código. Esse é um exemplo de assistência oferecida por um copiloto. Outros copilotos podem auxiliar na leitura e organização de documentos, planilhas e diferentes informações, conforme os recursos e permissões disponíveis.

### Qual é a diferença entre chatbot e copiloto?

Uma forma simples de entender essa diferença é:

- **Chatbot:** normalmente tem a conversa como principal forma de interação.
- **Copiloto:** costuma acompanhar uma tarefa em andamento e aproveitar o contexto do trabalho para ajudar.

Essa separação não é absoluta. Um chatbot também pode trabalhar com documentos e ferramentas, e um copiloto também pode funcionar por meio de uma conversa.

### Exemplo prático — Criando um plano de estudos

Na segunda atividade, a proposta foi utilizar o **Gemini**, do Google, como assistente para estruturar um plano de estudos de cibersegurança com base no contexto informado.

**Prompt utilizado, com ajustes de escrita:**

```text
Crie um plano de estudos de 30 dias para mim.

Área escolhida: Cibersegurança.
Tópicos iniciais: utilize os tópicos definidos na Prática 01.

Estruture o plano com:
1. Meu objetivo de aprendizagem.
2. Cronograma semanal (semanas 1 a 4), distribuindo os tópicos.
3. Materiais e referências indicados para cada semana.

Considere o arquivo que disponibilizei e, caso existam conexões autorizadas,
utilize também conteúdos relevantes dos meus e-mails ou do meu Drive.
Você também pode sugerir materiais públicos disponíveis na internet.

Não exponha dados pessoais ou sensíveis.
Organize o resultado em um arquivo que eu possa salvar e consultar depois.
```

**Observação:** o acesso ao Gmail, Google Drive ou outros arquivos depende das integrações e permissões concedidas. A geração de arquivos para baixar também depende das funcionalidades disponíveis na ferramenta utilizada.

> **Materiais das atividades:** os arquivos produzidos nas práticas podem ser organizados no diretório `pratica/PraticaIA/` do repositório.

---

## 🤖 9. Agentes de IA — Autonomia e execução de tarefas

Os **agentes de Inteligência Artificial** são sistemas que podem receber um objetivo, organizar etapas e utilizar ferramentas para executar tarefas, dependendo das permissões concedidas. Enquanto um chatbot costuma ser utilizado para conversar e um copiloto acompanha uma atividade, um agente pode **realizar ações** para avançar em um objetivo. Por exemplo, um agente voltado ao desenvolvimento de software pode analisar arquivos de um projeto, propor alterações no código e executar testes em um ambiente autorizado.

### Como funcionam os agentes?

De maneira simplificada, um agente pode seguir estas etapas:

1. **Receber um objetivo:** entender o que o usuário deseja realizar.
2. **Planejar ações:** identificar possíveis passos para resolver a tarefa.
3. **Utilizar ferramentas:** acessar recursos permitidos, como arquivos ou terminal.
4. **Avaliar resultados:** verificar o que aconteceu após cada ação.
5. **Continuar ou finalizar:** ajustar o plano quando necessário e apresentar o resultado.

**Importante:** agentes não são necessariamente um novo tipo de modelo matemático. Muitas vezes, eles combinam um LLM com ferramentas, instruções e mecanismos de controle. Também não significa que possuem autonomia ilimitada.

### Exemplo prático — Google Antigravity

Durante o curso, foi apresentado o **Google Antigravity** como exemplo de ferramenta voltada ao desenvolvimento com agentes de IA.

Uma das possibilidades é utilizar uma interface de linha de comando (CLI) para interagir com ferramentas do ambiente de desenvolvimento.

O seguinte comando foi apresentado para instalação no **Prompt de Comando do Windows (CMD)**:

```bat
curl -fsSL https://antigravity.google/cli/install.cmd -o install.cmd && install.cmd && del install.cmd
```

**Atenção:** esse comando baixa e executa um script. Antes de utilizá-lo, confirme se o endereço e as instruções continuam válidos na [documentação oficial do Google Antigravity](https://antigravity.google/docs/cli-getting-started?hl=pt-br) e revise o conteúdo do instalador. A instalação não foi testada nesta revisão.

Isso também nos lembra de um cuidado importante na cibersegurança: **quanto mais permissões oferecemos a um agente, mais atenção precisamos ter com as ações que ele pode executar**.

---

## 🔐 10. Qual é a relação da IA com a Cibersegurança?

A Inteligência Artificial também possui diversas aplicações na área de Cibersegurança.

Algumas possibilidades incluem:

- **Detecção de phishing:** análise de mensagens e e-mails para identificar características de tentativas de fraude.
- **Identificação de malware:** reconhecimento de padrões associados a softwares maliciosos.
- **Análise de logs:** identificação de eventos suspeitos em registros de sistemas e redes.
- **Detecção de anomalias:** reconhecimento de comportamentos que fogem do padrão esperado.
- **Apoio à análise de incidentes:** organização e interpretação de grandes quantidades de informações relacionadas a possíveis ataques.

Entretanto, os modelos também podem produzir falsos positivos, deixar passar ameaças e apresentar respostas incorretas.

Por isso, a IA deve ser utilizada como ferramenta de apoio, e não como substituta completa da análise humana.

Além disso, as mesmas tecnologias também podem ser utilizadas por agentes maliciosos, tornando importante conhecer tanto seus benefícios quanto seus riscos.

---

## 📝 11. Resumo dos conceitos

| Conceito | Descrição |
|---|---|
| Inteligência Artificial (IA) | Área da computação voltada ao desenvolvimento de sistemas capazes de realizar tarefas associadas à inteligência. |
| Teste de Turing | Proposta para avaliar se uma máquina consegue apresentar comportamento conversacional semelhante ao humano. |
| ELIZA | Um dos primeiros chatbots, baseado principalmente em regras e reconhecimento de padrões. |
| Machine Learning | Área da IA que desenvolve modelos capazes de aprender padrões a partir de dados. |
| Deep Learning | Subárea do Machine Learning que utiliza redes neurais artificiais com múltiplas camadas. |
| LLM | Grande modelo de linguagem treinado para processar e produzir linguagem natural. |
| Transformer | Arquitetura de Deep Learning baseada em mecanismos de atenção, utilizada em muitos LLMs modernos. |
| Chatbot | Sistema para interagir com usuários por meio de conversas, com regras ou IA. |
| Copiloto | Assistente integrado a atividades e ferramentas para ajudar durante o trabalho. |
| Agente de IA | Sistema capaz de planejar etapas e utilizar ferramentas para executar ações autorizadas. |

### Relação entre as tecnologias

É importante entender que essas áreas não são completamente separadas:

**Inteligência Artificial → Machine Learning → Deep Learning → Transformers → Muitos dos LLMs modernos**

Ou seja, os Transformers são uma arquitetura utilizada dentro do Deep Learning, enquanto os LLMs são modelos de linguagem que frequentemente utilizam essa arquitetura. **Chatbots, copilotos e agentes** são formas de aplicar essas tecnologias, e não uma sequência obrigatória de evolução.

---

## 📖 Referências para estudo

- [Alan Turing — Computing Machinery and Intelligence (1950)](https://doi.org/10.1093/mind/LIX.236.433)
- [Joseph Weizenbaum — ELIZA (1966)](https://doi.org/10.1145/365153.365168)
- [IBM — IA, Machine Learning e Deep Learning](https://www.ibm.com/br-pt/think/topics/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks)
- [IBM — Large Language Models](https://www.ibm.com/think/topics/large-language-models)
- [Google Research — Attention Is All You Need (2017)](https://research.google/pubs/attention-is-all-you-need/)
- [DIO — Potencializando estudos e carreira com IA](https://github.com/digitalinnovationone/potencializando-estudos-carreira-com-ia)
- [Google Antigravity — Documentação da CLI](https://antigravity.google/docs/cli-getting-started?hl=pt-br)

---

> **Observação:** estas anotações fazem parte do meu processo de aprendizado no curso de Cibersegurança do Santander em parceria com a DIO. O objetivo é registrar os principais conceitos apresentados e complementar o conteúdo com exemplos e explicações para facilitar revisões futuras.