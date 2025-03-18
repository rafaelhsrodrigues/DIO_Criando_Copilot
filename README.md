# DIO_Criando_Copilot

Resumo da Aula Criando um Copilot do zero:

No Copilot Studio, selecione o ambiente em que irá desenvolver, e na aba lateral selecione AGENTES e então clique+ NOVO AGENTE.
Na próxima página, inserir as seguintes informações:
- Idioma: Selecionar inglês para que seu agente utilize a função Generativa conforme descrito no final dessa página.
- Nome: Um nome descritivo para que seja fácil de identificar.
- Descrição: Use suas próprias palavras para descrever com o que o seu agente deve ajudar, incluindo seu público-alvo e a meta final.
- Instruções: Direcione o comportamento do agente, incluindo suas tarefas e como ele as conclui. 
- Conhecimento: Caso queira inserir neste momento, adicione arquivos ou links para a Base de Conhecimento. 
Antes de finalizar, clique nos "3 pontos", da parte superior direita e selecione EDITAR CONFIGURAÇÕES AVANÇADAS. Aqui, você vai escolher em qual Solução seu agente pertencerá.


## Tópicos
Ao criar o agente, o Copilot Studio insere alguns tópicos automaticamente para serem trabalhados. Para acessá-los, na página inicial do seu agente, clique em TÓPICOS.
Esses tópicos possuem “gatilhos” iniciais, e são acionados quando o usuário escreve determinada frase ou assunto, ou uma ação.

Por exemplo o tópico “Conversation Start”. Quando o usuário abre o chatbot, o tópico Conversation Start é acionado e mostra uma mensagem pré-definida de boas-vindas.
Um outro exemplo é o tópico “End of Conversation”. Esse tópico possui o gatilho “Disparado pelo agente”, ou seja, quando o usuário digita uma mensagem finalizando a conversa, como tchau, até mais, adeus, então o tópico é acionado. Em seguida, no fluxo desse tópico, é feito uma pergunta ao usuário se as dúvidas foram sanadas, e nesse momento há uma arvore de decisão, caso seja respondido “SIM” ou “NÃO”. E dependendo da resposta, o fluxo segue com mais decisões.

### Fallback (tratando o erro)
Um Tópico de sistema importante é o Fallback. Ele é acionado quando o usuário envia uma mensagem sobre algo que o agente não está treinado ou configurado a fazer. Por padrão, o tópico Fallback pede para o usuário reformular a frase duas vezes, se em uma terceira vez o agente ainda não entenda a mensagem, conforme o fluxo do tópico, o usuário é escalonado para falar com um humano (o Fallback redireciona para o Tópico Escalate, e dentro desse tópico, você configura se há possibilidade de escalar para um humano, ou envia uma mensagem ao usuário com algum contato)

### Comentários
Uma boa prática é realizar comentários, explicando a lógica feita para esse tópico. 
Para isso, dentro do tópico, clique em COMENTÁRIO e insira as informações
