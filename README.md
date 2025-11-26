# Banco-Nova-Era-Prompt-Design

# Fluxo de validação — fases detalhadas

Este guia apresenta o fluxo de validação em quatro fases, explicando cada etapa com clareza e sequência lógica. O desenho prioriza governança (proteção e conformidade) e inteligência (experiência do usuário com baixo atrito e mensagens úteis).

---

## Fase 1: Início e protocolo de governança (3 dígitos)

1. **Saudação personalizada:** A interação começa reconhecendo o cliente pelo primeiro nome, estabelecendo um tom cordial e humano (RN 3.1).
2. **Solicitação de três dígitos do CPF:** É pedido apenas um pedaço mínimo do documento (os três primeiros dígitos) para iniciar a validação com baixo atrito e sem expor dados completos logo no início (LGPD, governança).
3. **Ativação do timer de sessão:** Inicia-se um temporizador de três minutos para monitorar inatividade e manter a sessão sob controle operacional e de risco.

---

## Fase 2: Decisão de fluxo e fallback

4. **Liberação imediata após validação parcial:** Se os três dígitos conferem com o cadastro e retornam sucesso (status SUCCESS), o fluxo segue sem exigir mais dados, otimizando a jornada (RN 3.2.A).
5. **Solicitação de documento completo como plano B:** Se o cadastro não for encontrado (status NOT_FOUND), o sistema solicita o documento completo para prosseguir com a identificação sem encerrar a experiência abruptamente (RN 3.2.B).

---

## Fase 3: Validação completa e inteligência (checagem cruzada)

6. **Conclusão segura com documento válido:** Ao validar o documento completo, os dados são armazenados de forma criptografada e o acesso é liberado para as próximas etapas do atendimento (RN 3.3.C).
7. **Detecção de erro de tipo com alerta cruzado:** Se o valor informado é inválido para o campo, mas corresponde ao outro tipo de documento (ex.: CNPJ em campo de CPF), o sistema orienta o ajuste de forma inteligente, evitando mensagens genéricas e frustração (RN 3.3.B).
8. **Erro crítico após esgotar checagens:** Se não há correspondência nem como CPF nem como CNPJ, o sistema retorna erro final de formato, encerrando a tentativa com uma orientação clara para correção (RN 4.1).

---

## Fase 4: Gestão de exceções e limites

9. **Reengajamento por inatividade:** Ao atingir o timer de três minutos sem resposta, é enviada uma mensagem de retomada para recuperar a atenção antes de considerar o encerramento (RN 4.2).
10. **Transbordo humano por limite de tentativas:** Após três falhas consecutivas na validação completa, o atendimento é encaminhado para um especialista, evitando ciclo infinito e garantindo resolução definitiva (RN 4.3).

---

## Encerramento do fluxo

- **Governança aplicada de ponta a ponta:** Minimização de exposição de dados, controle de sessão e armazenamento seguro.
- **Inteligência prática:** Decisões rápidas quando há sinal positivo, fallback útil quando há lacuna, e mensagens específicas que antecipam erros comuns.
- **Continuidade garantida:** Nenhum beco sem saída; sempre há uma rota para concluir a validação ou escalar para suporte humano.



  
