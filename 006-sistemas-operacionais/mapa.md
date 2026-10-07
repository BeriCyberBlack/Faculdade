# Atividade de Sistemas Operacionais e Virtualização

## 1. O que é e como funciona a Virtualização

* **A. Conceito e Hypervisor:** Virtualização é pegar um único computador físico e fazer ele funcionar como se fossem vários, podendo rodar sistemas operacionais diferentes como Windows e Linux ao mesmo tempo na mesma máquina. O **Hypervisor** é o programa que divide os recursos do computador real e cria as Máquinas Virtuais (VMs) de um jeito que separa completamente um sistema do outro.

* **B. Tipos de Hypervisor:** 
  * **Tipo 1 (*Bare-metal*):** Instala o programa direto na máquina limpa, sem nenhum sistema operacional por baixo. É o que as empresas usam em servidores grandes porque é mais rápido e seguro.
  * **Tipo 2 (*Hosted*):** Esse programa instalamos no nosso computador do dia a dia. Ele roda como se fosse um aplicativo comum dentro do Windows ou Linux que já está rodando na máquina.

* **C. Máquinas Virtuais vs. Contêineres:** 
  * **Máquinas Virtuais:** Simulam um computador inteiro. São ótimas para isolar tudo, mas são mais pesadas porque rodam um sistema operacional completo lá dentro.
  * **Contêineres:** São bem mais leves. Em vez de simular um computador todo, eles focam em rodar apenas o aplicativo. Na nuvem, são muito utilizados com ferramentas como o **Kubernetes** para criar e fechar serviços rapidamente quando o site recebe muitos acessos.

* **D. Benefícios e Desvantagens:** 
  * **Benefício:** Economia com equipamentos, gastando menos com conta de luz e ar-condicionado. Se uma VM der problema, as outras continuam funcionando normalmente.
  * **Desvantagem:** Quando se colocam muitas Máquinas Virtuais pesadas rodando juntas, elas passam a disputar memória. Isso força o computador a usar o disco rígido como memória reserva, o que deixa o sistema muito lento.

* **E. Aplicações Práticas:** Podemos usar a virtualização na nuvem, que é a base de tudo o que acessamos na internet hoje. As empresas podem aproveitar para rodar sistemas antigos que ainda são necessários, mas utilizando um servidor moderno. Para nós, estudantes, permite testar programas, realizar laboratórios de invasão de sistemas (*pentest*) e testar sistemas operacionais novos sem medo de corromper a nossa própria máquina física.

---

## 2. Estudo de Caso e Análise Crítica

* **A. Consolidação de Servidores:** A empresa deve juntar esses 25 servidores que quase não são usados em apenas 5 computadores físicos robustos, rodando várias máquinas virtuais. Com a redução para apenas 5 máquinas, haverá uma grande diminuição no consumo de energia, redução de espaço físico, menor custo de manutenção, otimização da mão de obra e fim do desperdício de hardware. A questão principal é saber configurar tudo de forma correta para que uma máquina virtual não atrapalhe o desempenho da outra. Para o administrador de redes, fica muito mais fácil por centralizar o controle em um único software, bastando configurar as regras certas e manter rotinas de cópias de segurança (backup).

* **B. Desempenho e Escalabilidade:** Para obter o melhor desempenho, a opção ideal seria adotar o **Hypervisor Tipo 1** nos servidores principais. Com relação à compatibilidade, o correto antes de qualquer escolha é verificar se a solução conversa perfeitamente com o sistema já existente na empresa. Além disso, é primordial garantir que a estrutura seja **escalável**, permitindo aumentar a memória das máquinas virtuais e criar novas instâncias conforme a necessidade de crescimento do negócio.

* **C. Segurança e Mitigação de Riscos:** O maior perigo hoje são os vírus e as invasões com o intuito de roubar dados ou derrubar os sistemas. Uma das principais defesas para proteger esse ambiente virtualizado é a implementação de um **Firewall**, excelente para bloquear conexões estranhas na rede, combinado com uma política rígida de controle de acessos, concedendo privilégios e permissões apenas para as pessoas que realmente precisam mexer no sistema.

* **D. Tendências Futuras e Automação:** Na área de automação, a virtualização ficará cada vez mais automática e imperceptível para o usuário final, integrando-se diretamente com ferramentas de nuvem. Destaca-se o uso de ecossistemas como o **Prometheus** para monitorar Métricas, Logs e Rastreios (observabilidade) em tempo real, permitindo corrigir falhas e gargalos de maneira proativa, antes mesmo que o sistema chegue a travar.

---

## Referência Bibliográfica

* VOLTZ, Wagner Mendes. **Sistemas Operacionais**. Maringá - PR: Unicesumar, 2025.
