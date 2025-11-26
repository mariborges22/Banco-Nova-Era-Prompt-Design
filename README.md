# Banco-Nova-Era-Prompt-Design

Fluxo de validação — fases detalhadas com mensagens do agente (Banco Nova Era, cliente Pedro)
Este guia apresenta o fluxo de validação em quatro fases, explicando cada etapa com clareza e sequência lógica.
Cada caso inclui a mensagem personalizada da agente Mia, adaptada ao contexto do Banco Nova Era e ao cliente Pedro.

Fase 1: Início e protocolo de governança (3 dígitos)
1. 	Saudação personalizada
• 	Explicação: A interação começa reconhecendo o cliente pelo primeiro nome, estabelecendo proximidade e cordialidade.
• 	Mensagem: "Olá, Pedro! Sou a Mia, assistente do Banco Nova Era, e vou te ajudar com sua validação."
2. 	Solicitação de três dígitos do CPF
• 	Explicação: É pedido apenas um pedaço mínimo do documento (os três primeiros dígitos) para iniciar a validação com baixo atrito e sem expor dados completos.
• 	Mensagem: "Para começarmos, me diga apenas os 3 primeiros dígitos do seu CPF, por favor. 🔒"
3. 	Ativação do timer de sessão
• 	Explicação: Inicia-se um temporizador de três minutos para monitorar inatividade e manter a sessão sob controle.
• 	Mensagem (sistema interno, não exibida ao cliente): "(Timer de 3 minutos iniciado para monitorar inatividade)"

Fase 2: Decisão de fluxo e fallback
4. 	Liberação imediata após validação parcial
• 	Explicação: Se os três dígitos conferem com o cadastro e retornam sucesso, o fluxo segue sem exigir mais dados.
• 	Mensagem: "Perfeito, Pedro! Sua validação inicial foi concluída com sucesso. ✅ Vamos prosseguir."
5. 	Solicitação de documento completo como plano B
• 	Explicação: Se o cadastro não for encontrado, o sistema solicita o documento completo para prosseguir sem encerrar a experiência abruptamente.
• 	Mensagem: "Pedro, não encontrei seu cadastro com esses dígitos. Para avançarmos, preciso que você informe o documento completo, por favor."

Fase 3: Validação completa e inteligência (checagem cruzada)
6. 	Conclusão segura com documento válido
• 	Explicação: Ao validar o documento completo, os dados são armazenados de forma criptografada e o acesso é liberado.
• 	Mensagem: "Ótimo, Pedro! Seu documento foi validado com sucesso. 🔐 Agora podemos continuar com seu atendimento no Banco Nova Era."
7. 	Detecção de erro de tipo com alerta cruzado
• 	Explicação: Se o valor informado é inválido para o campo, mas corresponde ao outro tipo de documento, o sistema orienta o ajuste.
• 	Mensagem: "Pedro, parece que você digitou um CNPJ no campo de CPF. Quer tentar novamente informando o documento correto?"
8. 	Erro crítico após esgotar checagens
• 	Explicação: Se não há correspondência nem como CPF nem como CNPJ, o sistema retorna erro final de formato.
• 	Mensagem: "Pedro, o documento informado não pôde ser validado. Verifique o formato e tente novamente."

Fase 4: Gestão de exceções e limites
9. 	Reengajamento por inatividade
• 	Explicação: Ao atingir o timer de três minutos sem resposta, é enviada uma mensagem de retomada.
• 	Mensagem: "Pedro, você ainda está aí? ⏳ Preciso da sua resposta para continuar o atendimento."
10. 	Transbordo humano por limite de tentativas
• 	Explicação: Após três falhas consecutivas na validação completa, o atendimento é encaminhado para um especialista.
• 	Mensagem: "Pedro, notei que houve algumas dificuldades na validação. Vou encaminhar você para um especialista do Banco Nova Era que poderá ajudar melhor."

Encerramento do fluxo
• 	Governança aplicada: minimização de exposição de dados, controle de sessão e armazenamento seguro.
• 	Inteligência prática: mensagens específicas que antecipam erros e reduzem frustração.
• 	Continuidade garantida: sempre há uma rota para concluir a validação ou escalar para suporte humano.

  
