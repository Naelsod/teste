# README
#Pré-requisitos para rodar localmente o projeto:
O projeto foi rodado localmente numa máquina
Windows 10 
Utilizando a plataforma
Mendix Studio Pro 10.24.13
E salvando suas informações no
Postgree 18.6

#Tecnologias:
Mendix: Apesar de não ter conhecimento eu me desafiei a usar o Mendix para começar meu aprendizado na plataforma e queria aprender como ela funciona, além de ela ser uma plataforma low code facilitando bastante o meu desenvolvimento
Postgres: Utilizei o banco do Postgres por ele ser capaz de lidar com grandes números de dados e por ter maior familiaridade.

#Banco de dados:
As informações foram salvas no banco do Postgres dentro de uma tabela simples
que contém um id como primary key, datahora, Temperatura e eficiência.
o banco não tem bem um script a parte para sua criação pois suas tabelas foram criadas automaticamente pelo Mendix após confirmar na hora de executar a aplicação, a única configuração que eu tive que fazer foi colocar o url e as credenciais do banco dentro da plataforma Mendix

#API:
Utilizei a Api openweathermap para buscar as informações de uma cidade.
No projeto deixei fixa em Patos de minas.

#Oque Faltou:
Mesmo no meu primeiro contato com Mendix eu acredito ter atendido as necessidades do projeto, porém acho que poderia melhorar o design, colocar um sistema de alerta e monitoramento com mais funcionalidades, permitir o usuário escolher a cidade buscada na api, possibilitar que o sistema tenha diversas máquinas e fazer um código mais limpo e eficiente e com melhores práticas de programação

#Perguntas:

Se em vez de 1 máquina fossem 100, enviando leituras a cada 5 minutos, o que você imagina que
precisaria mudar ou poderia travar no seu sistema?

R = Meu sistema foi projetado incialmente para fazer a leitura dos dados de uma máquina, assim eu teria que mudar a maneira operante pois 100 máquinas poderiam pesar um pouco da aplicação, teria que colocar um id, nome e cidade para cada uma das máquinas, teria que alterar os meus Flows para que operassem de acordo com o id da máquina informado e não com um vínculo fixo igual funciona agora.

Se quiséssemos, no futuro, prever falhas antes que aconteçam usando os dados de temperatura e
eficiência, que tipo de dado histórico você imagina que seria útil coletar desde já? 

R Como a máquina e ligada diretamente com a temperatura, imagino que seria importante verificar qual época e horário são mais frios e qual e mais quente, dessa forma conseguimos estimar em que época a máquina vai ter mais dificuldade em operar e se programar de acordo 

Cite uma melhoria que você faria no sistema se tivesse mais tempo, e por quê.

R= Eu colocaria um sistema de filtro no histórico para que seja possível pesquisar por dia mês ano ou até máquina, assim você consegue ver qual horário do dia foi mais eficiente ou menos eficiente 
Poderia fazer com que o sistema consiga criar as máquinas e que elas também tivessem nome e cidade como atributo, assim possibilitando o programa a ter mais de uma máquina e mais de um local de trabalho
Também faria um dashboard mais robusto com gráficos gerais e números de todas as máquinas operante, média de eficiência das máquinas entre outras funcionalidades.
