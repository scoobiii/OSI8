DeepEnergy and DeepCooling as the 8th OSI Layer

Eco Hold ecohold76@gmail.com
Aug 7, 2023, 7:32 PM (5 days ago)
to melody.mcelwee, silander, jain, abnt, contact-powerapi

Subject: Proposal for Inclusion of Power and Cooling as the 8th OSI Layer

Dear Committee Members of ISO/TC 301 Energy Management and Energy Savings and ISO/IEC JTC 1/SC 6 Telecommunications and Information Exchange Between Systems,

I hope this email finds you well. My name is José Soares Sobrinho, and I am writing to you regarding a proposal that I believe could significantly enhance the OSI reference model and address critical considerations in today’s networking landscape. I am a student and researcher passionate about the field of computer networks, and I would like to present an idea for your consideration.

The OSI reference model has been a foundational framework in the world of computer networking, providing a structured approach to understanding and designing network protocols and devices. However, as our networks evolve and become increasingly complex, there are certain aspects that the model does not adequately address. Specifically, I am referring to the critical factors of power and cooling.

Cooling and power are two fundamental components for the operation of computer networks. Effective cooling is essential to maintain network equipment within safe temperature ranges, while stable power supply is necessary to ensure uninterrupted operation. Unfortunately, these crucial aspects are not explicitly integrated into the OSI reference model, potentially leading to a range of issues such as equipment failures, service interruptions, increased energy costs, and negative environmental impacts.

In light of this, I propose the inclusion of a new layer, termed the “Power and Cooling Layer,” as the 8th layer within the OSI reference model. This layer would address the considerations related to power supply, energy efficiency, and cooling mechanisms. Just as the other layers in the OSI model provide specific functionalities and services, this new layer would focus on ensuring that network protocols and devices are designed to effectively manage power consumption, cooling requirements, and energy efficiency.

The integration of the Power and Cooling Layer would offer several benefits to the networking ecosystem, including:

Improved Network Reliability: By explicitly considering power and cooling aspects, the network’s overall reliability can be enhanced, reducing the risk of equipment failures due to overheating and power shortages.

Enhanced Network Performance: Proper management of power consumption and cooling can lead to optimized performance and reduced instances of service disruptions.

Better Energy Efficiency: The Power and Cooling Layer would promote energy-efficient designs, contributing to reduced energy consumption and associated costs.

Reduced Environmental Impact: By optimizing power usage and cooling mechanisms, the environmental impact of network operations can be minimized.

I kindly request your consideration in discussing the inclusion of the Power and Cooling Layer in the OSI reference model within your esteemed committees. This addition could align the model with the evolving needs of modern networks and ensure that power and cooling aspects are given due importance. Moreover, I believe that the inclusion of this layer would enhance the overall sustainability and effectiveness of computer networks.

Thank you for taking the time to read my proposal. I would be honored to provide further insights, data, or engage in discussions regarding this idea. Your guidance and expertise are invaluable, and I look forward to any feedback or recommendations you may have.

Sincerely,

José Soares Sobrinho
Email: ecohold76@gmail.com
Phone: +5511 986 542 351

Attachment: - Additional Documentation or References
https://medium.com/@ecohold76/power-and-cooling-the-8th-osi-layer-d37a4da276f6

)

