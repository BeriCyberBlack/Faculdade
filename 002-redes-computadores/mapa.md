{\rtf1\ansi\ansicpg1252\cocoartf2821
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Arial-BoldMT;\f1\fswiss\fcharset0 ArialMT;\f2\fswiss\fcharset0 Helvetica-Bold;
\f3\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red39\green38\blue34;\red79\green79\blue79;
\red255\green255\blue255;\red246\green246\blue245;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;\cssrgb\c20392\c19608\c17647;\cssrgb\c38431\c38431\c38431;
\cssrgb\c100000\c100000\c100000;\cssrgb\c97255\c97255\c96863;}
\paperw11905\paperh16837\margl1133\margr1133\margb1133\margt1133\vieww11520\viewh8400\viewkind0
\deftab720
\pard\pardeftab720\sl276\slmult1\qj\partightenfactor0

\f0\b\fs22 \cf2 Fase 1: Cen\'e1rio\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0\fs24 \cf2 A Tecnologia da Informa\'e7\'e3o (TI) desempenha um papel fundamental no desenvolvimento e na execu\'e7\'e3o das atividades empresariais, sendo respons\'e1vel por garantir efici\'eancia, seguran\'e7a e escalabilidade dos sistemas. Conforme destacado por Laudon e Laudon (2020), os sistemas de informa\'e7\'e3o s\'e3o essenciais para a automa\'e7\'e3o e melhoria dos processos organizacionais, contribuindo diretamente para a competitividade das empresas.\
Al\'e9m disso, segundo Tanenbaum e Wetherall (2011), a infraestrutura de redes de computadores \'e9 respons\'e1vel pela comunica\'e7\'e3o entre dispositivos e sistemas, permitindo o compartilhamento de dados e recursos de forma eficiente.\
Diante desse contexto, este projeto tem como objetivo planejar e implementar uma infraestrutura de rede segura, eficiente e organizada para atender \'e0s necessidades de uma empresa, garantindo conectividade entre setores e controle adequado dos recursos.\
\pard\pardeftab720\sl276\slmult1\qj\partightenfactor0

\fs22 \cf2 \
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b\fs24 \cf2 Fase 2: Infraestrutura B\'e1sica
\f1\b0 \

\f0\b Rede 1 - Componentes\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 - Duas redes independentes e gerenci\'e1veis para distribui\'e7\'e3o do tr\'e1fego.\
- Um ponto de acesso Wi-Fi dedicado.\
- Seis desktops conectados via cabo.\
- Tr\'eas tablets corporativos conectados por IP din\'e2mico.\
- Um servidor de arquivos.\
- A comunica\'e7\'e3o entre a Rede 1 e o servidor dever\'e1 ser protegida.\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Implementa\'e7\'e3o:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Segmentada para tr\'e1fego gerenci\'e1vel, integrando desktops, dispositivos m\'f3veis via Wi-Fi e um servidor de arquivos com camadas de prote\'e7\'e3o espec\'edficas.\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Rede 2 - Componentes:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 4 workstations\
1 computador do gerente (com scanner)\
2 terminais de autoatendimento\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Implementa\'e7\'e3o:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Focada em esta\'e7\'f5es de trabalho administrativas (incluindo Ger\'eancia de TI) e terminais de autoatendimento.\
\pard\pardeftab720\qj\partightenfactor0
\cf2 \
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Servidor Central - Componente:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Servidor \
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Implementa\'e7\'e3o:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Atuar\'e1 como controlador de servi\'e7os de rede (DHCP e DNS) e gateway de seguran\'e7a para controle de acesso \'e0 internet.\
\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Fase 3: Endere\'e7amento IP\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 O endere\'e7amento IP seguiu a l\'f3gica de segmenta\'e7\'e3o por classes privadas, utilizando como crit\'e9rio o Registro Acad\'eamico (RA) para a defini\'e7\'e3o dos octetos de rede e sub-rede.\
Rede 01: 192.168.1.X (Base: \'faltimo d\'edgito do RA)\
Rede 02: 192.168.5.X (Base: pen\'faltimo d\'edgito do RA)\
\pard\pardeftab720\qj\partightenfactor0
\cf2 \
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Fase : Execu\'e7\'e3o\
1- Indica\'e7\'e3o da ferramenta de seguran\'e7a:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 A solu\'e7\'e3o indicada para o cen\'e1rio \'e9 a implementa\'e7\'e3o de um Firewall (NGFW - Next-Generation Firewall).\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Justificativa:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Seguran\'e7a Abrangente e Multicamada, Controle de Tr\'e1fego Interno e Externo e Visibilidade e Controle no N\'edvel da Aplica\'e7\'e3o\
servidor proxy possa ser uma ferramenta \'fatil para o cache de conte\'fado web e a aplica\'e7\'e3o de pol\'edticas de uso da internet, ele n\'e3o possui a robustez e a abrang\'eancia necess\'e1rias para funcionar como o principal dispositivo de seguran\'e7a no cen\'e1rio descrito. A fun\'e7\'e3o de gateway de seguran\'e7a, que controla todo o fluxo de dados entre as redes internas e a internet, \'e9 a especialidade do Firewall.\
\pard\pardeftab720\sl276\slmult1\qj\partightenfactor0

