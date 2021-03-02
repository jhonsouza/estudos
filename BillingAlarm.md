## Billing Alarm

- CloudWatch: serviço da AWS que permite o monitoramento da sua nuvem 
- alarme de controle de faturamento da AWS, emiti um alerta toda vez que o gasto do mês ultrapassar o valor definido

- Criação de um alarme de faturamento:
 1. abre o console do CloudWatch
 2. selecione no canto esquerdo faturamento (Billing)
 3. clique em criar alarme (Create alarm)
    - existem dois Create alarm:
     - o do canto superior esquerdo permite escolher as metricas de monitoramento
     - O do meio da tela, criar um monitoramento generico
 4. é possível ajustar o período de monitoramento (por padrão a cada 6h)
 5. existem dois tipos de limite:
    - Estático (Static)
    - Detecção de anomalias
 6. existem 4 metricas para a cobrança:
     1.  `> (Greater): quando o valor da cobrança é maior que o estimado`
     2.  `>= (Greater/Equal): quando valor é maior ou igual ao valo estimado `
     3.  `<= (Lower/Equal): quando o valor é meno ou igual ao valo estimado`
     3.  `< (Lower): quando o valor é menor que o valor estimado`
 7. valor a ser monitorado
 8. Cria de novo tópico SNS (serviço de notificação simples - simple notification service)
    - nome do tópico
    - e-mail que será avisado (necessário confirmação do e-mail)
9. nomaer o alarme e dar uma breve descrição 
10. Criar alarme 