(YURI GRINSHTEYN: Google acquired Stackdriver back in 2014,
0:02
and the suite of operations tools in Google Cloud
0:04
has come a very long way since then.
0:06
Today, cloud monitoring is built right into the Cloud Console,
0:10
and I’m here to show you how to set up and use monitoring
0:12
in your cloud projects.
0:13
This is the Stack Doctor.
0:15
[MUSIC PLAYING]
0:18
0:22
With the integration of monitoring features
0:23
into the Cloud Console, you’ll notice that the Stackdriver
0:26
brand is gone.
0:27
But the functionality you’ve come to depend on
0:29
isn’t changing.
0:30
You’ll still be able to use all of the features you’re used to.
0:33
Let’s take a look at those, and what’s new.
0:35
Let’s start by selecting monitoring
0:37
from the products menu.
0:38
Instead of opening the Stackdriver UI in a new window,
0:41
you get a new, better design UI right in the console.
0:44
Note that you can still select or configure
0:46
the workspace in this new UI.
0:47
The concept of workspaces and using them
0:49
to aggregate monitoring data across multiple projects
0:52
hasn’t changed.
0:53
Workspaces and their host projects
0:54
are still how you create and retain
0:56
monitoring configuration data.
0:58
Let’s take a look at the core features of cloud monitoring.
1:01
We’ll start by setting up a VM and deploying a web
1:03
server on it.
1:04
From there, we’ll install the monitoring agent,
1:06
set up an uptime check, and configure a dashboard
1:08
to show us the health of our new service.
1:10
We’ll put the link to the full steps in the episode notes
1:13
so you can easily follow along.
1:15
Start by creating a compute engine virtual machine
1:17
by going to the products menu and selecting Compute Engine.
1:20
From there, create a new instance.
1:21
You can leave most options at default.
1:23
Once the instance is created, use the SSH functionality
1:26
in the console to open a secure terminal
1:28
session to your new VM.
1:29
We’re going to use this to do two things–
1:31
install the Apache web server and install the monitoring
1:34
agent.
1:35
First run sudo apt-get update and sudo apt-get
1:38
install apache php to get the latest package versions,
1:42
and install Apache.
1:43
Then, run these two commands to download and install
1:46
the monitoring agent.
1:47
Now that the environment is set up,
1:49
we’re ready to configure cloud monitoring.
1:51
Let’s first create an uptime check
1:53
that will monitor our web service
1:54
and potentially notify us if there’s a problem.
1:56
From the Products menu, select Monitoring
1:58
and go to Uptime Checks.
2:00
Create a new one.
2:00
You’ll need to give the machine’s external IP address
2:02
to enter as the target here.
2:04
Test the check before saving it to make sure everything
2:06
is configured properly.
2:08
Note that this IP address is ephemeral by default
2:10
and may change.
2:12
You may want to assign a static IP address to this machine,
2:14
if this is a service with external users or consumers.
2:18
From here, let’s configure a dashboard
2:20
so we can easily visualize the health of our small service.
2:22
We can include charts showing us the availability
2:25
and performance of our uptime check
2:26
and charts showing us infrastructure utilization
2:29
to get a complete picture.
2:31
Go to Products, select Monitoring,
2:32
and click on Dashboards.
2:34
Then create a new dashboard.
2:35
To add a chart showing uptime check failures,
2:38
select Uptime Check URL as the resource,
2:40
and check Past as the metric.
2:42
Filter the data through just the uptime check you just created
2:45
and use the Count False aggregator to only show you
2:47
failures.
2:48
Once you’ve saved this chart, you
2:50
can follow a similar process to add other charts
2:52
to your dashboard.
2:53
You might want to include a chart showing
2:54
the performance of your service as reflected
2:56
by the uptime check latency metric.
2:57
You can also include charts showing
2:59
your resource utilization of your infrastructure.
3:01
Looking at metrics like CPU utilization of your VM
3:03
is a great place to start.
3:05
One of the new features that’s being made available
3:08
with this release is the Dashboards API.
3:10
You’ll now be able to automate the creation of dashboards
3:12
in your workspaces and generally automate
3:14
more of your monitoring setup.
3:16
We’ll come back to dashboard and monitoring
3:18
automation in future episodes.
3:19
Once your monitoring is setup, you’ll
3:21
probably want alerting to get notified
3:23
if the service goes down.
3:24
Since we’ve already set up the monitoring,
3:26
we can create a new alerting policy
3:28
by clicking on it in the menu.
3:29
We can set our uptime check as the resource type,
3:32
and set the metric to make sure that it passes,
3:34
then set up an email notification.
3:36
If you want to see more details on how to set it up,
3:38
check out the link below to the earlier
3:40
video we did on alerting.
3:42
That wraps up our intro to cloud monitoring
3:44
and our tour of its new integration
3:45
in the Cloud Console.
3:47
We created a service, configured a dashboard
3:49
to show us its health, and set up
3:50
alerting to let us know if it has any issues.
3:53
You are now ready to start using cloud monitoring
3:55
in your own environment.
3:56
I hope you are as excited about the future of cloud monitoring
3:59
and these new features as I am.
4:00
That’s it for this episode.
4:02
Come back next time, when we take a look
4:03
at what’s new in cloud logging.
4:05
This is the Stack Doctor.
4:06
Stay healthy out there.
4:07
[MUSIC PLAYING])
2 (Guia de início rápido: monitorar uma máquina virtual do Compute Engine
Monitorar uma máquina virtual do Compute Engine
bookmark_border
Neste documento, mostramos como monitorar um servidor da Web Apache instalado em uma instância de máquina virtual (VM) do Compute Engine.

Se você quiser monitorar uma instância de VM do Amazon EC2, consulte o guia de início rápido Primeiros passos com o monitoramento da AWS.

Neste guia de início rápido, você fará as ações a seguir:

Criar uma instância de VM do Compute Engine.
Instalar um servidor da Web Apache
Instalar e configurar o Agente de operações para o servidor da Web Apache
Gere métricas de tráfego e visualização no painel predefinido do Apache.
Crie uma política de alertas.
Fazer a limpeza.
Antes de começar
Algumas das etapas deste documento podem não funcionar corretamente se sua organização aplicar restrições ao ambiente do Google Cloud. Nesse caso, talvez não seja possível concluir tarefas como criar endereços IP públicos ou chaves de contas de serviço. Se você fizer uma solicitação que retorne um erro sobre restrições, veja como Desenvolver aplicativos em um ambiente restrito do Google Cloud.

Você precisa ter um projeto do Google Cloud com faturamento ativado para concluir este guia de início rápido. Se você não tiver um projeto do Google Cloud ou se o faturamento não estiver ativado para o projeto do Google Cloud, faça o seguinte:

Se você começou a usar o Google Cloud agora, crie uma conta para avaliar o desempenho dos nossos produtos em situações reais. Clientes novos ganham US$ 300 em créditos para executar, testar e implantar cargas de trabalho.
No console do Google Cloud, na página do seletor de projetos, selecione ou crie um projeto do Google Cloud.

Observação: se você não pretende manter os recursos criados neste procedimento, crie um projeto novo em vez de selecionar um que já existe. Depois de concluir essas etapas, é possível excluir o projeto. Para fazer isso, basta remover todos os recursos associados a ele.
Acessar o seletor de projetos

Verifique se a cobrança está ativada para o seu projeto do Google Cloud.

Se você tiver um canal de notificação por e-mail configurado, pule esta etapa.

Para configurar um canal de notificação por e-mail, faça o seguinte:

No Console do Google Cloud, selecione o Cloud Monitoring ou clique no botão a seguir:

Acessar Monitoring
Selecione Alerting.
Clique em edit Editar canais de notificação.
Na seção E-mail, clique em Adicionar novo e preencha a caixa de diálogo.
Criar uma instância de VM do Compute Engine
Recomendamos que você crie uma nova instância de VM do Compute Engine para este guia de início rápido porque instala e configura o software.

No Console do Google Cloud, acesse Compute e selecione Compute Engine:

Acessar o Compute Engine

Para criar uma instância de VM, clique em Criar instância.

Preencha os campos da instância da seguinte forma:

No campo Nome, use quickstart-vm.
No campo Tipo de máquina, selecione Small.
Verifique se o disco de inicialização está configurado para o Debian GNU/Linux.
Em Firewall, selecione Permitir tráfego HTTP e Permitir tráfego HTTPS.
Não altere os valores padrão dos outros campos.

Clique em Criar. Quando a VM estiver pronta, ela aparecerá na lista de instâncias na guia Instâncias.

Instalar um servidor da Web Apache
Para implantar um servidor da Web Apache na instância de VM do Compute Engine, faça o seguinte:

Para abrir um terminal na instância, na coluna Conectar, clique em SSH.

Para atualizar as listas de pacotes na instância, execute o seguinte comando:

sudo apt-get update
Para instalar um servidor HTTP Apache2, execute o seguinte comando:

sudo apt-get install apache2 php7.0
Observação: se o comando anterior falhar, use sudo apt-get install apache2 php. Se você for solicitado a continuar a instalação, insira Y.
Abra o navegador e conecte-se ao servidor HTTP Apache2 usando o URL http://EXTERNAL_IP, em que EXTERNAL_IP é o endereço IP externo da VM. Esse endereço está na coluna IP externo da instância de VM.

Você verá a página padrão do Apache2:

Exibição da página padrão do Apache2.

Instalar e configurar o Agente de operações
Para coletar registros e métricas do seu servidor da Web Apache, instale o agente de operações usando o terminal:

Para abrir um terminal na instância de VM, na coluna Conectar, clique em SSH.

Para instalar o agente de operações, execute o seguinte comando:

curl -sSO https://dl.google.com/cloudagents/add-google-cloud-ops-agent-repo.sh
sudo bash add-google-cloud-ops-agent-repo.sh --also-install
Você verá o seguinte: google-cloud-ops-agent installation succeeded.

Copie o comando a seguir e cole-o no terminal:

Configures Ops Agent to collect telemetry from the app and restart Ops Agent.
set -e

Create a back up of the existing file so existing configurations are not lost.
sudo cp /etc/google-cloud-ops-agent/config.yaml /etc/google-cloud-ops-agent/config.yaml.bak

Configure the Ops Agent.
sudo tee /etc/google-cloud-ops-agent/config.yaml > /dev/null << EOF
metrics:
receivers:
apache:
type: apache
service:
pipelines:
apache:
receivers:
- apache
logging:
receivers:
apache_access:
type: apache_access
apache_error:
type: apache_error
service:
pipelines:
apache:
receivers:
- apache_access
- apache_error
EOF

sudo service google-cloud-ops-agent restart
sleep 60
O comando anterior cria a configuração para coletar e ingerir registros e métricas do servidor da Web Apache. Para mais informações sobre como ingerir registros do servidor da Web do Apache, consulte Configurar o agente de operações do servidor da Web do Apache.

Gerar tráfego e ver métricas
Com os painéis de monitoramento, é possível visualizar e analisar métricas relacionadas aos seus serviços. Neste guia de início rápido, você gera métricas no servidor da Web Apache e visualiza os dados no painel Visão geral do Apache GCE criado automaticamente.

Para gerar métricas no servidor da Web Apache, siga estas etapas:

No Console do Google Cloud, acesse o Compute Engine:

Acessar o Compute Engine

Na coluna Conectar, clique em SSH para abrir um terminal para a instância de VM.

Para gerar tráfego no servidor da Web Apache, execute o seguinte comando:

timeout 120 bash -c – ‘while true; do curl localhost; sleep $((RANDOM % 4)) ; done’
O comando anterior gera tráfego fazendo uma solicitação ao servidor da Web Apache a cada quatro segundos.

Para visualizar o painel Visão geral do Apache GCE, faça o seguinte:

No Console do Google Cloud, selecione Monitoring ou clique no botão a seguir:
Acessar Monitoring

No painel de navegação, selecione Painéis de dados.

Em Todos os painéis, selecione o painel Apache GCE Overview. O painel é aberto.

No painel, há vários gráficos que contêm informações sobre a integração do Apache e do Compute Engine:

Exemplo do painel “Visão geral do Apache GCE”.

Crie uma política de alertas
Observação: se você não tiver configurado um canal de notificação por e-mail, consulte Configurar a notificação por e-mail na seção Antes de começar deste guia de início rápido.
Para criar uma política de alertas que monitore uma métrica e envie uma notificação por e-mail quando a taxa de tráfego no servidor da Web do Apache exceder 4 KiB/s, faça o seguinte:

No Console do Google Cloud, selecione Monitoring ou clique no botão a seguir:
Acessar Monitoring

No painel de navegação, selecione notifications Alertas e clique em Criar política.

Selecione a série temporal a ser monitorada:

Clique em Selecionar uma métrica e insira Instância de VM na barra de filtro.

Na lista Categorias de métricas ativas, selecione Apache.

Na lista Métricas ativas, selecione workload/apache.traffic.

O gráfico de tráfego do Apache é exibido.

Na seção Transformar dados, selecione os seguintes valores:

Janela contínua: 1 minuto

Função de janela contínua: taxa

Na seção Configurar acionador de alertas, selecione os seguintes valores e clique em Avançar:

Acionador de alerta: quaisquer violações de série temporal

Posição limite: acima do limite

Valor do limite: 4.000.

Na seção Configurar notificações e finalizar alerta, selecione os seguintes valores:

Canais de notificação: o e-mail para o qual você deseja receber alertas.

Duração do fechamento automático de incidentes: 30 minutos

Nomeie a política de alertas: tráfego do Apache acima do limite

Clique em Criar política. Sua política de alertas está ativa.

Testar a política de alertas
Para testar a política de alertas que você acabou de criar, faça o seguinte:

No Console do Google Cloud, acesse Compute e selecione Compute Engine:

Acessar o Compute Engine

Na coluna Conectar, clique em SSH para abrir um terminal para a instância de VM.

No terminal, digite o seguinte comando:

timeout 120 bash -c – ‘while true; do curl localhost; sleep $((RANDOM % 4)) ; done’
O comando anterior gera tráfego no servidor da Web do Apache.

Uma notificação por e-mail é enviada depois que o valor limite de taxa de tráfego de 4 KiB/s é excedido no servidor da Web Apache. O processo pode levar alguns minutos para ser concluído.

A notificação por e-mail que você recebe é semelhante a esta:

Notificação por e-mail da política de alertas de tráfego do Apache.

Limpeza
Para evitar cobranças na sua conta do Google Cloud pelos recursos usados nesta página, siga estas etapas.

Se você criou um novo projeto do Google Cloud para este guia de início rápido, exclua o projeto do Google Cloud:

Cuidado: excluir um projeto tem os seguintes efeitos:
Tudo no projeto é excluído. Se você tiver usado um projeto existente para as tarefas neste documento, a exclusão dele incluirá a exclusão de quaisquer outros trabalhos feitos no projeto.
Os IDs do projeto personalizados são perdidos. Ao criar o projeto, você pode ter criado um código do projeto personalizado para ser usado no futuro. Para preservar os URLs que usam o ID do projeto, como um URL appspot.com, exclua recursos específicos do projeto, em vez de excluir o projeto inteiro.
No Console do Google Cloud, acesse a página Gerenciar recursos.
Acessar “Gerenciar recursos”

Na lista de projetos, selecione o projeto que você quer excluir e clique em Excluir .
Na caixa de diálogo, digite o ID do projeto e clique em Encerrar para excluí-lo.
Se você criou uma nova VM em um projeto, exclua a instância de VM:

No Console do Google Cloud, acesse a página Instâncias de VMs.
Acessar instâncias de VM

Marque a caixa de seleção de a instância que você quer excluir.
Para excluir a instância, clique em more_vert Mais ações, clique em Excluir e siga as instruções.
Se você usou uma instância de VM atual neste guia de início rápido, desinstale o agente de operações:

Para desinstalar o agente de operações, abra o terminal e execute o seguinte comando:

sudo bash add-google-cloud-ops-agent-repo.sh --uninstall
A seguir
Para saber como criar painéis personalizados, consulte Gerenciar painéis personalizados.

Para saber como usar o Cloud Logging para visualizar registros no servidor da Web Apache instalado em uma VM do Compute Engine, consulte Cloud Logging para VMs do Compute Engine.

Para mais informações sobre o Logging e a relação dele com o Monitoring, consulte Logging.

Para uma lista completa das métricas compatíveis com o Google Cloud, consulte a Lista de métricas. Se quiser criar as próprias métricas do Monitoring, consulte Métricas personalizadas.)
3 (Visão geral do Cloud Monitoring

bookmark_border
Neste documento, fornecemos uma visão geral do Cloud Monitoring, que faz parte do pacote de operações do Google Cloud. O Cloud Monitoring é integrado à maioria dos serviços do Google Cloud e coleta e armazena automaticamente informações de desempenho sobre esses serviços. Ele também pode coletar métricas do sistema e de aplicativos de terceiros. As ferramentas de visualização e análise de dados fornecidas pelo Cloud Monitoring ajudam você a responder a perguntas importantes, como as seguintes:

Qual é a carga do meu serviço?
Meu site está respondendo corretamente?
Meu serviço tem um bom desempenho?
O Cloud Monitoring oferece suporte ao Console do Google Cloud e à API para a maioria dos serviços, e as páginas de referência da API Cloud Monitoring, como a página alertPolicies.list, permitem testar chamadas de API diretamente da página de referência.

Este documento é destinado a desenvolvedores e administradores de sistemas que precisam monitorar o desempenho de um serviço ou sistema.

Monitorar a carga em um serviço
Para entender a carga atual em um serviço ou para visualizar os dados de desempenho dele no último mês, use as ferramentas de gráficos e painéis. É possível criar gráficos e monitorar dados de métricas (numéricas) que seu projeto do Google Cloud coleta, incluindo:

Métricas do sistema geradas pelos serviços do Google Cloud. Essas métricas fornecem informações sobre como o serviço está operando. Por exemplo, o Compute Engine informa mais de 25 métricas exclusivas para cada instância de máquina virtual (VM). Para uma lista completa de métricas, consulte Métricas do Google Cloud.

Métricas do sistema e do aplicativo que os agentes do pacote de operações do Google Cloud coletam. Essas métricas fornecem mais informações sobre recursos do sistema e aplicativos executados em instâncias do Compute Engine. Outra opção é configurar o agente para coletar métricas de plug-ins de terceiros, como servidores da Web Apache ou Nginx, ou bancos de dados MongoDB ou PostgreSQL.

Métricas definidas pelo usuário gravadas pelo serviço usando a API Cloud Monitoring ou uma biblioteca como a OpenTelemetry.

Métricas com base em registros, que coletam informações numéricas sobre os registros gravados no Cloud Logging. As métricas com base em registros definidas pelo Google incluem contagens de erros que seu serviço detecta e o número total de entradas de registro recebidas pelo seu projeto do Google Cloud. Também é possível definir métricas com base em registros. Por exemplo, é possível criar uma métrica que conta o número de erros 404 Not Found para um aplicativo implantado no App Engine.

Para visualizar seus dados para ver tendências, identificar outliers e ver outros detalhes sobre eles, use as seguintes ferramentas:

Painéis do Google Cloud: o Cloud Monitoring cria automaticamente esses painéis com base nos recursos usados pelo projeto do Google Cloud.

Por exemplo, quando um projeto do Google Cloud contém instâncias de VM do Compute Engine, os painéis para essas instâncias de VM e discos são criados automaticamente. Ao usar o painel Instâncias de VM, é possível ver detalhes, como o uso de memória e disco, identificar endereços IP e identificar quais VMs estão descartando pacotes de rede. Esse painel também exibe informações sobre o uso do agente do Cloud Monitoring e fornece sugestões para instrumentação.

Painéis personalizados: você cria ou instala esses painéis. Os painéis personalizados permitem definir quais dados você quer visualizar e como ver esses dados. Por exemplo, é possível exibir dados de métricas, políticas de alertas e registros armazenados no projeto do Google Cloud. É possível exibir dados de série temporal em um gráfico, com um medidor, visão geral ou em formato tabular. Os painéis também são compatíveis com widgets de texto. É possível criar um painel personalizado com a API Dashboards ou com o Console do Google Cloud.

Gráficos: é possível adicionar gráficos a um painel personalizado ou usar o Metrics Explorer, uma ferramenta de gráficos usada para criar rapidamente gráficos e explorar dados de série temporal. É possível salvar gráficos criados com o Metrics Explorer em um painel personalizado.

Ao criar um gráfico, você seleciona os dados de série temporal que deseja visualizar. Por exemplo, é possível configurar um gráfico para exibir dados de instâncias de VM do Compute Engine que estão localizadas na zona us-east-1d.

As configurações do gráfico permitem comparar dados atuais com dados anteriores, exibir valores atípicos e percentuais e exibir várias métricas. Por exemplo, a captura de tela a seguir mostra um gráfico que exibe o número de bytes lidos e gravados por uma única VM:

O Metrics Explorer exibe bytes de leitura e gravação de disco.

Para mais informações sobre como visualizar dados de série temporal, consulte Como usar painéis e gráficos.

Monitorar a disponibilidade do site
Para monitorar se um site está respondendo, configure uma verificação de tempo de atividade. Essas verificações sondam periodicamente o serviço de uma maneira que imita como os clientes acessam o serviço e registram o sucesso e a latência da sondagem.

Para visualizar informações sobre suas verificações de tempo de atividade, o Cloud Monitoring fornece um painel que resume o status de cada verificação e, para cada verificação, apresenta um painel com informações detalhadas. A visualização detalhada de uma verificação de tempo de atividade exibe o sucesso ou a falha da resposta e a latência dela, além de detalhes sobre essa verificação:

Amostra de visualização detalhada de uma verificação de tempo de atividade.

Para mais informações sobre esse tópico, consulte Como gerenciar verificações de tempo de atividade.

Receber notificações quando um serviço não tiver um bom desempenho
Para receber notificações quando o desempenho de um serviço atender aos critérios definidos por você, crie uma política de alertas. Por exemplo, é possível criar uma política de alertas que notifique sua equipe de plantão quando o 90o percentil da latência de respostas HTTP 200 do seu serviço exceder 100 ms. Da mesma forma, você pode ser notificado quando uma verificação de tempo de atividade falhar.

Com as políticas de alertas, você configura se uma única série temporal pode atender a uma condição ou se várias séries temporais precisam atender à condição antes de ser atendida. As políticas de alertas podem ser simples ou complexas. Exemplo:

Notifique-me quando qualquer verificação de tempo de atividade para o domínio example.com falhar por pelo menos três minutos.

Notifique a equipe de plantão quando o 90º percentil das respostas HTTP 200 exceder uma latência de 100 ms para três ou mais servidores da Web em dois locais do Google Cloud, desde que haja menos de 15 QPS no servidor.

Avisar se a carga de CPU de qualquer instância de VM no projeto do Google Cloud estiver acima do limite de 0,6.

O Cloud Monitoring fornece um painel que resume o status das suas políticas de alertas e, para cada política, fornece um painel com informações detalhadas. Conforme mostrado na captura de tela a seguir, o painel detalhado de um alerta exibe os dados que estão sendo monitorados, o limite do alerta, os canais de notificação, uma lista de incidentes e qualquer documentação definida pelo usuário incluída em uma notificação:

Política de alertas que monitora a carga da CPU.

As condições são o componente principal de uma política de alertas. Uma condição descreve um possível problema com o sistema que você quer que o Cloud Monitoring monitore. Por exemplo, você pode descrever condições como as seguintes:

Qualquer verificação de tempo de atividade para o domínio example.com falha por pelo menos três minutos.
O espaço livre de qualquer instância de VM monitorada é inferior a 10%.
Quando as condições de uma política de alertas são atendidas, por exemplo, quando cada verificação de tempo de atividade do domínio example.com falha por três minutos, o Cloud Monitoring abre um incidente e emite notificações.

Um incidente é um registro permanente que armazena informações sobre o recurso que está sendo monitorado. Por exemplo, uma política de alertas que monitora o uso da CPU armazenaria informações sobre a VM cuja utilização faz com que a condição seja atendida. Quando a condição para de ser atendida, o incidente é fechado automaticamente. É possível visualizar todos os incidentes, abertos e fechados, usando o painel de alertas.

Especifique quem será notificado quando configurar uma política de alertas. Ele é compatível com canais de notificação comuns, incluindo e-mail, Cloud Mobile App e serviços como o PagerDuty ou o Slack. Para ver uma lista completa de canais de notificação, consulte Criar e gerenciar canais de notificação.

Para mais informações sobre políticas de alertas, consulte Visão geral de alertas.

Monitorar sistemas grandes
Nesta seção, descrevemos como gerenciar recursos como uma coleção e como monitorar métricas armazenadas em vários projetos do Google Cloud.

Gerenciar recursos como uma coleção
Para gerenciar os recursos como uma coleção em vez de individualmente, crie um grupo de recursos. Um grupo de recursos é uma coleção dinâmica de recursos que satisfazem alguns critérios fornecidos por você. À medida que você adiciona e remove recursos, por exemplo, ao adicionar instâncias de VM do Compute Engine ao projeto do Google Cloud, a associação no grupo é alterada automaticamente. Veja a seguir exemplos de grupos de recursos:

Instâncias do Compute Engine com nomes que começam com a string prod-.
Recursos com a tag test-cluster.
Instâncias do Amazon EC2 na região A ou região B.
Depois de definir um grupo de recursos, é possível monitorar o grupo como se fosse um único recurso. Por exemplo, é possível configurar uma verificação de tempo de atividade para monitorar um grupo de recursos. Para gráficos e políticas de alertas, também é possível filtrar com base no nome do grupo.

Para mais informações sobre esse tópico, consulte Configurar grupos de recursos.

Monitorar métricas de vários projetos do Google Cloud
Para visualizar e monitorar os dados de série temporal para vários projetos do Google Cloud e contas da AWS por meio de uma única interface, configure um escopo de métricas de vários projetos.

Por padrão, as páginas do Cloud Monitoring no Console do Google Cloud fornecem acesso apenas à série temporal armazenada no projeto de escopo. O projeto de escopo é o que você selecionou com o seletor de projetos do Console do Google Cloud. O projeto de escopo armazena os alertas, verificações de tempo de atividade, painéis e grupos de monitoramento que que você configura.

O projeto de escopo também hospeda um escopo de métricas. O escopo de métricas define os projetos e as contas com métricas visíveis para o projeto de escopo. É possível configurar o escopo das métricas para incluir dados de série temporal de outros projetos do Google Cloud e de contas da AWS. Para informações sobre como modificar um escopo de métricas, consulte Configurar um escopo de métricas para vários projetos.

Modelo de dados do Cloud Monitoring
Nesta seção, apresentamos o modelo de dados do Cloud Monitoring:

Uma métrica descreve algo que é medido. Exemplos de métricas incluem a utilização da CPU de uma VM e a porcentagem de um disco usado.

Uma série temporal é uma estrutura de dados que contém medições com carimbo de data/hora de uma métrica e informações sobre a origem e o significado dessas medidas.

Por exemplo, o exemplo a seguir ilustra uma série temporal:

“timeSeries”: [
{
“points”: [
{
“interval”: {
“startTime”: “2020-07-27T20:20:21.597143Z”,
“endTime”: “2020-07-27T20:20:21.597143Z”
},
“value”: {
“doubleValue”: 0.473005
}
},
{
“interval”: {
“startTime”: “2020-07-27T20:19:21.597239Z”,
“endTime”: “2020-07-27T20:19:21.597239Z”
},
“value”: {
“doubleValue”: 0.473025
}
},
],
“resource”: {
“type”: “gce_instance”,
“labels”: {
“instance_id”: “2708613220420473591”,
“zone”: “us-east1-b”,
“project_id”: “sampleproject”
}
},
“metric”: {
“labels”: {
“device”: “sda1”,
“state”: “free”
},
“type”: "agent.googleapis.com/disk/percent_used"
},
“metricKind”: “GAUGE”,
“valueType”: “DOUBLE”,

},
Veja alguns detalhes sobre o que uma série temporal contém:

A matriz points contém as medidas com carimbo de data/hora.

No exemplo anterior, a matriz points contém dois valores:

“points”: [
{
“interval”: {
“startTime”: “2020-07-27T20:20:21.597143Z”,
“endTime”: “2020-07-27T20:20:21.597143Z”
},
“value”: {
“doubleValue”: 0.473005
}
},
{
“interval”: {
“startTime”: “2020-07-27T20:19:21.597239Z”,
“endTime”: “2020-07-27T20:19:21.597239Z”
},
“value”: {
“doubleValue”: 0.473025
}
},
],
Para entender o significado de um valor, consulte os outros dados incluídos na série temporal e as definições desses dados.

O campo resource descreve o componente de hardware ou software que está sendo monitorado. No Cloud Monitoring, o componente de hardware ou software é chamado de recurso monitorado. Exemplos de recursos monitorados incluem instâncias do Compute Engine e aplicativos do App Engine. Para ver uma lista completa de recursos monitorados, consulte a Lista de recursos monitorados.

No exemplo anterior, o campo resource é o seguinte:

“resource”: {
“type”: “gce_instance”,
“labels”: {
“instance_id”: “2708613220420473591”,
“zone”: “us-east1-b”,
“project_id”: “sampleproject”
}
O campo type lista o recurso monitorado como um gce_instance, que indica que essas medidas são tomadas em uma instância de VM do Compute Engine.

O campo labels contém pares de chave-valor que fornecem informações adicionais sobre o recurso monitorado. Para um tipo gce_instance, os rótulos identificam a instância de VM que está sendo monitorada.

O campo metric descreve o que está sendo medido.

No exemplo anterior, o campo metric é como mostrado:

“metric”: {
“labels”: {
“device”: “sda1”,
“state”: “free”
},
“type”: "agent.googleapis.com/disk/percent_used"
},
Para os serviços do Google, o campo type especifica o serviço e o que está sendo monitorado. Neste exemplo, o agente do Cloud Monitoring é o serviço e está avaliando a porcentagem do disco usado. Quando o campo type começa com custom ou external, a métrica é personalizada ou definida por terceiros.

O campo labels contém pares de chave-valor que fornecem informações adicionais sobre a medição. Esses rótulos são definidos como parte do MetricDescriptor, que é uma estrutura de dados que define os atributos dos dados medidos. O MetricDescriptor da métrica agent.googleapis.com/disk/percent_used inclui os rótulos device e state.

O campo metricKind descreve a relação entre medições adjacentes em uma série temporal:

As métricas GAUGE armazenam o valor da coisa que está sendo medida em um determinado momento, por exemplo, um registro de temperatura por hora.

As métricas CUMULATIVE armazenam o valor acumulado daquilo que está sendo medido em um determinado momento. Por exemplo, um odômetro em um veículo.

As métricas DELTA armazenam a alteração no valor do que está sendo medido durante um período especificado. Por exemplo, um resumo de ações que mostra os ganhos ou as perdas delas.

O campo valueType descreve o tipo de dados da medição: INT64, DOUBLE, BOOL, STRING ou DISTRIBUTION.

O Cloud Monitoring grava uma série temporal para cada combinação de valores de rótulo de métrica e recurso. Você pode usar esses rótulos para agrupar e filtrar séries temporais. Por exemplo, quando um projeto do Google Cloud contém várias instâncias de VM do Compute Engine, a utilização da CPU para cada instância de VM é uma série temporal única. Veja algumas maneiras de exibir esses dados:

É possível mostrar a utilização da CPU de cada instância de VM.
É possível mostrar a utilização da CPU para uma instância de VM específica filtrando a série temporal por um único valor do rótulo instance_id.
É possível agrupar pelas instâncias de VM pelo rótulo machine_type e, em seguida, exibir a utilização média da CPU. A captura de tela a seguir ilustra um gráfico com esta configuração:

Utilização média da CPU agrupada por tipo de máquina.

A seguir
Para explorar o Cloud Monitoring, consulte o Guia de início rápido para monitorar uma instância do Compute Engine.

Para informações sobre como configurar o projeto do Google Cloud para visualizar métricas de vários projetos e contas da AWS, consulte Visão geral dos escopos das métricas.

Para mais informações sobre a API Cloud Monitoring, consulte APIs e referência.

Para listas de métricas e recursos monitorados, consulte Lista de métricas e Lista de recursos monitorados.

Para informações sobre preços, cotas e limites, consulte Recursos.)
4 (All together now: our operations products in one place
February 24, 2020
Raghu Nandan
PM Director of Operations Management

Our suite of operations products has come a long way since the acquisition of Stackdriver back in 2014. The suite has constantly evolved with significant new capabilities since then, and today we reach another important milestone with complete integration into the Google Cloud Console. We’re now saying goodbye to the Stackdriver brand, and announcing an operations suite of products, which includes Cloud Logging, Cloud Monitoring, Cloud Trace, Cloud Debugger, and Cloud Profiler.

The Stackdriver functionality you’ve come to depend on isn’t changing. Over the years, these operations products have seen a strong growth in usage by not just application developers and DevOps teams, but also IT operators and security teams. Complete integration of the products into the Cloud Console, along with in-context presence within the key service pages themselves—like the integrations into Compute Engine, Google Kubernetes Engine, Cloud SQL, and Dataflow management consoles—brings a great experience to all users. Putting operations tasks a quick click away, without users losing context of the activities they had been performing, shows how seamless an operations journey can be.

In addition to this console integration, we’re very happy to share some of the progress in our products, with lots of exciting features launching today.

Cloud Logging

Continuing with our goal to build easy-to-use products, we have completely overhauled the Logs Viewer and will be rolling this out to everyone over the next week. This makes it even easier for you to quickly identify and troubleshoot issues. We’re also pleased to announce that the ability to customize how long logs are retained is now available in beta. With both the new Cloud Logging user interface and the new 10-year log retention feature, you can search logs quickly and identify trends and correlations. We also understand that in some cases, it is very useful to export logs from Cloud Logging to other locations like BigQuery, Cloud Storage, or even third-party log management systems. To make this easier, we are making Logs Router generally available. Similarly, data from Cloud Trace can also be exported to BigQuery. Log Router’s support for customer management encryption keys (CMEK) also makes this a good solution for environments needing to meet that security need for compliance and other purposes.

Cloud Monitoring

Our biggest change of all that you’ll see in the console is Cloud Monitoring, as this was the last Stackdriver product to migrate over to our Google Cloud Console. You’ll now find a better designed, easy-to-navigate site, and important new features targeted to make your life easier. We are increasing our metrics retention to 24 months and writing metrics at up to 10-second granularity. The increased granularity is especially useful when making quick operational decisions like load balancing, scaling, etc. Like Cloud Logging, you can now access what you need more quickly, as well as prepare for future troubleshooting with longer retention.

An additional key launch is Dashboards API, which lets you develop a dashboard once and share it multiple times in other workspaces and environments. Users might also notice better metrics recommendations by surfacing to the top of the selection list the most popular metrics for a given resource type. This is a great example of understanding the preferred metric by the millions of users on Google Cloud, and surfacing them quickly in other situations.

This release makes it possible to route alerts to independent systems with Pub/Sub support, continuing with the ability to connect a broad variety of operational tools with Cloud Monitoring. To keep up with the needs of some of our largest users, we are also expanding support for hundreds of projects within a Workspace—providing a single point of control and management interface for multiple projects. Stay tuned for more details about all of these new capabilities in a series of blog posts over the next few weeks.

2020 will continue to see momentum for our operations suite of products, and we’re looking forward to the road ahead as we continue to help developers and operators across the world to manage and troubleshoot issues quickly and keep their systems up and running.

Learn more about the operations suite here.

Posted in
Management Tools
Google Cloud
Cloud Operations
Related articles)
5 (Preços do pacote de operações do Google Cloud
O preço do pacote de operações do Google Cloud permite que você controle o uso e os gastos. Os produtos do pacote de operações do Google Cloud são cobrados por volume de dados ou uso. Você pode usar as cotas de uso de dados gratuito para começar sem taxas ou compromissos iniciais.

As tabelas a seguir resumem as informações de preços do Cloud Logging, do Cloud Monitoring e do Cloud Trace:

Resumo dos preços do Cloud Logging
Recurso Preço1 Cota gratuita por mês
Armazenamento do Logging* US$ 0, 50/GiB;
Cobrança única por streaming de registros para armazenamento de bucket de registros para indexação, consulta e análise.Inclui até 30 dias de armazenamento em buckets de registro. Não há cobranças adicionais para consultar e analisar dados de registros. Primeiros 50 GiB/projeto/mês
Retenção do Logging† US$ 0,01 por GiB por mês para registros retidos por mais de 30 dias; faturamento mensal de acordo com a retenção. Os registros retidos para o período de retenção padrão não geram custo de retenção.
Entrada Logging‡ Sem custo extra Não relevante
Roteador de registrosCheck Sem custo extra Não relevante
Análise de registros♣ Sem custo extra Não relevante

O volume de armazenamento conta o tamanho real das entradas de registro antes da indexação. Não há cobranças de armazenamento para registros armazenados no bucket _Required.
† Não há cobranças de retenção para registros armazenados no bucket de registros _Required, que tem um período de armazenamento fixo de 400 dias.
‡ O Ingress é definido como os registros recebidos pela API Cloud Logging.
Check O roteamento de registros é definido como encaminhar registros recebidos para um destino compatível. Cobranças de destino podem ser aplicadas aos registros roteados.
♣ Não há cobrança para fazer upgrade de um bucket de registros para usar a análise de registro ou para emitir consultas SQL na página Análise de registros.
Observação: o idioma dos preços do Cloud Logging mudou em 19 de julho de 2023. No entanto, as cotas gratuitas e as taxas não mudaram. Sua fatura pode se referir à linguagem de preços antiga.
Resumo dos preços do Cloud Monitoring
Recurso Preço Cota gratuita por mês Início da vigência
Todos os dados do Monitoring
, exceto os dados ingeridos usando o Managed Service para Prometheus US$ 0,2580/MiB1: primeiros 150–100.000 MiB
US$ 0,1510/MiB: próximos 100.000–250.000 MiB
US$ 0,0610/MiB : mais de 250.000 MiB Todas as métricas não faturáveis do Google Cloud
Primeiros 150 MiB por conta de faturamento para métricas cobradas por bytes ingeridos 1º de julho de 2018
Métricas ingeridas usando o Google Cloud Managed Service para Prometheus, incluindo métricas do plano de controle do GKE US$ 0,15/milhão de amostras†: primeiras 0 a 50 bilhões de amostras ingeridas#
US$ 0,12/milhão de amostras: próximas 50 a 250 bilhões de amostras ingeridas
US$ 0,09/milhão de amostras: próximas 250-500 bilhões de amostras ingeridas
US$ 0,06/milhões de amostras: >500 bilhões de amostras ingeridas Não relevante 16 de maio de 2022
Como monitorar dados ingeridos usando métricas de carga de trabalho do GKE As métricas de carga de trabalho do GKE estão obsoletas e foram removidas no GKE 1.24. Durante o período de suspensão de uso, a ingestão de métricas de carga de trabalho do GKE não será cobrada. Não relevante Não relevante
Chamadas da API Monitoring US$ 0,01/1.000 chamadas de API de leitura
(as chamadas de gravação são gratuitas) Primeiro milhão de chamadas de API de leitura incluídas por conta de faturamento 1º de julho de 2018
Execução de monitoramento de verificações de tempo de atividade USD 0,30/1.000 execuções‡ 1 milhão de execuções por projeto do Google Cloud 1º de outubro de 2022
Execução de monitores sintéticos de monitoramento USD 1,20/1.000 execuções* 100 execuções por conta de faturamento 1o de novembro de 2023
† O Google Cloud Managed Service para Prometheus usa o armazenamento do Cloud Monitoring para dados de métricas criados externamente e usa a API Monitoring para recuperar esses dados. O serviço gerenciado para o Prometheus mede com base em amostras ingeridas em vez de bytes, de acordo com as convenções do Prometheus. Para mais informações sobre a medição baseada em amostra, consulte Preços para controle e previsibilidade. Para exemplos computacionais, consulte Exemplos de preços com base em amostras ingeridas.

As amostras são contabilizadas por conta de faturamento.
‡ As execuções são cobradas na conta de faturamento em que são definidas. Para mais informações, consulte Preços para execução da verificação de tempo de atividade.

As execuções são cobradas na conta de faturamento em que estão definidas. Para cada execução, é possível receber cobranças extras de outros serviços do Google Cloud, incluindo serviços como Cloud Functions, Cloud Storage e Cloud Logging. Para informações sobre essas cobranças extras, consulte o documento de preços do respectivo serviço do Google Cloud.
Resumo dos preços do Cloud Trace
Recurso Preço Cota gratuita por mês Início da vigência
Ingestão do Trace US$ 0,20/milhão de períodos Primeiros 2,5 milhões de períodos 1º de novembro de 2018
Para informações detalhadas sobre os custos dos produtos do pacote de operações do Google Cloud, consulte as seguintes seções desta página:
Cloud Logging
Cloud Monitoring
Error Reporting
Cloud Profiler
Cloud Trace
Para mais informações sobre preços, consulte a página do Anthos.

Como visualizar o uso
Para ver seu uso atual, acesse a página Relatórios do Cloud Billing do Console do Google Cloud.

ACESSAR O CLOUD BILLING

Com base nos dados de uso atuais, é possível fazer uma estimativa das faturas usando a calculadora de preços.

Por exemplo, uma configuração em que toda instância de VM do Compute Engine gera 10 GiB de registros sujeitos a cobrança e 20 MiB de métricas sujeitas a cobrança por mês. Ao usar a calculadora de preços, você determina o custo estimado do Cloud Monitoring e do Cloud Logging:

1 VM 10 VMs 100 VMs 1.000 VMs
Custo de métricas por mês US$ 0,00 US$ 12,90 US$ 477,30 US$ 5.121,30
Custo da geração de registros por mês US$ 0,00 US$ 25,00 US$ 475,00 US$ 4.975,00
Custo total: US$ 0,00 US$ 37,90 US$ 952,30 US$ 10.096,30
Como configurar um alerta de faturamento
Para receber notificações se as cobranças faturáveis ou previstas excederem um orçamento, crie um alerta na página Orçamentos e alertas do Console do Google Cloud:

Faça login no Console do Google Cloud:
FAÇA LOGIN NO CONSOLE DO GOOGLE CLOUD
Abra o menu de navegação menu do Console e selecione Faturamento. Se você tiver mais de uma conta do Cloud Billing, siga uma das orientações a seguir:
Para gerenciar o Cloud Billing no projeto atual, selecione Acessar a conta de faturamento vinculada.
Para localizar outra conta do Cloud Billing, selecione Gerenciar contas de faturamento e escolha a opção em que você quer definir um orçamento.
No menu de navegação de faturamento, selecione Orçamentos e alertas.
Clique em add_box Criar orçamento.
Preencha a caixa de diálogo do orçamento. Nesse campo, selecione projetos e produtos do Google Cloud e depois crie um orçamento para a combinação. Por padrão, você recebe notificações ao atingir 50%, 90% e 100% do orçamento. Para ver a documentação completa, consulte Definir orçamentos e alertas.
Observação:na caixa de diálogo de faturamento, use as seguintes configurações:
Para criar um alerta sobre o uso do Cloud Logging, selecione Cloud Logging
Para criar um alerta sobre o uso do Cloud Monitoring, selecione Stackdriver Monitoring
Para criar um alerta sobre o uso do Cloud Trace, selecione Stackdriver Trace
Cloud Logging
buckets de registro são os contêineres do Logging que armazenam dados de registros. O Logging cobra pelo volume de dados de registro armazenado no bucket de registros _Default e nos buckets de registro definidos pelo usuário, quando esse volume excede a cota mensal gratuita. Para o bucket de registros _Default e buckets de registros definidos pelo usuário, o Logging também cobra quando os registros são retidos por mais do que o período de armazenamento padrão, que é de 30 dias.

Não há cobranças extras pelo Logging para rotear registros, para usar a API Cloud Logging ou para registros armazenados no bucket de registros _Required, que tem um período de armazenamento fixo de 400 dias.

Esta seção fornece informações sobre os seguintes tópicos:

Modelo de armazenamento do Cloud Logging
Preços de armazenamento
Preços de retenção
Reduzir o armazenamento de registros
Preços de métricas com base em registros
Criar política de alertas em bytes de registro ingeridos mensalmente
Para um resumo das informações de preços, consulte Resumo dos preços do Cloud Logging.

Para saber os limites que se aplicam ao seu uso do Logging, incluindo períodos de armazenamento de dados, consulte Cotas e limites.

Para ver e entender seus dados de uso do Cloud Logging, consulte Como estimar suas faturas.

Modelo de armazenamento do Cloud Logging
Para cada projeto do Google Cloud, o Logging cria automaticamente dois buckets de registros: _Required e _Default. Para esses dois buckets, o Logging cria automaticamente coletores de registro denominados _Required e _Default, que encaminham registros para os buckets nomeados de maneira correspondente. Não é possível desativar ou modificar o coletor _Required. É possível desativar ou modificar o coletor _Default para evitar que o bucket _Default armazene novos registros.

É possível criar buckets de registros definidos pelo usuário em qualquer um dos projetos do Google Cloud. Também é possível configurar coletores para rotear qualquer combinação de registros, mesmo entre projetos do Google Cloud na organização do Google Cloud, para esses buckets de registros.

Para o bucket de registros _Default e buckets de registros definidos pelo usuário, é possível configurar um período de armazenamento personalizado.

É possível fazer upgrade dos buckets de registro para usar o Log Analytics. Não há cobrança para fazer upgrade de um bucket de registros para usar a Análise de registros.

Para mais informações sobre buckets e coletores do Cloud Logging, consulte Visão geral de roteamento e armazenamento.

Preços de armazenamento
O Logging não cobra por registros armazenados no bucket _Required. Não é possível excluir o bucket _Required ou modificar o coletor _Required. O bucket _Required armazena os seguintes registros:

Registros de auditoria de atividade do administrador
Registros de auditoria de eventos do sistema
Registros de auditoria do administrador do Google Workspace
Registros de auditoria do Grupos do Google Enterprise
Registros de auditoria de login
Registros de transparência no acesso No entanto, ativar a transparência no acesso requer determinados níveis de suporte do Google Cloud. Veja a documentação de registros da transparência no acesso para mais informações.
Observação: se você rotear cópias de registros armazenados automaticamente no bucket _Required para outro bucket de registros, os preços de armazenamento e armazenamento serão aplicados.
O Logging cobra pelo volume pré-indexado de dados de registros armazenado no bucket de registros _Default e nos buckets de registro definidos pelo usuário, quando o volume total excede a cota mensal gratuita. Cada gravação de uma entrada de registro no bucket de registros _Default ou em um bucket de registros definido pelo usuário é computada em sua cota de armazenamento. Por exemplo, se você tiver coletores que encaminham uma entrada de registro para três buckets de registros, ela será armazenada três vezes.

Preços de retenção
Observação : a partir de 1o de abril de 2023, os custos de retenção se aplicam a dados de registros retidos por mais tempo do que o período de armazenamento padrão do bucket de registros. Para detalhes sobre preços, consulte Resumo dos preços do Cloud Logging. Para revisar o armazenamento faturável para seus buckets de registro, acesse a página Armazenamento de registros do Console do Google Cloud.
A tabela a seguir lista os períodos de armazenamento de dados para registros armazenados em buckets:

Bucket de registros Período de armazenamento padrão Armazenamento personalizado
_Required 400 dias Não configurável
_Default 30 dias Configurável
Definido pelo usuário 30 dias Configurável
O Logging cobra custos de retenção quando os registros são retidos por mais tempo do que o período de armazenamento padrão. Não é possível configurar o período de armazenamento do bucket de registros _Required. Não há custos de armazenamento quando os registros são armazenados apenas para o período de armazenamento padrão do bucket de registros.

Se você diminuir o período de armazenamento de um bucket de registros, haverá um período de carência de sete dias em que os registros expirados não serão excluídos. Não é possível consultar ou visualizar registros expirados. No entanto, nesses sete dias, é possível restaurar o acesso total estendendo o período de armazenamento do bucket de registros. Os registros armazenados durante o período de carência são contabilizados nos custos de retenção.

Se você rotear uma entrada de registro para vários buckets de registros, os custos de armazenamento e retenção podem ser cobrados várias vezes. Por exemplo, suponha que você encaminhe uma entrada de registro para o bucket de registros _Default e para um definido pelo usuário. Além disso, suponha que você configure um período de armazenamento personalizado para os dois buckets com mais de 30 dias. Para essa configuração, você recebe duas cobranças de armazenamento e duas cobranças de retenção.

Reduzir o armazenamento de registros
O Logging permite identificar e excluir manualmente entradas de registro de serem armazenadas em buckets de registro ao configurar filtros de exclusão nos coletores. Ao usar filtros de exclusão, é possível reduzir os custos de armazenamento. Como alternativa, considere também se é necessário rotear seus registros para fora do Cloud Logging.

Os filtros de exclusão podem remover todas as entradas de registro que correspondem ao filtro ou apenas uma porcentagem dos registros que correspondem ao filtro. Quando uma entrada de registro corresponde a um filtro de exclusão de um coletor, esse coletor não encaminha a entrada de registro para o destino. Como resultado, o destino não ingere a entrada de registro. As entradas de registro excluídas não são descontadas da cota de armazenamento. Para instruções sobre como definir filtros de exclusão, consulte Exclusões de registros.

Para manter o acesso a registros que não estão armazenados em buckets de registros, também é possível usar coletores de registros para rotear entradas de registro do Cloud Logging para um destino compatível. O Cloud Logging não cobra por registros de rota. No entanto, os serviços do Google Cloud que recebem seus registros cobram pelo uso. Para mais informações, consulte estes documentos:

Preços do Cloud Storage
Preços do BigQuery
Preços do Pub/Sub
Para informações sobre como rotear registros para fora do Cloud Logging, consulte Rotear registros para destinos compatíveis.

Preços de métricas com base em registros
As métricas com base em registros definidas pelo sistema são fornecidas para todos os projetos do Google Cloud e não estão sujeitas a cobranças.

As métricas com base em registros definidas pelo usuário são uma classe de métricas personalizadas do Cloud Monitoring e são faturáveis. Para ver detalhes de preços, consulte Métricas faturáveis.

Para mais informações, consulte Visão geral das métricas com base em registros.

Criar política de alertas em bytes de registro ingeridos mensalmente
Para criar uma política de alertas acionada quando o número de bytes de registro gravados nos buckets exceder o limite definido pelo usuário do Cloud Logging, use as configurações a seguir.

Etapas para criar uma política de alertas
Novo estado
Campo
Valor
Recurso e métrica No menu Recursos, selecione Global.
No menu Categorias de métrica, selecione Métrica com base em registros.
No menu Métricas, selecione Bytes de registro mensais ingeridos.
Filtrar Nenhuma.
Várias séries
Agregação de série temporal sum
Janela contínua 60 m
Função de janela contínua max
Campo
Configurar gatilho de alerta
Valor
Tipo de condição Threshold
Acionador de alerta Any time series violates
Posição do limite Above threshold
Valor do limite Você determina o valor aceitável.
Teste a janela novamente O valor mínimo aceitável é de 30 minutos.
Cloud Monitoring
O Monitoring cobra pelos seguintes itens:

Métricas medidas por bytes ingeridos, quando os dados de métricas ingeridos excedem a cota de métricas mensal gratuita.

Métricas não sujeitas a cobrança não contam para o limite de cota.

Métricas medidas pelo número de amostras ingeridas.

Chamadas de leitura da API Cloud Monitoring que excedem a cota de API mensal gratuita.

As chamadas de gravação da API Monitoring não são contabilizadas no limite de cotas.

Execução de verificações de tempo de atividade

Execução de monitores sintéticos.

No Monitoring, ingestão refere-se ao processo de gravação de série temporal no Monitoring. Cada série temporal inclui um número de pontos de dados; esses pontos de dados são a base para as cobranças de processamento. Para informações sobre preços, consulte Preços do Cloud Monitoring.

Nesta seção, você encontra as informações a seguir:

Definições de métricas sujeitas a cobrança e não faturáveis.
Descrições de estratégias de processamento baseadas em byte e amostra.
Exemplos de preços de métricas cobradas por bytes ingeridos.
Exemplos de preços de métricas cobradas por amostras ingeridas.
Exemplos de preços para execução de verificações de tempo de atividade (em vigor a partir de 1o de outubro de 2022).
Exemplos de preços para execução de monitores sintéticos (em vigor a partir de 1o de novembro de 2023).
Para informações sobre os preços atuais, consulte Preços do Cloud Monitoring.

Para saber os limites que se aplicam ao uso do Monitoring, consulte Cotas e limites.

Para ver o uso atual, acesse a página de relatórios do Cloud Billing ou de configurações do Monitoring no Console do Google Cloud.

ACESSAR CONFIGURAÇÕES DO MONITORING

Com base nessas informações, faça uma estimativa das suas faturas.

Métricas não faturáveis
Os dados de métricas do Google Cloud, do Anthos e do Knative não são faturáveis. Estas são as métricas não sujeitas a cobrança (gratuitas):

Métricas do Google Cloud. Para mais informações, consulte a nota de rodapé 2.
Métricas do Anthos. Para mais informações, consulte a nota de rodapé 2.
Métricas do Istio
Métricas do Knative
Métricas do sistema do Google Kubernetes Engine
métricas agent.googleapis.com/agent/
Métricas sujeitas a cobrança
Todos os dados de métricas, exceto os listados na seção Métricas não faturáveis, são faturáveis. A maior parte da ingestão de métricas é cobrada pelo número de bytes, mas algumas são cobradas pelo número de amostras. descritos nas seções a seguir.

Os fatores a seguir contribuem para os custos de ingestão:

O tipo de pontos de dados, valores escalares ou de distribuição, coletados pelas métricas.

Para informações sobre o tipo de dados associado a um tipo de métrica específico, consulte a lista de métricas.
Para informações sobre tipos de dados escalares e de distribuição, consulte Tipos de valor.
O número de pontos de dados gravados em séries temporais. Esse valor depende da frequência com que os dados são amostrados e da cardinalidade dos seus dados. A cardinalidade determina quantas séries temporais são geradas para uma combinação de tipos de recursos monitorados e de métrica. Para mais informações, consulte Cardinalidade.

Os valores dos rótulos de métricas e recursos que fazem parte da série temporal não contribuem para as cobranças.

Métricas cobradas por bytes ingeridos
As métricas a seguir podem ser cobradas e cobradas pelo número de bytes ingeridos:

Métricas do agente em agent.googleapis.com, exceto o grupo agent.googleapis.com/agent/

A partir de 6 de agosto de 2021, as métricas agent.googleapis.com/processes/ serão cobradas a 5% da taxa de volume de outras métricas sujeitas a cobrança. Por exemplo, processar 100 MiB de métricas de processo custará o mesmo que processar 5 MiB de outras métricas sujeitas a cobrança.3

Métricas de integrações de terceiros com agente de operações. Essas métricas são ingeridas no Monitoring com identificadores do formulário workload.googleapis.com/APPLICATION.METRIC. Por exemplo, o tipo de métrica workload.googleapis.com/nginx.requests se enquadra nessa categoria.

Métricas da AWS

Métricas personalizadas

Métricas externas

Métricas com base em registros definidas pelo usuário

Para fins de preços, o volume de ingestão é calculado da seguinte forma:

Para um tipo de dados escalar: 8 bytes para cada ponto de dados gravado em uma série temporal. Métricas de contagem com base em registros definidas pelo usuário se enquadram nessa categoria.
Para um tipo de dados de distribuição: 80 bytes para cada ponto de dados gravado em uma série temporal.
Para informações sobre pontos de dados em séries temporais, consulte Séries temporais: dados de um recurso monitorado.

Métricas cobradas pelas amostras ingeridas
As métricas a seguir podem ser cobradas e cobradas pelo número de amostras ingeridas:

Métricas do Google Cloud Managed Service para Prometheus: métricas prometheus.googleapis.com.
Para fins de preços, a contagem de amostra é calculada da seguinte forma:

Para um tipo de dados escalar: 1 para cada ponto gravado em uma série temporal.
Para um tipo de dados de distribuição: 2 para cada ponto gravado em uma série temporal, mais 1 para cada bucket de histograma com uma contagem diferente de zero.
Para informações sobre pontos de dados em séries temporais, consulte Séries temporais: dados de um recurso monitorado.

Criação de alertas sobre métricas ingeridas
Não é possível criar um alerta com base nas métricas ingeridas mensalmente. No entanto, é possível fazer isso para seus custos com o Cloud Monitoring. Se quiser mais informações, consulte Como configurar um alerta de faturamento.

Exemplos de preços com base em bytes ingeridos
Veja nos exemplos a seguir como ter uma estimativa de custos para a coleta de dados de métricas cobradas por bytes ingeridos. Esses exemplos têm o objetivo de ilustrar os cálculos. Para estimativas mais abrangentes, use a calculadora de preços. Se você acessar essa ferramenta, use o produto de pacote de operações do Google Cloud para inserir dados de métricas, registros e rastreamento.

Este é o cenário básico: você tem alguns recursos monitorados (como Compute Engine, Kubernetes Engine ou App Engine) que gravam dados de algumas métricas a cada mês.

As variáveis em todos os cenários incluem:

O número de recursos
O número de métricas
Se as métricas são do Google Cloud ou não
A taxa em que os dados da métrica são gravados
Os exemplos desta seção mostram os preços do Monitoring desde julho de 2020.

Contexto comum
Nos exemplos de preços a seguir, pressupomos que cada ponto de dados de métrica ingerido é dos tipos duplo, int64 ou bool, que contam como 8 bytes para fins de determinação de preços. Há cerca de 730 horas (365 dias / 12 meses * 24 horas) em um mês, ou 43.800 minutos.

Para uma métrica que grava dados à taxa de 1 ponto de dados/minuto por um mês, considere as seguintes informações:

O total de pontos de dados é 43.800.
O volume total ingerido é:
350.400 bytes (43.800 pontos de dados * 8 bytes)
0,33416748 MiB (350.400 bytes / 1.048.576 bytes/MiB)
Para uma métrica que grava dados à taxa de 1 ponto de dados/hora por um mês, considere as seguintes informações:

O total de pontos de dados é 730.
Volume total ingerido:
5.840 bytes (730 pontos de dados * 8 bytes)
0,005569458 MiB (5.840 bytes / 1.048.576 bytes/MiB)
Examples
Cenário 1: você tem 1.000 recursos e cada um grava 75 métricas. Essas são apenas métricas do Google Cloud, com taxa de gravação de um ponto de dados por minuto.

Ingestão mensal: 25.063 MiB: 0,33416748 MiB para uma métrica * 75.000 (ou seja, 1.000 recursos, 75 métricas)
Custo aproximado por mês: US$ 0,00 (as métricas do Google Cloud são gratuitas)
MiB ingeridos Taxa (US$/MiB) Custo (US$)
Ilimitados 0,00 US$ 0,00
Total 25.063 US$ 0,00
Cenário 2: você tem 1.000 recursos e cada um grava 75 métricas personalizadas. Essas gravações de métricas estão sujeitas a cobranças e têm uma taxa de um ponto de dados por minuto.

Ingestão mensal: 25.063 MiB (mesmo cenário acima)
Custo aproximado por mês: US$ 6.427,55
MiB ingeridos Taxa (US$/MiB) Custo (US$)
150 0,00 US$ 0,00
24.913 0,258 US$ 6.427,55
Total 25.063 US$ 6.427,55
Cenário 3: você tem 1.000 recursos e cada um grava 75 métricas personalizadas. Essas gravações de métricas estão sujeitas a cobranças e têm uma taxa de um ponto de dados por hora.

Ingestão mensal: 418 MiB = 0,005569458 MiB para uma métrica * 75.000
Custo aproximado por mês: US$ 69,14
MiB ingeridos Taxa (US$/MiB) Custo (US$)
150 0,00 US$ 0,00
267 0,258 US$ 69,14
Total 417 US$ 69,14
Cenário 4: você tem um recurso que grava 500.000 métricas. Essas gravações de métricas estão sujeitas a cobranças e têm uma taxa de um ponto de dados por minuto.

Ingestão mensal: 167.084 MiB: 0,33416748 MiB para uma métrica * 500.000
Custo aproximado por mês: US$ 35.890,98
MiB ingeridos Taxa (US$/MiB) Custo (US$)
150 0,00 US$ 0,00
99.850 0,258 US$ 25.761,30
67.084 0,151 US$ 10.129,68
Total 167.084 US$ 35.890,98
Preços para controle e previsibilidade
O preço do serviço gerenciado para o Prometheus foi projetado para ser controlável. Como as cobranças são geradas por amostra, use os seguintes fatores para controlar os custos:

Período de amostragem: alterar o período de extração de métricas de 15 segundos para 60 segundos pode gerar uma economia de 75%, sem sacrificar a cardinalidade. É possível configurar períodos de amostragem por job, por destino ou global.

Filtragem: use a filtragem para reduzir o número de amostras enviadas ao repositório de dados locais do serviço. Para mais informações, consulte Como filtrar métricas exportadas. Use as configurações de remarcação de métricas na sua configuração de extração do Prometheus para descartar métricas no momento da ingestão com base nos correspondentes de rótulo.

Mantenha dados de alta cardinalidade e baixo valor locais. É possível executar o Prometheus padrão com o serviço gerenciado usando as mesmas configurações de paisagem e manter os dados localmente que não vale a pena enviar para o repositório de dados global do serviço.

O preço do serviço gerenciado para o Prometheus foi projetado para ser previsível.

Você não recebe penalizações por ter histogramas esparsos. As amostras são contadas apenas para o primeiro valor diferente de zero e, em seguida, quando o valor do bucketn é maior que o valor no bucketn-1. Por exemplo, um histograma com valores 10 10 13 14 14 14 conta como três amostras, para o primeiro, terceiro e quarto buckets.

Dependendo de quantos histogramas você usa e para que eles são usados, a exclusão de buckets inalterados dos preços geralmente pode fazer com que 20% a 40% menos amostras sejam contadas para fins de faturamento do que o número absoluto de buckets de histograma indicaria.

Ao cobrar por amostra, você não receberá penalizações por contêineres com escalonamento rápido e não escalonados, preemptivos ou temporários, como os criados pelo HPA ou pelo Autopilot do GKE.

Se o serviço gerenciado para Prometheus fosse cobrado por métrica, você pagaria pela cardinalidade de um mês completo de uma só vez, sempre que um novo contêiner fosse acrescentado. Com o preço por amostra, você paga apenas enquanto o contêiner está em execução.

Consultas, incluindo consultas de alerta

As consultas emitidas pelo console do Google Cloud não são cobradas. Todas as outras consultas emitidas pelo usuário, incluindo as consultas emitidas quando as regras de gravação do Prometheus são executadas, são cobradas por meio de chamadas API Cloud Monitoring. Para a taxa atual, consulte a tabela de resumo dos preços do Serviço gerenciado para o Prometheus ou do Monitoring.

Exemplos de preços com base em amostras ingeridas
Veja nos exemplos a seguir como estimar os custos para coletar métricas cobradas pelas amostras ingeridas. A cobrança baseada em amostra é usada para o Google Cloud Managed Service para Prometheus.

Esses exemplos têm o objetivo de ilustrar técnicas de cálculo, não de fornecer dados de faturamento.

O cenário básico é o seguinte: você tem algum número de contêineres ou pods que estão gravando pontos em algum número de séries temporais por mês. Os dados podem consistir em valores escalares ou distribuições.

As variáveis em todos os cenários incluem:

O número de contêineres ou pods.
O número de séries temporais.
Se os dados consistem em valores escalares, distribuições ou ambos.
A taxa em que os dados são gravados.
Contagem de amostras
Antes de estimar os preços, é preciso saber como contar amostras. O número de amostras contadas para um valor depende do seguinte:

Se o valor é uma escalar ou uma distribuição
A taxa em que os valores são gravados
Nesta seção, você verá como estimar o número de amostras gravadas para uma série temporal durante o período de faturamento mensal.

Em um mês, há cerca de 730 horas (365 dias / 12 meses * 24 horas), 43.800 minutos ou 2.628.000 segundos.

Se uma série temporal gravar valores escalares, cada valor será contabilizado como uma amostra. O número de amostras gravadas em um mês depende apenas da frequência em que os valores são gravados. Veja estes exemplos:

Para valores gravados a cada 15 segundos:
Taxa de gravação: 1 valor/15s = 1 amostra/15s
Amostras por mês: 175.200 (1 amostra/15s * 2.628.000 segundos/mês)
Para valores gravados a cada 60 segundos:
Taxa de gravação: 1 valor/60s = 1 amostra/60s
Amostras por mês: 43.800 (1 amostra/60s * 2.628.000 segundos/mês)
Se uma série temporal gravar valores de distribuição, cada valor poderá conter 2 + n amostras, em que n é o número de buckets no histograma. O número de amostras gravadas em um mês depende do número de buckets nos histogramas e da frequência com que os valores são gravados.

Por exemplo, cada instância de um histograma de 50 intervalos pode conter 52 amostras. Se os valores forem gravados uma vez a cada 60 segundos, um histograma de 50 buckets gravará no máximo 2.277.600 amostras por mês. Se o histograma tiver 100 buckets e for gravado uma vez a cada 60 segundos, cada histograma poderá conter 102 amostras e gravar no máximo 4.467.600 amostras por mês.

A maioria das séries temporais de distribuição contém menos do que o número máximo de amostras. Na prática, entre 20% e 40% dos buckets de histograma estão vazios. Essa porcentagem é ainda maior para usuários com histogramas esparsos, como os gerados pelo Istio.

Ao contar amostras de preços, somente buckets com valores não vazios são incluídos. O número máximo de amostras por histograma é 2 + n. Se 25% dos buckets estiverem vazios, o número esperado de amostras será 2 + 0,75 n por histograma. Se 40% dos buckets estiverem vazios, o número esperado de amostras será de 2 + 0,60n por histograma.

Os seguintes cálculos e a tabela de resumo mostram o número máximo de amostras e os números mais realistas de amostras esperadas:

Para valores de histograma de 50 intervalos gravados a cada 15 segundos:

Taxa de gravação: 1 valor/15 s
Máximo de amostras:
Por histograma: 52
Por mês: 9.110.400 (52 * 1 valor/15s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 25% estejam vazias:
Por histograma: 39,5 (2 + 0,75(50) ou 2 + (50 - 12,5))
Por mês: 6.920.400 (39,5 * 1 valor/15s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 40% estejam vazias:
Por histograma: 32 (2 + 0,6(50) ou 2 + (50 - 20))
Por mês: 5.606.400 (32 * 1 valor/15s * 2.628.000 segundos/mês)
Para valores de histograma de 50 intervalos gravados a cada 60 segundos:

Taxa de gravação: 1 valor/60 s
Máximo de amostras:
Por histograma: 52
Por mês: 2.277.600 (52 * 1 valor/60s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 25% estejam vazias:
Por histograma: 39,5 (2 + 0,75(50) ou 2 + (50 - 12,5))
Por mês: 1.730.100 (39,5 * 1 valor/60s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 40% estejam vazias:
Por histograma: 32 (2 + 0,6(50) ou 2 + (50 - 20))
Por mês: 1.401.600 (32 * 1 valor/60s * 2.628.000 segundos/mês)
Para valores de histograma de 100 intervalos gravados a cada 15 segundos:

Taxa de gravação: 1 valor/15 s
Máximo de amostras:
Por histograma: 102
Por mês: 17.870.400 (102 * 1 valor/15s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 25% estejam vazias:
Por histograma: 77 (2 + 0,75(100) ou 2 + (100 - 25))
Por mês: 13.490.400 (77 * 1 valor/15s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 40% estejam vazias:
Por histograma: 62 (2 + 0,6(100) ou 2 + (100 - 40))
Por mês: 10.862.400 (62 * 1 valor/15s * 2.628.000 segundos/mês)
Para valores de histograma de 100 intervalos gravados a cada 60 segundos:

Taxa de gravação: 1 valor/60 s
Máximo de amostras:
Por histograma: 102
Por mês: 4.467.600 (102 * 1 valor/60s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 25% estejam vazias:
Por histograma: 77 (2 + 0,75(100) ou 2 + (100 - 25))
Por mês: 3.372.600 (77 * 1 valor/60 s * 2.628.000 segundos/mês)
Amostras esperadas, supondo que 40% estejam vazias:
Por histograma: 62 (2 + 0,6(100) ou 2 + (100 - 40))
Por mês: 2.715.600 (62 * 1 valor/60s * 2.628.000 segundos/mês)
A seguinte tabela resume as informações anteriores:

Contagem em lote Taxa de gravação Amostras por mês
(máx.) Amostras por mês
(25% vazias) Amostras por mês
(40% vazias)
50 1 amostra/15s 9.110.400 6.920.400 5.606.400
50 1 amostra/60s 2.277.600 1.730.100 1.401.600
100 1 amostra/15s 17.870.400 13.490.400 10.862.400
100 1 amostra/60s 4.467.600 3.372.600 2.715.600
Examples
Para estimar os preços, conte o número de amostras gravadas durante um mês e aplique os valores. Os preços das amostras são definidos por milhão, para intervalos empilhados, da seguinte maneira:

Intervalo de ingestão Serviço gerenciado para o Prometheus Máximo para o intervalo
Até 50 bilhões (50.000 milhões) US$ 0,15/milhões US$ 7.500,00
50 bilhões a 250 bilhões (250.000 milhões) US$ 0,12/milhões US$ 24.000,00
250 bilhões a 500 bilhões (500.000 milhões) US$ 0,09/milhões US$ 22.500,00
Mais de 500 bilhões (500.000 milhões) US$ 0,06/milhão
O restante desta seção apresenta possíveis cenários.

Cenário 1: você tem 100 contêineres, cada um gravando uma série de mil séries temporais escalares.

Variante A: se cada série temporal for gravada a cada 15 segundos (1 amostra/15s), o número de amostras gravadas por mês será de 17.520.000.000 (175.200 amostras/mês * 1.000 séries temporais * 100 contêineres) ou 17,520 milhões de contêineres.

Variante B: se cada série temporal for gravada a cada 60 segundos (1 amostra/60s), o número de amostras gravadas por mês será de 4.380.000.000 (43.800 amostras/mês * 1.000 séries temporais * 100 contêineres), ou 4.380 milhões.

Em ambos os casos, há menos de 50.000 milhões de amostras,portanto, somente a primeira taxa se aplica. Nenhuma amostra é cobrada com as outras taxas.

Variante Amostras ingeridas Intervalo de ingestão Serviço gerenciado para o Prometheus
(US$ 0,15, US$ 0,12, US$ 0,09 e US$ 0,06)
A (1 amostra/15s)

Total 17.520 milhões

17.520 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 2.628,00

US$2.628,00
B (1 amostra/60 segundos)

Total 4.380 milhões

4.380 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 657,00

US$657,00
Cenário 2: você tem 1.000 contêineres, cada um gravando 1.000 séries temporais escalares.

Variante A: se cada série temporal for gravada a cada 15 segundos (1 amostra/15s), o número de amostras gravadas por mês será de 175.200.000.000, ou 175.200 milhões:

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As 125.200 milhões de amostras restantes são cobradas de acordo com a segunda taxa.
Não há amostras cobradas nas outras taxas.
Variante B: se cada série temporal for gravada a cada 60 segundos (1 amostra/60s), o número de amostras gravadas por mês será de 43.800.000.000, ou 43.800 milhões. Esse valor mensal é menor que 50.000 milhões de amostras. Portanto, apenas a primeira taxa se aplica.

Variante Amostras ingeridas Intervalo de ingestão Serviço gerenciado para o Prometheus
(US$ 0,15, US$ 0,12, US$ 0,09 e US$ 0,06)
A (1 amostra/15s)

Total 50.000 milhões
125.200 milhões

175.200 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 15.024,00

US$22.524,00
B (1 amostra/60 segundos)

Total 43.800 milhões

43.800 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 6.570,00

US$6.570,00
Cenário 3: você tem 100 contêineres, cada um gravando uma série temporal de distribuição de 1.000 buckets de 100 buckets. Você espera que 25% dos buckets estejam vazios.

Variante A: se cada série temporal for gravada a cada 15 segundos (1 amostra/15s), o número de amostras gravadas por mês será de 1.349.040.000.000 (13.490.400 amostras/mês * 1.000 séries temporais * 100 contêineres) ou 1.349.040 milhões de contêineres.

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As próximas 200.000 milhões de amostras são cobradas a partir da segunda taxa.
Os próximos 250.000 milhões de amostras são cobrados na terceira taxa.
Os 749.040 milhões de amostras restantes são cobrados com a quarta taxa.
Variante B: se cada série temporal for gravada a cada 60 segundos (1 amostra/60s), o número de amostras escritas por mês será de 337.260.000.000 (3.372.600 amostras/mês * 1.000 séries temporais * 100 contêineres) ou 337.260 milhões,

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As próximas 200.000 milhões de amostras são cobradas a partir da segunda taxa.
As 87.260 milhões de amostras restantes são cobradas pela terceira taxa.
Variante Amostras ingeridas Intervalo de ingestão Serviço gerenciado para o Prometheus
(US$ 0,15, US$ 0,12, US$ 0,09 e US$ 0,06)
A (1 amostra/15s)

Total 50.000 milhões
200.000.000.
250.000.000.
749.040.000.
1.349.040 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 24.000,00
US$ 22.500,00
US$ 44.942,40
US$98.942,40
B (1 amostra/60 segundos)

Total 50.000 milhões
200.000.000
87.260.00

337.260.000.000 Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 24.000,00
US$ 7.853,40

US$39.353,40
Cenário 4: você tem 1.000 contêineres, cada um gravando uma série temporal de distribuição de 10.000 buckets de 100 buckets. Você espera que 40% dos buckets estejam vazios.

Variante A: se cada série temporal for gravada a cada 15 segundos (1 amostra/15s), o número de amostras gravadas por mês será de 108.624.000.000.000 (10.862.400 amostras/mês). * 10.000 séries temporais * 1.000 contêineres, ou 108.624.000 milhões.

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As próximas 200.000 milhões de amostras são cobradas a partir da segunda taxa.
Os próximos 250.000 milhões de amostras são cobrados na terceira taxa.
Os 108.124.000 exemplos restantes são cobrados à quarta taxa.
Variante B: se cada série temporal for gravada a cada 60 segundos (1 amostra/60s), o número de amostras gravadas por mês será de 27.156.000.000.000 (2.715.600 amostras/mês * 10.000 séries temporais * 1.000 contêineres), ou 27.156.000 milhões.

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As próximas 200.000 milhões de amostras são cobradas a partir da segunda taxa.
Os próximos 250.000 milhões de amostras são cobrados na terceira taxa.
Os 26.656.000 exemplos restantes são cobrados na quarta taxa.
Variante Amostras ingeridas Intervalo de ingestão Serviço gerenciado para o Prometheus
(US$ 0,15, US$ 0,12, US$ 0,09 e US$ 0,06)
A (1 amostra/15s)

Total 50.000.000
200.000.000
250.000.000
108.124.000 milhões
108.624.000 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 24.000,00
US$ 22.500,00
US$ 6.487.440,00
US$6.541.440,00
B (1 amostra/60 segundos)

Total 50.000.000
200.000.000
250.000.000
26.656.000 milhões
27.156.000.000.000 Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 24.000,00
US$ 22.500,00
US$ 1.599.360,00
US$1.653.360,00
Cenário 5: você tem o seguinte:

1.000 contêineres, cada um com 1.000 séries temporais escalares a cada 15 segundos. O número de amostras escritas por mês é 175.200.000.000 ou 175.200 milhões. (Cenário 2, variante A)

1.000 contêineres, cada um gravando 10.000 séries temporais de distribuição de 100 intervalos a cada 15 segundos. Você espera que 40% dos buckets estejam vazios. O número de amostras escritas por mês é 108.624.000.000.000 ou 108.624.000 milhões. (Cenário 4, variante A)

O número total de amostras por mês é de 108.799.200 milhões (175.200 milhões + 108.624.000 milhões).

Os primeiros 50.000 milhões de amostras são cobrados de acordo com a primeira taxa.
As próximas 200.000 milhões de amostras são cobradas a partir da segunda taxa.
Os próximos 250.000 milhões de amostras são cobrados na terceira taxa.
As 108.299.200 milhões de amostras restantes são cobradas de acordo com a quarta taxa.
Variante Amostras ingeridas Intervalo de ingestão Serviço gerenciado para o Prometheus
(US$ 0,15, US$ 0,12, US$ 0,09 e US$ 0,06)
2A + 4A

Total 50.000.000
200.000.000
250.000.000
108.299.200 milhões
108.799.200 milhões Até 50.000 milhões
Até 250.000.000
Até 500.000 milhões
Mais de 500.000 milhões US$ 7.500,00
US$ 24.000,00
US$ 22.500,00
US$ 6.497.952,00
US$6.551.952,00
Preços para execução da verificação de tempo de atividade (início da vigência: 1o de outubro de 2022)
Monitoramento de cobranças para cada execução regional de uma verificação de tempo de atividade, além da cota mensal gratuita de 1 milhão de execuções. Uma verificação executada em três regiões conta como três execuções.

O custo para a execução da verificação de tempo de atividade é de US $0,30/1.000 execuções. A cobrança aparece na sua fatura como SKU “CA14-D3DE-E67F” para “Monitoramento das verificações de tempo de atividade”.

Os exemplos a seguir ilustram como estimar os custos para executar verificações de tempo de atividade. O objetivo desses exemplos é ilustrar técnicas de cálculo, e não fornecer dados de faturamento.

Como contar execuções de verificações de tempo de atividade
Para estimar o custo das verificações de tempo de atividade, é preciso saber quantas execuções regionais ocorrem em um mês. O Monitoring cobra US$ 0,30/1.000 execuções, com uma cota mensal gratuita de 1 milhão de execuções.

Para estimar o custo das verificações de tempo de atividade, use o seguinte cálculo:

(EXECUTIONS_PER_MONTH - 1,000,000) * .0003
Para cada verificação de tempo de atividade, o número de execuções depende das seguintes opções de configuração:

A frequência com que a verificação de tempo de atividade é executada: a cada minuto, 5 minutos, 10 minutos ou 15 minutos.

O número de regiões em que a verificação de tempo de atividade é executada.

O número de segmentações para as quais a verificação de tempo de atividade está configurada. Se a verificação de tempo de atividade estiver configurada para uma única VM, o número de metas será 1. Se a verificação de tempo de atividade estiver configurada para um grupo de recursos, o número de destinos será o número de recursos no grupo.

Ao configurar uma verificação de tempo de atividade, você especifica um local para a verificação de tempo de atividade, e cada local é mapeado para uma ou mais regiões. A tabela a seguir mostra os locais válidos para verificações de tempo de atividade e as regiões para as quais eles são mapeados:

Local da configuração da verificação de tempo de atividade Inclui regiões do Google Cloud
ASIA_PACIFIC asia-southeast1
EUROPE europe-west1
SOUTH_AMERICA southamerica-east1
USA us-central1, us-east4, us-west1
GLOBAL Todas as regiões incluídas por outros locais
É necessário configurar as verificações de tempo de atividade para serem executadas em pelo menos três regiões.

Para estimar o número de execuções de uma verificação de tempo de atividade, você precisa saber quantas regiões são cobertas pelo local dela:

ASIA_PACIFIC, EUROPE e SOUTH_AMERICA incluem uma região.
USA inclui três regiões.
GLOBAL inclui seis regiões.
Em um mês, há cerca de 730 horas (365 dias / 12 meses * 24 horas) ou 43.800 minutos.

Uma verificação de tempo de atividade configurada para ser executada uma vez por minuto em USA é executada em três regiões. Se essa verificação de tempo de atividade estiver configurada para verificar uma única VM, ela executará 131.400 (3 * 43.800) vezes em um mês. Se a verificação estiver configurada para verificar um grupo de recursos de 10 membros, a verificação de tempo de atividade será executada 1.314.000 (10 * 131.400) vezes em um mês.

Uma verificação de tempo de atividade configurada para ser executada uma vez por minuto em ASIA_PACIFIC, EUROPE e USA é executada em cinco regiões. Essa verificação de tempo de atividade é executada 219.000 vezes em um mês se configurada para uma única meta.

A tabela a seguir mostra as contagens de execução por hora e mensal para uma única verificação de tempo de atividade configurada para execução com frequências diferentes em diferentes números de regiões:

Frequência de execução da verificação, uma vez a cada:
Número de regiões
Execuções por hora
por destino Execuções mensais
por destino
1 minuto 3
4
5
6 180
240
300
360 131.400
175.200
219.000
262.800
5 minutos 3
4
5
6 36
48
60
72 26.280
35.040
43.000
52.660
10 minutos 3
4
5
6 18
24
30
36 13.140
17.520
21.900
26.280
15 minutos 3
4
5
6 12
16
20
24 8.760
11.680
14.600
17.520
Examples
Para estimar preços, determine seu total de execuções mensais e subtraia 1.000.000. Todas as execuções restantes são cobradas a US $0,30/1.000 .Portanto, multiplique as demais por 0,0003.

(EXECUTIONS_PER_MONTH - 1,000,000) * .0003
Cenário 1: você tem uma verificação de tempo de atividade no local USA que verifica uma VM uma vez por minuto. Essa verificação é executada em três regiões. O cheque é executado 131.400 vezes por mês e não custa nada.

Total de execuções mensais
Execuções mensais sujeitas à cobrança
(mais de 1.000.000) Custo
(US$ 0,30/1.000 execuções)
131.400 0 US$ 0,00
Cenário 2: você tem uma verificação de tempo de atividade no local USA que verifica um grupo de recursos de 10 membros uma vez por minuto. Essa verificação é executada em três regiões. O cheque é executado 10 * 131.400 vezes por mês e custa US $94,20/mês. A única diferença entre esse cenário e o cenário 1 é o número de destinos.

Total de execuções mensais
Execuções mensais sujeitas à cobrança
(mais de 1.000.000) Custo
(US$ 0,30/1.000 execuções)
1.314.000 (10 destinos) 314.000 US$ 94,20
Cenário 3: você tem 10 verificações de tempo de atividade GLOBAL, cada uma verificando uma VM uma vez por minuto. Essas verificações são executadas em seis regiões. Portanto, cada verificação é executada 262.800 vezes por mês. O total de execuções mensais é de 2.628.000 (10 * 262.800). Esse cenário custa US$ 488,40/mês.

Total de execuções mensais
Execuções mensais sujeitas à cobrança
(mais de 1.000.000) Custo
(US$ 0,30/1.000 execuções)
2.628.000 1.628.000 US$ 488,40
Cenário 4: você tem cinco verificações de tempo de atividade no local USA que verificam uma VM a cada cinco minutos. Essas verificações são executadas em três regiões. Portanto, cada verificação é executada 26.280 vezes por mês. O total de execuções mensais para esse conjunto de verificações é de 105.120 (4 * 26.280).

Você também tem duas verificações de tempo de atividade GLOBAL que verificam uma VM a cada 15 minutos. Essas verificações são executadas em seis regiões. Portanto, cada verificação é executada 17.520 vezes por mês. O total de execuções mensais para esse conjunto de verificações é de 35.040 (2 * 17.520).

Seu total de execuções mensais é de 140.160 (105.120 + 35.040). Esse cenário não custa nada.

Total de execuções mensais
Execuções mensais sujeitas à cobrança
(mais de 1.000.000) Custo
(US$ 0,30/1.000 execuções)
140.160 0 US$ 0,00
Preços para execução de monitor sintético (início da vigência: 1o de novembro de 2023)
O Cloud Monitoring cobra por execução de um monitor sintético, além da cota gratuita mensal de 100 execuções por conta de faturamento. Por exemplo, se você criar três monitores sintéticos e configurar cada um deles para ser executado a cada cinco minutos, o número total de execuções por mês será de 26.784:

Number of executions per month = 3 synthetic monitors * 1 execution per monitor per 5 minutes *
1440 minutes per day * 31 days per month
= 26,784
Para determinar o número de execuções faturáveis, subtraia a cota gratuita do número total de execuções e multiplique o resultado pelo custo:

Total de execuções mensais
Execuções mensais faturáveis
(mais de 100 execuções por conta de faturamento) Custo
(US$ 1,20/1.000 execuções)
26.784 26.684 US$ 32,02
Error Reporting
Para informações sobre os preços atuais, consulte Preços do Error Reporting.

Para saber os limites que se aplicam ao uso do Error Reporting, consulte Cotas e limites.

Cloud Profiler
Não há custo associado ao uso do Cloud Profiler.

Para saber os limites que se aplicam ao uso do Profiler, consulte Cotas e limites.

Cloud Trace
As cobranças do Trace são baseadas no número de períodos de traces ingeridos e verificados. Quando os dados de latência são enviados ao Trace, eles são agrupados como um trace composto por períodos. Esses períodos são ingeridos pelo back-end do Cloud Trace. Ao visualizar dados do trace, os períodos armazenados são verificados pelo Cloud Trace. Nesta seção, você encontra as informações a seguir:

Definição de períodos de traces sujeitos a cobrança ou não faturáveis
Exemplo de preços
Como reduzir a ingestão de períodos de traces
Configurações de uma política de alertas que notifica você se a ingestão de períodos de traces chegar ao limite
Para informações sobre os preços atuais, consulte Preços do Cloud Trace.

Para saber os limites que se aplicam ao uso do Trace, consulte Cotas e limites.

Para ver seu uso atual, acesse a página de relatórios do Cloud Billing ou a Visão geral do Trace no Console do Google Cloud:

ACESSAR VISÃO GERAL DO TRACE

Com base nessas informações, faça uma estimativa das suas faturas.

Períodos de traces não faturáveis
Os preços do Cloud Trace não se aplicam aos períodos gerados automaticamente pelo ambiente padrão do App Engine, pelo Cloud Functions ou pelo Cloud Run: a ingestão desses traces não é cobrada.

Períodos de traces sujeitos a cobrança
A ingestão de períodos de traces, exceto os listados na seção Traces não faturáveis, são faturáveis e cobrados por volume ingerido. Isso inclui períodos criados pela instrumentação que você adicionou ao aplicativo do ambiente padrão do App Engine.

Exemplos de preços
O exemplo a seguir mostra os preços do Trace desde julho de 2020.

Se você ingerir 2 milhões de períodos em um mês, o custo será de US$ 0. Os primeiros 2,5 milhões de períodos ingeridos em um mês são gratuitos.
Se você ingerir 14 milhões de períodos em um mês, seu custo será de US$ 2,30. Os primeiros 2,5 milhões de períodos em um mês são gratuitos. O custo dos períodos restantes é calculado como 11,5 milhões de períodos * US$ 0,20/milhão de períodos = US$ 2,30.
Se você ingerir um bilhão de períodos em um mês, seu custo será de US$ 199. Os primeiros 2,5 milhões de períodos em um mês são gratuitos. O custo dos períodos restantes é calculado como 997,5 milhões de períodos * US$ 0,20/milhão de períodos = US$ 199,50.
Como reduzir o uso de traces
Para controlar o volume de ingestão de períodos do Trace, gerencie a taxa de amostragem de traces. Assim, será possível equilibrar a quantidade necessária para analisar o desempenho com a tolerância de custo.

Para sistemas de tráfego intenso, a maioria dos clientes pode coletar amostras de uma em 1.000 transações, ou até uma em 10.000 transações, e ainda ter informações suficientes para analisar o desempenho.

A taxa de amostragem é configurada com as bibliotecas de cliente do Cloud Trace.

Criação de alertas sobre períodos ingeridos mensalmente
Para criar uma política de alertas que seja acionada quando os períodos mensais do Cloud Trace ingeridos excederem um limite definido pelo usuário, use as configurações a seguir.

Etapas para criar uma política de alertas
Novo estado
Campo
Valor
Recurso e métrica No menu Recursos, selecione Global.
No menu Categorias de métrica, selecione Faturamento.
No menu Métricas, selecione Períodos de trace mensais ingeridos.
Filtrar
Várias séries
Agregação de série temporal sum
Janela contínua 60 m
Função de janela contínua max
Campo
Configurar gatilho de alerta
Valor
Tipo de condição Threshold
Acionador de alerta Any time series violates
Posição do limite Above threshold
Threshold value Você determina o valor aceitável.
Teste a janela novamente O valor mínimo aceitável é de 30 minutos.
Anthos
Não há cobrança para registros e métricas do sistema do Anthos.

Em clusters do Anthos no cluster do VMware, os registros e as métricas de sistema do Anthos incluem o seguinte:

Registros e métricas de todos os componentes em um cluster de administrador
Registros e métricas de componentes nesses namespaces em um cluster de usuário: kube-system, gke-system, gke-connect, knative-serving, istio-system, monitoring-system, config-management-system, gatekeeper-system, cnrm-system
Perguntas frequentes
Quais recursos do produto são gratuitos?

O preço do uso de produtos do pacote de operações do Google Cloud é determinado pelo volume de dados. Além desse custo, o uso de todos os outros recursos de um produto do conjunto é gratuito.

Quanto preciso pagar?

Para estimar os custos de uso, consulte Como estimar suas faturas.

Consulte Perguntas de faturamento para receber ajuda sobre esse tema.

Como entender os detalhes do meu uso?

Várias métricas permitem analisar o volume de registros e métricas usando o Metrics Explorer. Consulte Visualizar o uso detalhado no Metrics Explorer para mais detalhes.

Se você quiser uma análise ainda mais detalhada sobre o uso dos registros, analise o volume usando as métricas com base em registros no Datalab. Leia esta postagem do blog do Google Cloud para mais informações.

Como o escopo das métricas afeta o faturamento?

Na maioria das vezes, o escopo das métricas não afeta o faturamento. Registros e métricas são cobrados no projeto do Google Cloud que recebe os dados. O escopo das métricas define a coleção de projetos que terão métricas visíveis e monitoráveis. Ao definir essa configuração, você não muda os projetos que recebem dados de métricas nem causa duplicação.

Por exemplo, imagine que sua organização tenha 100 máquinas virtuais (VMs): 60 delas são hospedadas pelo Projeto A e 40 estão no Projeto B. O Projeto A recebe e armazena as métricas das VMs que hospeda, e é cobrado quando elas estão sujeitas a cobrança. A mesma coisa acontece no Projeto B. Se você criar um escopo de métricas que inclua os dois projetos, será possível ver as métricas combinadas de todas as 100 VMs. Agora, você tem a opção de ver somente as métricas do Projeto A, do Projeto B ou a combinação de ambas. Apesar de haver duas maneiras de visualizar as métricas do Projeto-A, isso não afeta o faturamento.

Caso você queira monitorar contas da AWS, será necessário criar um projeto de conector da AWS para conectar uma conta desse serviço ao Google Cloud. O projeto conector mantém os registros e os dados de monitoramento da conta da AWS.

O que acontece se eu ultrapassar as cotas gratuitas?

Você receberá cobranças automáticas quando o uso ultrapassar as cotas gratuitas. Você não perderá registros ou métricas. Para entender melhor os possíveis custos, consulte Como estimar suas faturas.

Crie uma política de alertas que monitore o uso e envie notificações quando você estiver prestes a atingir o limite de faturamento.

Tenho um grande volume de registros do Google Cloud que não são utilizados nos meus projetos. Quais são as cobranças aplicadas a esses registros? O que fazer para evitá-las?

Exclua registros para controlar quais são ingeridos no Logging. Consulte Como reduzir seu uso de registros para ver detalhes.

Os serviços que enviam registros para meu projeto receberão um erro se os registros forem excluídos?

Não. Os serviços que enviam entradas de registros não podem determinar se elas são processadas no Logging ou não.

Serei cobrado duas vezes pelos registros de fluxo da nuvem privada virtual?

Se você enviar seus registros de fluxo da VPC para o Logging, as cobranças de geração desses registros de fluxo serão dispensadas, e apenas as cobranças do Logging serão aplicadas. No entanto, se enviá-los e, em seguida, excluí-los do Logging, haverá cobranças por eles. Para mais informações, consulte a calculadora de preços do Google Cloud e selecione a guia “Cloud Load Balancing e Network Services”.

1 Para fins de definição de preços, todas as unidades são tratadas como medidas binárias, por exemplo, como mebibytes (MiB, ou 220 bytes) ou gibibytes (GiB ou 230 bytes).

2 Não há cobrança para as métricas do Google Cloud ou do Anthos que são medidas em até um ponto de dados por minuto (a resolução mais alta no momento). Futuramente, as métricas medidas em resoluções mais altas poderão ser cobradas.

3 Atualmente, as métricas do processo são coletadas a uma taxa padrão predefinida de uma vez por minuto, o que não pode ser alterado. Em geral, esses dados mudam lentamente. Por isso, essas métricas estão sendo amostradas. Portanto, as métricas do processo de cobrança a 5% da taxa padrão se alinham à taxa padrão se as métricas forem amostradas em intervalos de 20 minutos. Os usuários que coletam 100 MiB de dados dessas métricas são cobrados por apenas 5 MiB.

A seguir
Leia a documentação do pacote de operações do Google Cloud.
Use a calculadora de preços.
Saiba mais sobre as soluções e casos de uso do pacote de operações do Google Cloud.
Solicite uma cotação personalizada
Com os preços de pagamento por utilização do Google Cloud, você paga apenas pelos serviços que usa. Fale com nossa equipe de vendas e receba uma cotação personalizada para sua organização.
Entre em contato com a equipe de vendas)
capitulo 6 (Intro
0:00
SPEAKER: In our last episode, we covered the best practices
0:02
for deploying and using cloud operations in an enterprise
0:05
environment.
0:06
But we still left some questions unanswered.
0:09
How should you monitor your services?
0:11
How should you deal with alerts?
0:13
And what about managing costs?
0:14
Today, we’ll look at best practices
0:16
that you can use to get the most value out of cloud monitoring.
0:20
Welcome to Engineering for Reliability with Google Cloud.
0:22
0:26
Just like last time, let’s first figure out
Monitoring Objectives
0:29
why monitoring is important at all.
0:31
What are we trying to achieve when we use cloud monitoring?
0:34
We’re after three main objectives in parallel.
0:37
Our first objective is to keep our users happy.
0:39
That means we need to know whether our service is
0:41
meeting their needs.
0:42
And the best way to do that is through well-defined SLOs
0:45
and error budgets, and alerts that
0:47
let us know when our service is burning error budget.
0:51
Our second objective is to be able to quickly and effectively
0:53
respond when those alerts do fire.
0:56
This means having enough data about the state of our service
0:59
to be able to triage incidents, identify effective mitigations,
1:03
and accurately confirm the effectiveness
1:05
of those mitigations.
1:07
Our final goal is to do the first two while managing
1:10
the associated costs.
1:12
Now that we’ve covered the whys, let’s turn to the hows.
1:15
We’ll start by talking about what to monitor.
1:18
From there, we’ll get into how to best manage alerts.
1:21
And finally, we’ll cover cost management
1:23
for cloud monitoring.
1:25
Let’s get into it.
1:27
Let’s start by talking about the obvious first question.
What to Monitor
1:29
What should you be monitoring?
1:31
For the answer, we can turn to chapter 6
1:33
of the “Site Reliability Engineering” book on monitoring
1:36
distributed systems.
1:38
Fundamentally, the objective of monitoring
1:40
is to answer two questions.
1:41
The first one is all about symptoms.
1:43
What are our users experiencing, and is that experience
1:46
in any way less than ideal?
1:49
The second question is all about causes.
1:51
What’s causing the symptoms we’ve identified?
1:54
That cause may be direct or intermediate,
1:56
but it’s how we start to determine
1:58
how to restore user experience back to the desired state
2:01
if it’s degraded in some way.
2:03
We answer the first question by clearly defining our service,
2:06
identifying good service level indicators, or SLIs
2:10
that tell us, as accurately as possible,
2:12
how well our service is able to meet our users’ expectations,
2:16
and defining good service level objectives, or SLOs, that
2:19
set a target that our SLIs have to meet.
2:24
We’ve covered defining services, SLIs, and SLOs
2:27
in cloud monitoring extensively in the series,
2:29
but it’s always worth revisiting these topics.
2:31
The first thing to answer to the question of what should we
2:34
monitor is, how well is your service
2:36
meeting the needs of your users as expressed by good SLOs?
2:41
The next thing to make sure you’re monitoring covers
2:43
is what the “SRE” book refers to as the golden signals.
2:47
Traffic is essentially a measure of how much
2:49
user activity the service is responding to, usually
2:52
as a count of incoming requests for user-facing services
2:55
or data elements for data pipelines.
2:58
Error rate is a measure of what percentage of the time
3:01
the user activity is not successful,
3:03
which, of course, depends on the service and user expectations.
3:07
Latency is a measure of how long the service takes
3:09
to service a request.
3:11
And finally, saturation is a measure
3:13
of how much of the available capacity
3:15
the service is using at a given time.
3:17
3:19
A great way to ensure that you have
3:21
easy access to these signals is to create a dashboard
3:24
like this.
3:25
It shows the four golden signals for a given service at once.
3:28
It makes it easy to correlate, for example, increases
3:30
in inbound traffic to latency degradations or increased
3:34
capacity requirements.
3:35
You could automate the creation of dashboards
3:37
like this for your services.
3:39
We’ll link to some examples in the episode notes.
3:43
Finally, you may need to augment your monitoring
3:45
with custom telemetry to capture service-specific information.
3:48
We covered doing this in a previous episode.
3:50
Review that for an introduction to instrumenting your services
3:53
with OpenCensus and Prometheus.
3:55
So that takes care of the first question,
3:57
what you should be monitoring.
3:59
We’ve just covered SLOs, golden signals, and custom telemetry,
4:03
which brings us to alerting.
Alerting Best Practices
4:05
How should you configure alerts?
4:06
What should you alert on?
4:07
And how should you respond to alerts?
4:09
Let’s take a look.
4:12
Let’s again return to the monitoring chapter of the “SRE”
4:14
book.
4:15
These four criteria should be applied
4:16
to alerts that go to pagers.
4:18
Every time the pager goes off, we
4:20
should be able to react with a sense of urgency.
4:23
But we can only react with a sense of urgency
4:25
a few times a day before we become fatigued.
4:28
Every page should be actionable.
4:31
Every page response should require intelligence.
4:33
If a page merits only a robotic response,
4:35
it shouldn’t be a page.
4:37
And ideally, pages alert us about a novel problem
4:41
or an event that hasn’t been seen before.
4:43
That means we need to take action
4:44
to prevent pages from reoccurring once we’ve
4:46
mitigated the triggering condition
4:48
and, hopefully, identified the root cause.
4:51
Alerts that don’t meet these criteria should not be pages.
4:54
Alerts that aren’t actionable are of no use at all.
4:57
Alerts that require human intervention
4:59
but that aren’t urgent should be filed as tickets instead.
5:03
Cloud monitoring supports multiple notification channels.
5:06
And this allows you to set up alert delivery that
5:08
meets your needs.
5:09
For example, you could use email or PagerDuty delivery
5:11
to trigger pagers.
5:13
Then configure a webhook or Pub/Sub integration
5:15
to file tickets for non-urgent alerts.
5:19
You can also automate the management of your alerts
5:21
by using an automation tool like Terraform.
5:23
This helps to ensure consistency and avoids human errors
5:27
in alert configuration.
5:29
Finally, it’s important to understand
5:31
the tools you have available to capture and optimize
Optimizing Costs
5:33
your monitoring costs.
5:34
Let’s have a look at those now.
5:38
First, it’s important to understand
5:39
how you incur monitoring costs.
5:42
Platform metrics emitted by Google Cloud Services
5:44
are always free.
5:45
You are charged for other metrics,
5:47
such as custom metrics or those written by Istio,
5:50
based on storage volume.
5:52
Refer to the Pricing page for the latest
5:53
version of this information.
5:55
The Monitoring Settings page shows you exactly how much data
5:58
you are ingesting for each project in your metrics scope.
6:01
You can measure your usage by using billing reports
6:04
and filtering them to just the monitoring service
6:07
to see exactly how much monitoring charges you
6:09
are incurring in your project.
6:11
You can even figure out exactly how much
6:13
data is being ingested by each custom metric
6:15
by creating a chart and using the Metric Bytes Ingested
6:19
metric.
6:20
These tools do a great job of helping
6:22
you understand the sources of monitoring costs.
6:25
But what can you do to optimize those?
6:26
Let’s have a look.
6:29
The way that you use labels for cloud components
6:31
might impact the volume of time series
6:33
that are generated for your metrics and monitoring.
6:36
For example, you can use labels to appropriately
6:38
report metrics to cost centers on your bill
6:41
and to signify whether specific environments are production
6:43
or development.
6:45
Adding these labels means that additional time series
6:47
are generated in monitoring.
6:49
You can calculate the total number of times series
6:51
by multiplying the cardinality of all labels.
6:55
For example, if there are 11 cost center
6:57
values and 5 environment values, that
7:00
means 55 time series are generated.
7:02
This is why the way that you add labels might
7:05
add significant metric volume, and, therefore,
7:07
increase the cost.
7:09
We recommend carefully limiting the number of labels
7:11
and avoiding label values with high cardinality.
7:15
Metrics sent from the Cloud Ops Agent
7:17
are another source of monitoring costs.
7:19
The agent collects app and system metrics
7:21
from common third-party apps and additional VM-level metrics.
7:25
If you don’t need them for certain VMs,
7:27
you can reduce the volume by not sending these metrics.
7:30
You can also reduce the metric values
7:32
by reducing the number of VMs that use the agent.
7:35
Custom metrics are chargeable metrics
7:37
created by using the monitoring API or integrations
7:40
like OpenCensus to monitor any metrics that
7:42
are user instruments.
7:43
The more services that you instrument to send metrics,
7:46
the more custom monitoring metrics are generated.
7:49
If you want to reduce metric volumes,
7:51
you can reduce the number of custom monitoring metrics
7:53
that your services send.
Wrap Up
7:56
Thanks for joining me today.
7:57
We’ve covered best practices for setting up and using
7:59
cloud monitoring, including what to monitor,
8:02
how to manage alerts, and how to optimize your monitoring costs.
8:05
I hope these recommendations help you keep your users happy.
8:08
In our next episode, we’ll tackle best practices
8:11
for using cloud logging.
8:12
Thanks so much for watching today.
8:14
Don’t forget to like and subscribe to never miss out
8:16
on more Engineering for Reliability with Google Cloud.
8:19
See you soon.
8:20
[MUSIC PLAYING])
7 (Intro
0:00
SPEAKER: We’ve covered using Cloud monitoring
0:01
in your projects.
0:02
But what if you’re responsible for managing many projects,
0:05
and you need to unify monitoring across them?
0:07
And how can you control access to monitoring data
0:09
from many projects?
0:11
Today, we’ll look at Cloud monitoring metrics scopes,
0:14
and learn how to use them to monitor multiple Cloud
0:16
projects.
0:17
Welcome to Engineering for Reliability with Google Cloud.
0:20
Metrics Scopes and Monitored Projects
0:24
Let’s start with a simple example.
0:26
How can you make it easier to view monitoring data
0:28
for multiple projects?
0:31
If I go to monitoring settings for my project,
0:33
I can see that my current metrics scope only
0:35
has a single project in it, the one I’m currently viewing.
0:38
I can add others, but what’s actually happening here?
0:41
Let’s have a look at metrics scopes and how they work.
0:46
When you create a Google Cloud project,
0:48
that project hosts a metrics scope
0:50
and becomes the scoping project for that scope.
0:53
It stores the alerts, uptime checks, dashboards,
0:56
and monitoring groups that you configure for the scope.
0:59
For example, if you create a staging project and then
1:02
access monitoring, you can see the metrics
1:04
for the resources in the staging project.
1:06
This happens for every project you create.
1:09
Each project creates a metrics scope for itself,
1:12
and hosts monitoring configuration for itself.
1:15
But what if you want to centralize how that data is
1:17
stored and how it’s accessed?
1:19
You can add multiple projects to an existing scope.
1:22
Now, monitoring data for all projects in that scope
1:25
will be visible.
1:27
This will let you do things like create dashboards
1:29
showing resources from all the projects in the scope,
1:31
or alerting policies that apply to resources
1:34
in multiple projects as long as they’re in the metrics scope.
1:38
Note that the recommended approach for production
1:40
deployments is to create a dedicated project to host
1:42
monitoring configuration data and use its metrics
1:45
scope to set up monitoring for the projects that
1:47
have actual resources in them.
1:49
This way, should a project not be necessary anymore
1:52
and get deleted, the monitoring configuration
1:54
for all the other projects won’t be impacted.
1:57
What about access?
1:58
While in this configuration, you just
2:01
must have appropriate IAM permissions
2:03
to access monitoring data.
2:04
For example, a user would need to have the right role
2:07
in the monitoring project to be able to see monitoring
2:10
data for both projects.
2:12
A user who only has access to the staging project
2:14
would not be able to see any monitoring data
2:16
for the production project.
2:18
Now that you understand what metrics scopes are
2:21
and what to use them for, let’s have
2:22
a look at how to set them up in Cloud monitoring.
Managing Metrics Scopes in Cloud Console
2:26
Let’s start in our staging project.
2:27
2:30
We’ll go to Compute Engine, and see that we
2:32
have a single VM running.
2:33
2:37
We can go to monitoring, and see that monitoring data for the VM
2:40
is being shown.
2:43
For example, on the infrastructure summary
2:45
dashboard.
2:46
Let’s now go to our monitoring project,
2:52
and confirm that there aren’t any compute instances
2:54
running in it.
2:55
2:59
We also don’t have the out-of-the-box compute
3:01
dashboards because we don’t have any resources running in this
3:03
project.
3:04
Let’s now add our staging project
3:06
to be monitored by this metrics scope.
3:10
We can do that in monitoring settings by adding a project,
3:15
selecting the project we want to add,
3:18
and confirming that we want to use this monitoring
3:21
project as the scoping project rather than creating
3:24
a new scope.
3:24
3:28
Once this operation is complete, monitoring data
3:31
from the staging project will be visible in this metrics scope.
3:35
We can confirm that by going to the VM instances dashboard,
3:38
for example.
3:39
From here, we can see more details
3:40
about the instance being monitored, even though it’s
3:43
running in another project.
3:45
So that’s how we can use the Cloud Console to configure
3:48
metrics scopes and collect monitoring
3:50
data for multiple projects.
3:53
So that’s how to configure metrics scopes in the UI.
Monitoring data across multiple projects
3:56
But how can you figure out where your project is
3:58
being monitored, or where the monitoring data you can see
4:00
in your project is coming from?
4:02
Let’s have a look.
4:04
Now that we have added our staging project
4:06
to our monitoring metrics scope, let’s
4:08
see how we can navigate between the two.
4:11
We can see information about our current metrics scope
4:13
here on the monitoring overview page for the monitoring
4:15
project.
4:17
If we click on that, we can see that the monitoring project
4:20
is monitoring metrics for resources
4:21
running in the project itself and in our staging project.
4:26
We can go there directly from here.
4:30
In the staging project, we can do the same thing,
4:33
and see that this project is monitoring metrics for itself,
4:36
and that it is being monitored by our monitoring project.
4:40
And we can go back to that project
4:41
simply by clicking on that link.
4:44
So that’s how you can navigate between metrics scopes
4:47
and monitored projects in Cloud monitoring.
4:51
Navigating metrics scopes in the UI is easy enough.
Managing Metrics Scopes using the API
4:53
But how can you ensure that, for example, new projects
4:56
are added to your Production Monitoring configuration?
4:58
You can use the API to automate that.
5:00
Let’s have a look.
5:03
Let’s start in monitoring settings,
5:07
and confirm that this particular metrics scope is only
5:10
monitoring this project, which is the scoping
5:12
project for this metrics scope.
5:15
Now let’s go to our API.
5:17
We’ll use the Create method for metrics scopes projects
5:20
which takes two arguments.
5:21
First one is the parent, which is the metrics
5:24
scope that we want to add our stage and project to.
5:27
The second is our project itself,
5:30
which is a monitored project resource.
5:32
The name field includes a reference
5:34
to both the staging project and the metrics scope
5:36
we’re adding this project to.
5:39
Let’s execute this request, authenticate, and confirm
5:42
that the operation is done.
5:44
We can now go back to monitoring settings for our monitoring
5:47
project, refresh the page, and confirm
5:50
that the staging project has been
5:52
added to this metrics scope.
5:54
So that’s how you can use the Cloud monitoring
5:56
API to manage how projects are monitored by metrics scopes.
Outro
6:00
Thanks for joining me today.
6:02
We covered how metrics scopes lets you configure
6:04
monitoring across projects, and how to manage them in the UI
6:07
and using the API.
6:09
I hope this helps you standardize and automate
6:11
your monitoring, run more reliable services,
6:13
and keep your users happy.
6:14
Thanks so much for watching.
6:16
Don’t forget to like and subscribe to never miss out
6:18
on more Engineering for Reliability with Google Cloud.
6:21
See you soon.
6:23)

8 (0:00
SPEAKER: One thing that makes Google Cloud
0:01
production ready and ops-friendly
0:04
is the broad range of management,
0:05
monitoring, and alerting tools that it comes with.
0:09
While tools are no magic wand and do not
0:12
replace DevOps or SRE practices, you
0:15
should really watch this video to better understand
0:17
what they’re all about.
0:18
[MUSIC PLAYING]
0:22
0:25
Now, before I start talking about specific tools,
0:29
let me mention that these products work
0:31
best in the context of a team applying SRE or Site
0:35
Reliability Engineering principles.
0:37
There is not enough time to delve into this,
0:40
but you’ll find links to SRE literature on Service-Level
0:44
Objectives, or SLOs, error budget,
0:47
and blameless postmortems in the video description below.
0:51
The Hello World for DevOps tools is arguably the ability
0:54
to collect, read, and parse logs across a distributed
0:58
infrastructure involving multiple products.
1:01
Cloud Logging stores logs across all Google Cloud products
1:05
and provides you with search, monitoring,
1:08
and alerting capabilities.
1:10
It also comes with an API to ingest custom log data
1:13
from any source.
1:15
Because it is a fully managed service,
1:17
there are no hard drives to provision
1:19
or partitions to resize.
1:21
And it can ingest application and system log data
1:25
from thousands of sources simultaneously.
1:28
Even better, you can analyze all the log data
1:31
as it arrives in real time without having
1:33
to worry about synchronizing your server pods
1:37
or managing time zones.
1:38
Logs are made up of entries created
1:41
by Google Cloud Services, third-party applications,
1:44
or by your own code.
1:46
The message carried by the log entry is called the payload,
1:51
and it can be a simple string or structured data.
1:54
Examples of log entries can include
1:57
details of a compute engine instance starting up,
2:01
a new file being uploaded to a bucket,
2:04
a call made to a machine learning API,
2:06
or anything that your application writes
2:09
to the standard or error outputs.
2:11
Each log entry indicates where it
2:14
came from by including the name of the monitored resource.
2:17
Using the console’s Logs Viewer, you can query logging data
2:21
and obtain a precise subset of all the log
2:24
entries in your project.
2:26
The query will let you find entries
2:29
for a given resource from different namespaces based
2:32
on the log level and, of course, by timestamp.
2:37
Note that if using the console isn’t your thing,
2:40
these queries are also accessible from the logging
2:42
API, as well as from the command line.
2:45
Storing logs is free for the first gigabyte for every
2:49
project and then comes at $0.50 per additional gigabyte.
2:53
And your alerting policy can be set up
2:55
to trigger when your monthly logs ingested exceeds a given
2:58
limit.
2:59
But you can also define excluded logs
3:01
so that some are not stored in the first place.
3:05
The logs viewer and the logs API are powerful tools
3:08
on their own, but you can also decide
3:10
to export your logs to cloud storage,
3:14
to BigQuery, or to Pub/Sub, which then in turn
3:18
redirects them to virtually any log storage system.
3:22
Exporting logs is likely something
3:24
that you will want for archival or potentially legal purposes,
3:29
but also maybe to benefit from more advanced analytics.
3:32
There is even more to logs, but hopefully this
3:34
gives you a good sense of what every Google Cloud
3:37
product can rely on.
3:38
So now you know how logs are aggregated across all of Google
3:42
Cloud and how to navigate them.
3:45
If you liked this video, please like, subscribe, comment,
3:48
share, and look forward to more Google Cloud Essentials videos.
3:51
[MUSIC PLAYING])

9 (0:00
okay so in our previous video we had
0:01
seen whether a particular application
0:03
was in a running state or not so we had
0:04
used an apache web server and we had
0:06
used the uptime check to see whether
0:08
that particular web server was running
0:10
or not now the link to that particular
0:12
video i’ll give you the description
0:13
below as well as over here so in this
0:15
particular chapter we’ll do something
0:17
else so we have an instance running and
0:18
we want to check whether the cpu of that
0:21
particular instance
0:22
crosses a particular threshold now let’s
0:24
see how we can do something like that so
0:26
the first thing that we’ll do is we’ll
0:27
create a instance so let’s do that so
0:29
let’s go to our
Increase CPU utilization
0:31
compute engine and let’s go to a vms so
0:33
i’ve already created a vm instance so
0:35
let’s log into this vm instance
0:39
so let’s ssh into it
0:41
so to see the cpu utilization of this
0:43
particular machine so all that you need
0:45
to do is you need to run the top command
0:47
and you can see that currently the cpu
0:49
utilization is very less what we’ll do
0:50
is we need to increase the cpu
0:52
utilization so so here i have a stack
0:54
overflow page and this particular page
0:56
the link to this particular page i’ll
0:57
give in the description below so here
0:59
you can use a few commands to increase
1:01
the cpu utilization so i’ll be using
1:03
this particular command to increase the
1:04
cpu utilization of my machine so let me
1:06
just copy this and let’s paste it over
1:08
there
1:12
let’s exit out of this
1:14
clear screen
1:15
and let’s run this particular command
1:18
and now if i do a top
1:20
hopefully the cpu utilization of this
1:22
machine should have increased and you
1:24
can see that it has gone up to 93
1:26
and it’s gone up to 100 so now the next
1:28
thing that i need to do is i need to run
1:30
an alerting policy so that whenever my
1:32
cpu crosses a particular threshold it
1:34
should send an alert to a user
1:36
so let’s do that so let’s go back to our
1:39
console again and let’s go to alerting
Create an alerting policy
1:41
so this is again part of the monitoring
1:43
of course you can go to your hamburger
1:44
menu
1:46
and you will find alerting
1:48
underneath your monitoring section so
1:50
let’s
1:51
go to your monitoring and let’s click on
1:53
alerting
1:55
so currently there are no policies so
1:57
let’s create an alerting policy let’s
1:59
click on create policy
2:02
and here what you need to do is you need
2:04
to select the appropriate metrics so
2:05
let’s click on select metric
2:07
and we need to select a metric based on
2:09
the vm instance now of course you can
2:11
have alerting policies for other
2:12
services as well now for this particular
2:15
chapter we’ll just go for vm instance
2:18
and here you can go to your instance and
2:20
within your instance you can click on
2:21
cpu utilization and click on apply
2:26
and here to get a more appropriate or
2:29
more accurate data point what you can do
2:31
is you can actually lower your time so
2:32
let’s just make this as one
2:36
and here you can see a more appropriate
2:37
graph so here it shows when this
2:40
particular cpu utilization touches
2:41
around 90
2:43
so here we’ll select this particular
2:45
data point of one minute and we will
2:47
select the cpu utilization so let’s go
2:49
to next so here what we need to choose
2:52
is when you need to apply your
2:53
particular trigger so anytime the time
2:55
series violates above a particular
2:57
threshold so here you need to choose the
2:58
percentage so let’s choose the
3:00
percentages let’s say around 80 percent
3:04
whenever the cpu utilization goes above
3:06
80 percent uh trigger will be sent so
3:10
that’s about it let’s go to next
3:12
so here you need to select the
3:13
notification so again i’ve already
3:15
created a notification
3:17
in my previous chapter so i’ll be using
3:19
the same notification so
3:20
okay so now let me show you how the
3:22
notification channel looks like so let’s
3:24
open this in a new tab
3:25
so here are all the notification
3:27
channels that are currently available to
3:28
you you can either send a slack a web
3:30
hook or email an sms or you can send a
3:32
pub sub
3:33
so what i have done is i have sent an
3:35
email to this particular so whenever my
3:38
trigger is set it will send an email to
3:39
this particular email id
3:42
okay so once this is done let’s go back
3:44
to our
3:46
uh configure notification and let’s
3:48
choose this email that i have previously
3:50
configured
3:51
and
3:52
that’s about it now of course you can
3:54
also have other optional fields as well
3:56
but that’s not important for this
3:58
chapter so let’s just call this as my vm
4:01
alert
4:03
and let’s create a policy
4:11
and let’s wait for the trigger to be set
4:15
and an email to be sent to that
4:16
particular email id so let’s just wait
4:18
for a minute
4:19
and once you go back to your alerting
4:21
page you can see that there is an
4:22
incident that has taken place that’s
4:23
because the cpu utilization crossed the
4:25
80 threshold so now let’s see whether
4:27
we’ve received our email so let’s go
4:29
back to our email id and here you can
4:31
see that the cpu utilization has crossed
4:33
the 80 percent threshold so the value is
4:36
currently
4:37
90.90 whereas the cpu utilization
4:39
threshold we had set was 0.8 or 80
4:42
so that’s it for this lecture so in this
4:44
lecture you learned how you can set
4:46
alerts for a particular vm instance
4:48
based on rcp utilization so i hope this
4:50
was a useful lecture if you have any
4:52
issues with any of the other matrix
4:55
related to alerting please get in touch
4:57
with me that’s about it for this lecture
4:59
i will see in the next)

10 (
Console

Google Cloud Service Health Incidents Cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2.
Service Health
This page provides status information on the services that are part of Google Cloud. Check back here to view the current status of the services listed below. If you are experiencing an issue not listed here, please contact Support. Learn more about what’s posted on the dashboard in this FAQ. For additional information on these services, please visit https://cloud.google.com/.
Available
Service information
Service disruption
Service outage
Incident affecting Google Compute Engine
Cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2.

Incident began at 2022-07-19 06:33 and ended at 2022-07-20 21:20 (all times are US/Pacific).

Previously affected location(s)
London (europe-west2)

DATE TIME DESCRIPTION
29 Jul 2022 14:05 PDT
For a full Incident Report, please refer to https://status.cloud.google.com/incidents/fmEL9i2fArADKawkZAa2

21 Jul 2022 12:06 PDT
For a preliminary Incident Report (Mini IR) , please refer to https://status.cloud.google.com/incidents/fmEL9i2fArADKawkZAa2

19 Jul 2022 20:45 PDT
There was a cooling related failure in one of our buildings that hosts a portion of capacity for zone europe-west2-a for region europe-west2 that is now resolved. GCE, Persistent Disk and Autoscaling impacts have been addressed. Customers can launch VMs in all zones of europe-west2. A small number of HDD backed Persistent Disk volumes are still experiencing impact and will exhibit IO errors. If you are continuing to experience issues with these services, please contact Google Cloud Product Support and reference this message.

The issue has been resolved for all affected users as of Tuesday, 2022-07-19 20:43 US/Pacific.

We thank you for your patience while we worked on resolving the issue.

19 Jul 2022 15:29 PDT
Summary: Cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2.

Description: Mitigation work is currently underway by our engineering team.

We do not have an ETA for mitigation at this point.

There is a cooling related failure in one of our buildings that hosts a portion of capacity for zone europe-west2-a for region europe-west2 that is not yet completely resolved. GCE, Persistent Disk and Autoscaling impacts have been mitigated. Most customers can launch VMs in all zones of europe-west2. A minority of customers might continue to see failures in europe-west2-a. We continue to work on bringing back previously impacted capacity in europe-west2-a to fully restore GCE, Persistent Disk and Autoscaling. If you are continuing to experience issues with these services, please contact Google Cloud Product Support and reference this message.

Customers who launched new VMs in zones europe-west2-b and europe-west2-c and would like to delete their previously running VMs in europe-west2-a, can delete VMs via the console or GCE APIs. There might be a delay in processing the deletion and all deletions will be fully processed when all issues in europe-west2-a are resolved.

Diagnosis: Customers impacted by this issue would have seen abnormal VM terminations for a small set of their VMs.

Workaround: Customers who launched new VMs in zones europe-west2-b and europe-west2-c and would like to delete their previously running VMs in europe-west2-a, can delete VMs via the console or GCE APIs. There might be a delay in processing the deletion and all deletions will be fully processed when all issues in europe-west2-a are resolved.

19 Jul 2022 14:08 PDT
Summary: Cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2.

Description: Mitigation work is currently underway by our engineering team.

We do not have an ETA for mitigation at this point.

There is a cooling related failure in one of our buildings that hosts a portion of capacity for zone europe-west2-a for region europe-west2 that is not yet completely resolved.

GCE, Persistent Disk and Autoscaling impacts have been mitigated. Most customers can launch VMs in all zones of europe-west2.

A minority of customers might continue to see failures in europe-west2-a.

We continue to work on bringing back previously impacted capacity in europe-west2-a to fully restore GCE, Persistent Disk and Autoscaling. If you are continuing to experience issues with these services, please contact Google Cloud Product Support and reference this message.

Please refer to workaround section for additional information about VM deletion.

We will provide more information by Tuesday, 2022-07-19 16:00 US/Pacific.

Diagnosis: Customers impacted by this issue would have seen abnormal VM terminations for a small set of their VMs.

Workaround: Customers who launched new VMs in zones europe-west2-b and europe-west2-c and would like to delete their previously running VMs in europe-west2-a, can delete VMs via the console or GCE APIs. There might be a delay in processing the deletion and all deletions will be fully processed when all issues in europe-west2-a are resolved.

19 Jul 2022 12:29 PDT
Summary: Cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2. Europe-west2-b and europe-west2-c are not impacted for VMs. We have fixed the previously occurring issues when creating new Persistent Disk devices. Zonal autoscaling for europe-west2-a is impacted for customers who suffered VM terminations.

Description: We are experiencing an issue with Google Compute Engine beginning at Tuesday, 2022-07-19 08:10 US/Pacific.

Our engineering team continues to investigate the issue.

There has been a cooling related failure in one of our buildings that hosts zone europe-west2-a for region europe-west2. This caused a partial failure of capacity in that zone, leading to VM terminations and a loss of machines for a small set of our customers. We’re working hard to get the cooling back on-line and create capacity in that zone. We do not anticipate further impact in zone europe-west2-a and currently running VMs should not be impacted. A small percentage of replicated Persistent Disk devices are running in single redundant mode.)