\fs22 \cf2 \
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b\fs24 \cf2 2 - Identifica\'e7\'e3o da topologia utilizada:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 A topologia adotada em ambas as redes \'e9 a Estrela (Star). \
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 Justificativa:
\f1\b0  \
A topologia em estrela oferece a robustez necess\'e1ria para o ambiente administrativo e a agilidade requerida para a rede de dispositivos m\'f3veis e servidores. Ela garante que a infraestrutura seja resiliente a falhas pontuais e esteja preparada para futuras expans\'f5es tecnol\'f3gicas.\uc0\u8232 Cada dispositivo est\'e1 conectado a um ponto central (servidor/switch).\
\

\f0\b 3 - Descri\'e7\'e3o da equipe em cada setor:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f2 \cf3 \CocoaLigature0 \outl0\strokewidth-167 \strokec2 Rede 1: Operacional\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f3\b0 \cf3 \outl0\strokewidth-167 6 Desktops, 3 Tablets, 1 Servidor de Arquivos, 1 AP Wi-Fi\uc0\u8232 9 Profissionais (6 fixos, 3 m\'f3veis)\
\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f2\b \cf3 \outl0\strokewidth-167 Rede 2: Administrativo\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f3\b0 \cf3 \outl0\strokewidth-167 4 Workstations, 1 Scanner, 2 Terminais de Autoatendimento\
5 Profissionais (4 fixos, 1 rotativo)\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0
\cf4 \cb5 \CocoaLigature1 \outl0\strokewidth0 \
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f0\b \cf2 \cb1 Servidor:\
\pard\pardeftab720\sl360\slmult1\qj\partightenfactor0

\f1\b0 \cf2 1 Servidor Central (DHCP, DNS, Firewall)\
Equipe de TI\
\pard\pardeftab720\qj\partightenfactor0

\f3\fs21 \cf3 \
\
\pard\pardeftab720\sl276\slmult1\qj\partightenfactor0

\f0\b\fs24 \cf2 4 - Configura\'e7\'e3o de IPs:\
\pard\pardeftab720\qj\partightenfactor0

\f3\b0\fs28 \cf4 \cb5 \
\pard\pardeftab720\sl408\slmult1\qj\partightenfactor0

\f0\b\fs18 \cf2 \cb1 Dispositivo                 	 Rede	               Endere\'e7o IP		M\'e1scara de Sub-rede	 Gateway\
\pard\pardeftab720\sl408\slmult1\qj\partightenfactor0

\f1\b0 \cf2 Servidor Central		Servidor       192.168.1.1 / 192.168.5.1   	     255.255.255.0       	      \'96\
Servidor de Arquivos	Rede 1         192.168.1.10                	     255.255.255.0 	192.168.1.1 \
Desktops (06 unidades)	Rede 1         192.168.1.11 a 192.168.1.16 	     255.255.255.0     	192.168.1.1 \
Ponto de Acesso Wi-Fi	Rede 1         192.168.1.20            		     255.255.255.0       	192.168.1.1 \
Tablets (03 unidades)	Rede 1         *IP Din\'e2mico (DHCP)*      	     255.255.255.0      	192.168.1.1 \
Workstations (04 unid.)	Rede 2.        192.168.5.11 a 192.168.5.14	     255.255.255.0 	192.168.5.1 \
Terminais (02 unidades)	Rede 2         192.168.5.21 a 192.168.5.22 	     255.255.255.0		192.168.5.1\
\
\
\pard\pardeftab720\partightenfactor0

\f2\b\fs24 \cf3 \cb6 Refer\'eancias bibliogr\'e1ficas\
\pard\pardeftab720\sl276\slmult1\partightenfactor0

\f1\b0 \cf2 \cb1 FOROUZAN, Behrouz A. Comunica\'e7\'e3o de dados e redes de computadores. 4. ed. Porto Alegre: AMGH, 2010.\cb5 \
\cb1 KUROSE, James F.; ROSS, Keith W. Redes de computadores e a internet: uma abordagem top-down. 6. ed. S\'e3o Paulo: Pearson, 2013.\cb5 \
\cb1 LAUDON, Kenneth C.; LAUDON, Jane P. Sistemas de informa\'e7\'e3o gerenciais. 15. ed. S\'e3o Paulo: Pearson, 2020.\cb5 \
\cb1 STALLINGS, William. Criptografia e seguran\'e7a de redes. 6. ed. S\'e3o Paulo: Pearson, 2015.\cb5 \
\cb1 TANENBAUM, Andrew S.; WETHERALL, David J. Redes de computadores. 5. ed. S\'e3o Paulo: Pearson, 2011.}