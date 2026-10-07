# Fase 1: Cenário

A Tecnologia da Informação (TI) desempenha um papel fundamental no desenvolvimento e na execução das atividades empresariais, sendo responsável por garantir eficiência, segurança e escalabilidade dos sistemas. Conforme destacado por **Laudon e Laudon (2020)**, os sistemas de informação são essenciais para a automação e melhoria dos processos organizacionais, contribuindo diretamente para a competitividade das empresas.

Além disso, segundo **Tanenbaum e Wetherall (2011)**, a infraestrutura de redes de computadores é responsável pela comunicação entre dispositivos e sistemas, permitindo o compartilhamento de dados e recursos de forma eficiente.

Diante desse contexto, este projeto tem como objetivo planejar e implementar uma infraestrutura de rede segura, eficiente e organizada para atender às necessidades de uma empresa, garantindo conectividade entre setores e controle adequado dos recursos.

---

# Fase 2: Infraestrutura Básica

### Rede 1 - Componentes
* Duas redes independentes e gerenciáveis para distribuição do tráfego.
* Um ponto de acesso Wi-Fi dedicado.
* Seis desktops conectados via cabo.
* Três tablets corporativos conectados por IP dinâmico.
* Um servidor de arquivos.
* A comunicação entre a Rede 1 e o servidor deverá ser protegida.

**Implementação:**  
Segmentada para tráfego gerenciável, integrando desktops, dispositivos móveis via Wi-Fi e um servidor de arquivos com camadas de proteção específicas.

### Rede 2 - Componentes
* 4 workstations
* 1 computador do gerente (com scanner)
* 2 terminais de autoatendimento

**Implementação:**  
Focada em estações de trabalho administrativas (incluindo Gerência de TI) e terminais de autoatendimento.

### Servidor Central - Componente
* Servidor 

**Implementação:**  
Atuará como controlador de serviços de rede (DHCP e DNS) e gateway de segurança para controle de acesso à internet.

---

# Fase 3: Endereçamento IP

O endereçamento IP seguiu a lógica de segmentação por classes privadas, utilizando como critério o **Registro Acadêmico (RA)** para a definição dos octetos de rede e sub-rede.

* **Rede 01:** `192.168.1.X` (Base: último dígito do RA)
* **Rede 02:** `192.168.5.X` (Base: penúltimo dígito do RA)

---

# Fase 4: Execução

### 1. Indicação da ferramenta de segurança
A solução indicada para o cenário é a implementação de um **Firewall (NGFW - Next-Generation Firewall)**.

* **Justificativa:** Segurança Abrangente e Multicamada, Controle de Tráfego Interno e Externo e Visibilidade e Controle no Nível da Aplicação. Embora um servidor proxy possa ser uma ferramenta útil para o cache de conteúdo web e a aplicação de políticas de uso da internet, ele não possui a robustez e a abrangência necessárias para funcionar como o principal dispositivo de segurança no cenário descrito. A função de gateway de segurança, que controla todo o fluxo de dados entre as redes internas e a internet, é a especialidade do Firewall.

### 2. Identificação da topologia utilizada
A topologia adotada em ambas as redes é a **Estrela (Star)**. 

* **Justificativa:** A topologia em estrela oferece a robustez necessária para o ambiente administrativo e a agilidade requerida para a rede de dispositivos móveis e servidores. Ela garante que a infraestrutura seja resiliente a falhas pontuais e esteja preparada para futuras expansões tecnológicas. Cada dispositivo está conectado a um ponto central (servidor/switch).

### 3. Descrição da equipe em cada setor

* **Rede 1: Operacional**
  * 6 Desktops, 3 Tablets, 1 Servidor de Arquivos, 1 AP Wi-Fi
  * 9 Profissionais (6 fixos, 3 móveis)
* **Rede 2: Administrativo**
  * 4 Workstations, 1 Scanner, 2 Terminais de Autoatendimento
  * 5 Profissionais (4 fixos, 1 rotativo)
* **Servidor:**
  * 1 Servidor Central (DHCP, DNS, Firewall)
  * Equipe de TI

### 4. Configuração de IPs

| Dispositivo | Rede | Endereço IP | Máscara de Sub-rede | Gateway |
| :--- | :--- | :--- | :--- | :--- |
| **Servidor Central** | Servidor | 192.168.1.1 / 192.168.5.1 | 255.255.255.0 | – |
| **Servidor de Arquivos** | Rede 1 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| **Desktops (06 unidades)** | Rede 1 | 192.168.1.11 a 192.168.1.16 | 255.255.255.0 | 192.168.1.1 |
| **Ponto de Acesso Wi-Fi** | Rede 1 | 192.168.1.20 | 255.255.255.0 | 192.168.1.1 |
| **Tablets (03 unidades)** | Rede 1 | *IP Dinâmico (DHCP)* | 255.255.255.0 | 192.168.1.1 |
| **Workstations (04 unid.)** | Rede 2 | 192.168.5.11 a 192.168.5.14 | 255.255.255.0 | 192.168.5.1 |
| **Terminais (02 unidades)** | Rede 2 | 192.168.5.21 a 192.168.5.22 | 255.255.255.0 | 192.168.5.1 |

---

# Referências bibliográficas

* FOROUZAN, Behrouz A. **Comunicação de dados e redes de computadores**. 4. ed. Porto Alegre: AMGH, 2010.
* KUROSE, James F.; ROSS, Keith W. **Redes de computadores e a internet: uma abordagem top-down**. 6. ed. São Paulo: Pearson, 2013.
* LAUDON, Kenneth C.; LAUDON, Jane P. **Sistemas de informação gerenciais**. 15. ed. São Paulo: Pearson, 2020.
* STALLINGS, William. **Criptografia e segurança de redes**. 6. ed. São Paulo: Pearson, 2015.
* TANENBAUM, Andrew S.; WETHERALL, David J. **Redes de computadores**. 5. ed. São Paulo: Pearson, 2011.
