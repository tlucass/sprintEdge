#  Desenvolvimento da arquitetura de uma aplicação IoT para Eficiência Energética

A empresa de eficiência energética Akona Energy tem como objetivo oferecer serviços de consultoria altamente eficazes para otimizar o consumo de energia em seus clientes. Para alcançar essa meta, adotou uma arquitetura de aplicação IoT (Internet of Things) que permite a coleta, análise e visualização de dados de consumo de energia. Essa arquitetura é composta por várias camadas interconectadas, cada uma desempenhando um papel vital no processo de eficiência energética.



## Camada de Aplicação:

Na camada de aplicação, concentramos nossa atenção na interface de usuário e nas ferramentas que permitem aos clientes interagir com os dispositivos IoT e os dados de consumo de energia. Os principais componentes desta camada incluem:

#### 📱 App Mobile :
Um aplicativo móvel personalizado que permite aos clientes acessar dados de 	eficiência energética em qualquer lugar e tomar decisões em tempo real. Análise de dados que extraem insights valiosos dos dados coletados, gerando relatórios de desempenho energético.

## Camada de Back-End:
A camada de back-end abriga componentes essenciais para a coleta, armazenamento e gerenciamento de dados de eficiência energética. Os principais componentes incluem:

#### ✅ Orion Context Broker:

- O Orion Context Broker gerencia as entidades e o contexto dos dispositivos 	IoT, garantindo a coleta e atualização de dados em tempo real.

#### ✅ STH-Comet:

- O STH-Comet é responsável pelo armazenamento de dados históricos, incluindo 	informações de consumo de energia ao longo do tempo, permitindo análises 	retrospectivas e detecção de tendências. 

#### ✅ IoT Agent MQTT:

- Este agente IoT estabelece a comunicação eficaz entre os dispositivos IoT e a 	plataforma IoT, garantindo a transmissão confiável de dados.

#### ✅ Banco de Dados NoSQL MongoDB:
- O MongoDB armazena entidades, registros, subscrições e dados históricos, 	oferecendo escalabilidade e eficiência na gestão de dados.

#### ✅ Eclipse-Mosquitto:
- Um broker MQTT essencial para gerenciar a comunicação bidirecional entre os 	dispositivos de IoT e a aplicação.

A interação entre essas camadas é crucial para o funcionamento eficiente da aplicação IoT. Os dispositivos IoT coletam dados de consumo de energia e os enviam para a camada de back-end por meio dos protocolos MQTT ou HTTP/NGSIv2. Os dados são então processados pela camada de back-end, armazenados no MongoDB e disponibilizados para análise por meio da camada de aplicação.

## Camada IoT (Internet of Things):
#### 💡EnergiMonitor:
Características Principais:

- Medição de Consumo de Energia: O dispositivo é equipado com sensores de alta precisão que medem o consumo de energia elétrica. Ele pode ser conectado a tomadas para monitorar o uso em locais específicos.
- Comunicação Sem Fio: O EnergiMonitor utiliza tecnologia sem fio, como Wi-Fi, para transmitir dados de consumo para a plataforma IoT. Isso permite a instalação flexível em locais remotos.
- Análise de Harmônicas: Além do consumo geral de energia, o dispositivo é capaz de detectar harmônicas na qualidade da energia, identificando problemas como distorções de corrente e tensão que podem afetar a eficiência.
- Registro de Dados Históricos: O dispositivo armazena dados históricos de consumo e qualidade da energia, permitindo análises retrospectivas e detecção de tendências ao longo do tempo.
- Conectividade Bidirecional: Ele é capaz de receber comandos de controle da plataforma IoT, permitindo que os usuários ajustem remotamente o consumo de energia em resposta a análises e recomendações.
- Compatibilidade com Protocolos IoT: O EnergiMonitor suporta protocolos padrão de IoT, como MQTT e HTTP/NGSIv2, para facilitar a integração com a plataforma de back-end.
- Notificações em Tempo Real: Quando detecta anomalias no consumo de energia, o dispositivo pode enviar notificações em tempo real para alertar os usuários sobre possíveis problemas ou oportunidades de economia.
- Design Compacto e Instalação Fácil: O dispositivo é projetado para ser compacto e de fácil instalação, permitindo sua colocação discreta em várias partes de uma instalação.
- Alimentação Eficiente: Pode ser alimentado por energia da rede elétrica, garantindo operação contínua.




## ⚙️ Instruções de Uso:

#### Instalação de EnergiMonitor:

- Posicione os dispositivos EnergiMonitor nas tomadas ou locais específicos de monitoramento de energia.
- Certifique-se de que os dispositivos tenham uma conexão sem fio (Wi-Fi) estável para se comunicarem com a plataforma IoT.

#### Configuração do Aplicativo Móvel:

- Faça o download do aplicativo móvel personalizado em smartphones ou tablets.
- Faça login com as credenciais fornecidas pela empresa de eficiência energética.
- Conecte o aplicativo ao dispositivo EnergiMonitor, seguindo as instruções fornecidas no aplicativo.

#### Monitoramento de Consumo de Energia:

- Use o aplicativo móvel para monitorar em tempo real o consumo de energia elétrica nos locais em que os dispositivos EnergiMonitor estão instalados.
- Receba notificações em tempo real se houver anomalias no consumo de energia.

#### Análise de Dados:

- Utilize as ferramentas de análise de dados integradas ao aplicativo móvel para extrair insights dos dados coletados.
- Gerencie e visualize relatórios de desempenho energético para avaliar a eficiência energética.


## 📋 Requisitos:

1. #### Dispositivo EnergiMonitor:

- Certifique-se de que os dispositivos EnergiMonitor estejam devidamente instalados e conectados à rede Wi-Fi.

2. #### Aplicativo Móvel:

- Dispositivos móveis (smartphones ou tablets) com sistema operacional compatível (iOS, Android).
- Conexão à internet para acessar dados em tempo real.

3. #### Camada de Back-End:

- Servidores ou serviços em nuvem que hospedam os componentes da camada de back-end (Orion Context Broker, STH-Comet, IoT Agent MQTT, MongoDB e Eclipse-Mosquitto).
- Conexão estável à internet para garantir a disponibilidade dos serviços em nuvem.

## 🔗 Dependências:

#### Conectividade de Rede:
- Dependência de uma infraestrutura de rede Wi-Fi confiável para a comunicação dos dispositivos EnergiMonitor com a camada de back-end.
