# sprin-3-edge

README – Projeto ConectBall
 Integrantes

André Monteiro – RM 562397

Arthur Pastorello – RM 562345

José Henrique Escobar – RM 564419

Gustavo Estevam Cocchi – RM 562472


 
 
 Descrição do Projeto:

O ConectBall é uma plataforma digital inspirada em um LinkedIn para jogadoras de futebol feminino, que conecta atletas, clubes e fãs.
Para enriquecer a experiência e trazer inovação tecnológica, o projeto conta com a implementação de um sensor IoT na bola de futebol, que mede a velocidade dos chutes em tempo real.

Esses dados são enviados para a plataforma, onde podem ser visualizados em dashboards, fortalecendo a visibilidade do talento das atletas e gerando engajamento dos torcedores.

Arquitetura Proposta:
Fluxo Simplificado:

Sensor IoT (na bola): mede a velocidade do chute.

Gateway / MQTT Broker: envia os dados coletados do sensor.

IoT Agent (MQTT): traduz os dados para o padrão de comunicação.

Orion Context Broker: centraliza e gerencia os dados em tempo real.

Banco de Dados (MongoDB): armazena os dados históricos.

Dashboard / Aplicativo Web: apresenta a velocidade da bola e estatísticas para atletas, técnicos e fãs.

 A arquitetura pode ser expandida para Big Data, caso haja coleta em larga escala.


 

 
Recursos Necessários:
Hardware:

Sensor acelerômetro/giroscópio (ex.: MPU6050) acoplado à bola.

Microcontrolador com Wi-Fi (ESP32).

Gateway IoT ou roteador Wi-Fi.

Software/Plataforma:

MQTT Broker (ex.: Mosquitto) para troca de mensagens.

IoT Agent MQTT (FIWARE).

Orion Context Broker (FIWARE).

Banco de Dados MongoDB.

Dashboard Web (React ou Grafana).
 
  
  
  
Instruções de Uso:

Ligar o sensor IoT acoplado à bola.

Conectar o ESP32 à rede Wi-Fi configurada.

O ESP32 coleta os dados e envia via MQTT para o broker.

O IoT Agent traduz os dados e envia ao Orion Context Broker.

O MongoDB armazena os dados históricos.

O Dashboard exibe a velocidade em tempo real e relatórios.









