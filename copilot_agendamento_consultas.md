
# 🤖 Copilot: Agendamento de Consultas Médicas

Este projeto simula um copiloto construído com base no **Microsoft Copilot Studio**, com fluxo de conversa personalizado para **agendamento de consultas médicas**.

---

## 🧩 Tópico: Boas-vindas

**Disparadores:**  
`agendar consulta`, `marcar consulta`, `quero uma consulta`, `médico`, `médica`

**Mensagem:**  
```
Olá! 👋 Bem-vindo ao nosso Assistente Virtual de Agendamento Médico.  
Posso te ajudar a marcar sua consulta. Vamos começar?
```

**Ação:**  
Ir para o tópico `Selecionar Especialidade`

---

## 🧩 Tópico: Selecionar Especialidade

**Pergunta:**  
```
Qual especialidade médica você deseja agendar?
```

**Opções de resposta:**
- Clínica Geral
- Pediatria
- Ginecologia
- Dermatologia
- Cardiologia

**Variável salva:** `especialidade`

**Ação:**  
Ir para o tópico `Coletar Nome`

---

## 🧩 Tópico: Coletar Nome

**Pergunta:**  
```
Qual é o seu nome completo?
```

**Variável salva:** `nomePaciente`

**Ação:**  
Ir para o tópico `Selecionar Horário`

---

## 🧩 Tópico: Selecionar Horário

**Mensagem:**  
```
Temos horários disponíveis de segunda a sexta-feira:

🕘 09:00  
🕑 14:00  
🕓 16:00

Qual desses horários prefere?
```

**Variável salva:** `horario`

**Ação:**  
Ir para o tópico `Confirmar Agendamento`

---

## 🧩 Tópico: Confirmar Agendamento

**Mensagem final (com variáveis):**
```
Perfeito, {{nomePaciente}}!

Sua consulta com um(a) especialista em **{{especialidade}}** foi agendada para às **{{horario}}**.

Obrigado por usar nosso sistema! 😊  
Deseja fazer mais alguma coisa?
```

---

## 📦 Como usar este conteúdo

Este fluxo foi simulado manualmente para fins de aprendizado, e pode ser replicado em plataformas como o **Microsoft Copilot Studio**, **Power Virtual Agents** ou ferramentas de criação de bots de atendimento.

