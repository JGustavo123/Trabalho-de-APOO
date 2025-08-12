# Casos de Uso – EventAcad

## Caso de Uso 1 – Cadastro de Evento
**Atores:** Organizador  
**Fluxo Principal:**  
1. Organizador acessa o sistema e faz login  
2. Seleciona a opção "Cadastrar Evento"  
3. Informa nome, tema, local, data, horário, vagas e palestrantes  
4. Salva o cadastro  
**Fluxos Alternativos:**  
- [FA1] Dados obrigatórios não preenchidos → sistema solicita correção  
**Pré-condições:** Organizador autenticado  
**Pós-condições:** Evento cadastrado na base de dados

---

## Caso de Uso 2 – Inscrição em Evento
**Atores:** Participante  
**Fluxo Principal:**  
1. Participante acessa o sistema  
2. Visualiza lista de eventos disponíveis  
3. Seleciona um evento e confirma a inscrição  
**Fluxos Alternativos:**  
- [FA1] Evento com vagas esgotadas → sistema bloqueia inscrição  
**Pré-condições:** Participante autenticado  
**Pós-condições:** Inscrição registrada

---

## Caso de Uso 3 – Emissão de Certificado
**Atores:** Sistema, Participante  
**Fluxo Principal:**  
1. Participante participa do evento  
2. Presença é registrada (manual ou QR Code)  
3. Sistema verifica elegibilidade e gera certificado em PDF  
4. Participante acessa e baixa o certificado  
**Fluxos Alternativos:**  
- [FA1] Participante não cumpriu presença mínima → certificado não gerado  
**Pré-condições:** Evento finalizado e presença registrada  
**Pós-condições:** Certificado emitido
