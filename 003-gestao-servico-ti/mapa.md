# Relatório de Gestão e Infraestrutura de TI

Trabalho há mais de 15 anos em home office, por isso não tenho muitos exemplos modernos. Contudo, na última empresa em que trabalhei presencialmente, enfrentávamos sérios problemas de lentidão de rede, que será o foco deste exemplo.

---

## Etapa 1 – Planejamento, Estruturação e Mapeamento

* **O problema:** A rede da empresa está muito lenta e pessoas sem autorização estão conseguindo acessar arquivos confidenciais e o setor financeiro.
* **Sintomas:** Sistema lento e usuários acessando pastas e dados que não deveriam visualizar.
* **Impactos:** Perda de produtividade, clientes insatisfeitos com a demora no atendimento e risco de vazamento de informações sigilosas.
* **Envolvidos:** Funcionários e clientes.

### Plano de Ação Inicial (Mapeamento)
* Reunir todas as reclamações registradas sobre a lentidão e a demora no atendimento.
* Mapear os horários de pico (momentos mais críticos) e identificar quem está acessando os arquivos confidenciais.
* Planejar a melhoria da infraestrutura de rede e a revisão dos privilégios de acesso.

---

## Etapa 2 – Causa Raiz e Solução

### Técnica aplicada: Os 5 Porquês
**Problema central:** A rede está lenta e arquivos secretos estão expostos.

1. **Por quê?** Há muitos dispositivos utilizando a rede ao mesmo tempo e as pastas compartilhadas estão totalmente liberadas.
2. **Por quê?** Todos os computadores da empresa estão configurados e visíveis na mesma rede lógica.
3. **Por quê?** A rede não passou por um processo de segmentação (divisão em partes).
4. **Por quê?** Não existem regras de privilégios ou limitações de acesso definidas para os perfis dos funcionários.
5. **Por quê?** Faltou um planejamento inicial focado em segurança e governança de TI para mitigar esses riscos.

### Estratégias de Solução

#### Ações Corretivas
* Revogar as permissões de acesso às pastas secretas e restringi-las estritamente aos responsáveis.
* Aplicar políticas de limitação e controle do uso da internet corporativa para aliviar o tráfego geral.

#### Ações Preventivas
* **Segmentação de Rede:** Separar a rede por setores (ex: isolar o setor financeiro do restante dos funcionários), aumentando a velocidade interna e a segurança dos dados.
* **Governança:** Delegar a um profissional a responsabilidade pela gestão contínua da infraestrutura, focado em monitorar acessos e buscar novas soluções para a melhoria do serviço.

---

## Referência Bibliográfica

* PEREIRA, João Messias; BARBOZA, Weslley de Souza; FEITOSA, Yuri Rafael Gragefe. **Gestão de Serviços em TI**. Maringá - PR: Unicesumar, 2019.
