# ZohoCRM_AgendamentoWpp
Este código em Deluge automatiza o envio de mensagens agendadas via WhatsApp utilizando a integração entre o Zoho CRM e a API da GroupAtendimento. O processo verifica as "Deals" marcadas com a flag de agendamento e, se a data e hora forem válidas, envia a mensagem programada ao contato correspondente.

Funcionalidades:
Busca de Deals Agendadas: Verifica todas as Deals com a flag de agendamento ativa no Zoho CRM.
Validação de Data e Hora: Confere se a data e a hora do agendamento são válidas e correspondem à data atual.
Envio de Mensagens Personalizadas: Envia mensagens para o número de WhatsApp do contato relacionado à Deal.
Criação de Atendimento no GroupAtendimento: Se o número for válido no WhatsApp, cria um novo atendimento ou reutiliza um já existente.
Logs de Erros: Registra erros e atualiza as Deals com o status do envio (sucesso ou falha).
Pré-requisitos:
Integração com o Zoho CRM para acesso a Deals e Contatos.
Integração com a API da GroupAtendimento para verificação de números e criação de atendimentos.
Erros Comuns Tratados:
Data ou hora inválidas para o agendamento.
Número de WhatsApp não encontrado.
Usuário responsável pelo atendimento não cadastrado na plataforma GroupAtendimento.
