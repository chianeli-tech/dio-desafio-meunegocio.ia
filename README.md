# dio-desafio-meunegocio.ia

Solução do desafio Negócio com IA e Lovable

Decidi pelo AulaFácil porque podemos começar com um problema muito concreto — a organização administrativa do professor — sem tentar transformar o MVP em uma plataforma de ensino completa.

1. Dores que o AulaFácil pretende resolver

O professor particular costuma administrar sua atividade usando uma combinação de WhatsApp, agenda do celular, planilhas, cadernos e memória. Isso espalha informações importantes: horários das aulas, dados dos alunos, conteúdos trabalhados, pagamentos e pendências ficam em lugares diferentes, aumentando o risco de esquecimentos e retrabalho.

Outra dor é a falta de visão consolidada do negócio. O professor pode saber quais aulas tem hoje, mas nem sempre consegue responder rapidamente: quantos alunos ativos tenho? Quanto tenho para receber? Quantas aulas dei este mês? Quais alunos estão com pagamento pendente? O AulaFácil reuniria essas informações em um único painel.

Por fim, existe uma dor de acompanhamento pedagógico e histórico. Registrar o que foi trabalhado em cada aula permite que o professor retome o conteúdo na aula seguinte e tenha uma visão da evolução do aluno. No MVP, isso pode ser resolvido de maneira simples, com histórico e observações — sem precisar construir inicialmente uma plataforma pedagógica complexa.

Proposta de valor inicial:

“O AulaFácil ajuda professores particulares a organizar alunos, aulas e pagamentos em um único lugar, reduzindo o trabalho administrativo e permitindo que eles se concentrem no ensino.”

2. Estimativa do mercado

Aqui é importante separar mercado potencial de mercado que efetivamente compraria o software. Não encontrei uma estatística oficial que diga exatamente quantos professores particulares no Brasil poderiam ser clientes de um SaaS como o AulaFácil. Portanto, não seria correto apresentar um número inventado como “tamanho do mercado”.

Podemos, entretanto, construir uma estimativa de ordem de grandeza usando a população estudantil como base e depois aplicar hipóteses explícitas.

Brasil

O Censo Escolar 2025 registrou 46,0 milhões de matrículas na educação básica, sendo 9,25 milhões na rede privada.

Isso representa uma base enorme de potenciais usuários indiretos do serviço: alunos e suas famílias. O público-alvo direto do AulaFácil, entretanto, são os professores particulares, e não os estudantes.

Para o MVP, eu trabalharia com a seguinte hipótese de mercado:

Indicador	Estimativa para o projeto
Matrículas na educação básica	46,0 milhões
Potenciais alunos que podem demandar apoio particular	hipótese a validar
Professores particulares potenciais	mercado ainda a dimensionar
Público inicial	Professores particulares independentes
Nicho inicial	Matemática, Física e reforço escolar

Portanto, no Business Model Canvas eu chamaria o mercado brasileiro de “amplo e fragmentado”, mas evitaria atribuir um TAM financeiro sem uma pesquisa específica sobre número de professores e ticket médio de softwares desse segmento.

Rio de Janeiro

O município do Rio de Janeiro tinha 6.211.223 habitantes no Censo 2022.

Além disso, a rede municipal projetava 645.746 matrículas para 2025, considerando suas diferentes Coordenadorias Regionais de Educação.

Isso não representa todo o mercado educacional carioca — faltam, entre outros, rede estadual, federal e privada — mas demonstra a escala relevante da demanda educacional local.

Para o AulaFácil, o Rio pode funcionar como um mercado inicial geograficamente concentrado:

Rio de Janeiro → Zona Norte/Zona Sul → Grande Tijuca → Tijuca

Essa estratégia é interessante porque permite validar o produto em uma região pequena antes de tentar atender professores de todo o Brasil.

Tijuca

Aqui temos um dado particularmente interessante.

O Censo 2022 registrou 142.909 habitantes na Tijuca, colocando o bairro entre os dez mais populosos do Brasil.

E existe evidência prática de uma oferta significativa de serviços de aulas particulares na região. Uma busca local encontrou diversos negócios especializados em aulas particulares, reforço escolar e acompanhamento pedagógico na Tijuca e arredores, incluindo PenseBem Aulas Particulares, Professora Mariana Tavares | Aula Particular de Matemática, Física e Química, Então Bia - Reforço Escolar/Aulas Particulares - Tijuca e Estudos & Cia.

Isso não prova o tamanho do mercado do software, mas é uma evidência interessante de que existe uma atividade econômica local suficientemente concreta para servir como ambiente inicial de validação.

Uma maneira mais rigorosa de apresentar o mercado

Para o trabalho do curso, eu colocaria:

TAM — Brasil: professores particulares e pequenos negócios de educação que precisam administrar alunos, agenda e recebimentos.

SAM — Rio de Janeiro: professores particulares independentes e pequenos centros de reforço da cidade.

SOM — Tijuca e bairros adjacentes: primeiros professores independentes de Matemática, Física e reforço escolar que adotarem a ferramenta.

Isso é mais defensável do que inventar um número de milhões de reais.

3. Business Model Canvas — AulaFácil
Bloco	AulaFácil
Segmentos de clientes	Professores particulares; professores autônomos; pequenos centros de reforço; inicialmente Matemática, Física e reforço escolar
Proposta de valor	Centralizar alunos, agenda, histórico de aulas e pagamentos em uma ferramenta simples e barata
Canais	Instagram, indicação entre professores, grupos/comunidades de professores, demonstração direta e landing page
Relacionamento com clientes	Autoatendimento + onboarding simples + suporte digital
Fontes de receita	Assinatura mensal; plano gratuito limitado; plano pago com mais alunos/aulas
Recursos-chave	Aplicação web, banco de dados, infraestrutura cloud, marca e base de usuários
Atividades-chave	Desenvolvimento, manutenção, aquisição de professores e melhoria do produto
Parcerias-chave	Comunidades de professores, profissionais de educação, escolas/centros de reforço e possíveis parceiros de divulgação
Estrutura de custos	Hospedagem, banco de dados, domínio, ferramentas de desenvolvimento, aquisição de clientes e suporte
Modelo de monetização que eu testaria

Para o MVP, não implementaria pagamentos online.

Faria algo extremamente simples:

Plano Gratuito

até 5 alunos;
agenda;
histórico básico.

Plano Pro

alunos ilimitados;
controle financeiro;
histórico completo;
relatórios.

Isso permite testar a disposição de pagar sem gastar créditos do Lovable construindo uma integração de pagamentos.

4. Hipóteses que o MVP precisa testar

Esta é, na minha opinião, a parte mais importante para o seu desafio.

Um MVP não deveria tentar provar que “o aplicativo funciona”. Isso é relativamente fácil.

Ele precisa testar se existe um problema relevante e se as pessoas querem a solução.

Hipótese 1 — O problema existe

Professores particulares têm dificuldade para organizar alunos, aulas e pagamentos utilizando ferramentas genéricas.

Como testar: conversar com 10–15 professores e perguntar como fazem atualmente.

Indicador: pelo menos metade relatar problemas recorrentes de organização.

Hipótese 2 — Existe disposição para centralizar essas informações

Professores consideram útil ter alunos + agenda + histórico + pagamentos em um único sistema.

Teste: apresentar o protótipo para professores e observar quais funcionalidades eles consideram realmente úteis.

Indicador: a maioria indicar pelo menos duas ou três funcionalidades como relevantes para sua rotina.

Hipótese 3 — O produto é suficientemente simples

Um professor consegue começar a utilizar o AulaFácil sem treinamento.

Teste: entregar o MVP a alguns professores e pedir que cadastrem um aluno, uma aula e um pagamento sem explicação detalhada.

Indicadores:

tempo para completar o primeiro cadastro;
erros cometidos;
necessidade de suporte.
Hipótese 4 — O dashboard resolve uma dor real

Ter uma visão imediata de aulas, alunos e pagamentos pendentes economiza tempo e reduz esquecimentos.

Teste: comparar a rotina atual do professor com a utilização do dashboard.

Indicador: percepção de economia de tempo/maior controle.

Hipótese 5 — Professores aceitariam pagar

Essa é crucial.

Um grupo de professores estaria disposto a pagar uma pequena assinatura mensal pelo serviço.

Não precisamos descobrir o preço perfeito no primeiro MVP.

Podemos simplesmente testar:

“Você pagaria R$ X/mês por essa ferramenta?”

e, mais importante, observar se alguém realmente aceita avançar para um plano pago/piloto.

Hipótese 6 — O nicho inicial é suficientemente específico

Começar por professores de Matemática, Física e reforço escolar é mais eficiente do que tentar atender todos os professores.

Isso é importante porque um produto para “todo professor” tende a ficar genérico demais.

No seu caso, há uma oportunidade particularmente interessante de começar pelo universo que você conhece: professores particulares de Matemática e Física.

Hipótese 7 — A aquisição pode acontecer por indicação

Professores satisfeitos indicariam o AulaFácil para outros professores.

Teste: disponibilizar o MVP para os primeiros usuários e perguntar se indicariam a ferramenta a colegas.

Posteriormente isso poderia virar uma funcionalidade de indicação.


MVP preparando o mega prompt

O MVP passa a validar apenas a proposta de valor e o fluxo de uso, sem gastar créditos e tempo com login, cadastro, recuperação de senha ou controle de usuários.

Abaixo está a estrutura revisada, mantendo o restante da proposta.

1. Arquitetura do MVP

O AulaFácil MVP terá 5 telas principais.

#	Tela	Função principal
1	Dashboard	Visão geral da atividade
2	Alunos	Cadastro e acompanhamento
3	Agenda	Visualização e criação das aulas
4	Aula / Registro	Registrar o que aconteceu na aula
5	Financeiro	Controlar valores pagos e pendentes

Não haverá tela de login.

Ao abrir o aplicativo, o usuário será levado diretamente ao Dashboard, utilizando dados de demonstração previamente cadastrados.

Isso também é interessante para a apresentação do curso: o avaliador abre o aplicativo e imediatamente consegue enxergar o produto funcionando.

2. Tela 1 — Dashboard

Esta será a tela inicial do AulaFácil.

A ideia é que o professor consiga abrir o sistema pela manhã e entender sua situação em poucos segundos.

Cabeçalho

Olá, Professor!

Aqui está o resumo da sua atividade.

Cards

Alunos ativos

12

Aulas hoje

3

A receber

R$ 850,00

Aulas este mês

28

Os números devem ser calculados a partir dos dados cadastrados, e não informações estáticas.

Seção: Próximas aulas

Tabela/lista:

Horário	Aluno	Disciplina	Status
09:00	João	Matemática	Agendada
14:00	Maria	Física	Agendada
17:00	Pedro	Matemática	Agendada

Cada aula pode ter um botão:

Ver aula

Seção: Pagamentos pendentes

Exemplo:

João Silva — R$ 150,00 — vencimento 05/10

Maria Souza — R$ 200,00 — vencimento 01/10

Botão:

Ver financeiro

Ações rápidas

Três botões:

+ Novo aluno

+ Nova aula

+ Registrar pagamento

3. Tela 2 — Alunos

Aqui teremos o CRUD principal dos alunos.

Cabeçalho

Meus alunos

Botão:

+ Novo aluno

Campo:

🔍 Buscar aluno

Filtro:

Todos
Ativos
Inativos
Cadastro de aluno

Ao clicar em + Novo aluno, abrir um modal.

Dados pessoais
Nome completo
Telefone
E-mail
Data de nascimento — opcional
Dados acadêmicos
Escola — opcional
Série/ano
Disciplina principal
Matemática
Física
Matemática e Física
Outra
Dados da aula
Valor padrão da aula
Duração padrão
Observações

Botões:

Cancelar

Salvar aluno

4. Detalhes do aluno — painel lateral

Não criaremos uma sexta tela.

Ao clicar em um aluno, abre-se um painel lateral/modal.

Exemplo:

João Silva
Matemática — 1º ano EM

Informações
Telefone
E-mail
Escola
Série
Valor da aula
Resumo

Aulas realizadas: 8

Aulas futuras: 3

Total recebido: R$ 1.200

Pendente: R$ 150

Histórico
Data	Disciplina	Conteúdo
02/10	Matemática	Função quadrática
25/09	Matemática	Equações
18/09	Matemática	Sistemas

Botões:

+ Agendar aula

Editar aluno

5. Tela 3 — Agenda

Será uma das telas mais utilizadas.

Para manter o MVP simples, não precisamos de um calendário sofisticado.

Cabeçalho

Minha agenda

Botão:

+ Nova aula

Seletor:

Hoje | Semana

Navegação:

< Semana anterior | Semana atual | Próxima semana >

Lista de aulas
Segunda-feira — 05/10

09:00 – 10:00

João Silva
Matemática

Agendada

14:00 – 15:00

Maria Souza
Física

Agendada

Ações

Ao clicar na aula:

Ver detalhes
Editar
Cancelar
Registrar aula
6. Modal "Nova aula"

Não será uma nova tela.

Campos

Aluno

Dropdown com alunos cadastrados.

Data

Date picker.

Horário de início

Time picker.

Duração

30 min
60 min
90 min
120 min

Disciplina

Matemática
Física
Outra

Valor

Preenchido automaticamente com o valor padrão do aluno, mas editável.

Observações

Campo de texto opcional.

Botão

Agendar aula

7. Tela 4 — Aula / Registro

Essa tela transforma a agenda em histórico pedagógico.

Quando uma aula estiver marcada como realizada, o professor poderá registrar o que aconteceu.

Cabeçalho

Registrar aula

Aluno: João Silva
Data: 05/10/2026
Horário: 09:00–10:00
Disciplina: Matemática

Campos

Status

Realizada
Cancelada
Não realizada

Conteúdo trabalhado

Campo de texto.

Exemplo:

Função quadrática: raízes e vértice.

Observações

Campo maior.

Exemplo:

Aluno apresentou dificuldade na interpretação do gráfico.

Tarefa para próxima aula

Campo opcional.

Botões

Salvar registro

Salvar e marcar como realizada

Regra importante

Ao marcar a aula como Realizada, o sistema deverá:

registrar a aula no histórico do aluno;
contabilizá-la no Dashboard;
atualizar o financeiro, caso exista valor associado;
mantê-la disponível no histórico.

Assim temos uma integração real entre as funcionalidades do MVP.

8. Tela 5 — Financeiro

O objetivo será apenas oferecer controle financeiro básico.

Não queremos construir um sistema contábil.

Cards

Recebido este mês

R$ 2.450

A receber

R$ 650

Aulas realizadas

28

Lista financeira
Data	Aluno	Aula	Valor	Status
02/10	João	Matemática	R$150	Pago
03/10	Maria	Física	R$180	Pendente
04/10	Pedro	Matemática	R$150	Pago

Filtros:

Todos
Pagos
Pendentes
Registrar pagamento

Botão:

+ Registrar pagamento

Modal:

Aluno

Aula

Valor

Data do pagamento

Forma de pagamento

Pix
Dinheiro
Transferência
Outro

Botão:

Registrar pagamento

9. Fluxo principal do aplicativo

Com a retirada do Login, o fluxo fica ainda mais simples:

                    ┌─────────────────┐
                    │    DASHBOARD    │
                    └───┬────┬────┬───┘
                        │    │    │
               ┌────────┘    │    └─────────┐
               ▼             ▼              ▼
          ┌──────────┐  ┌──────────┐  ┌────────────┐
          │  ALUNOS  │  │  AGENDA  │  │ FINANCEIRO │
          └────┬─────┘  └────┬─────┘  └────────────┘
               │             │
               ▼             ▼
         ┌───────────┐  ┌────────────┐
         │  DETALHES │  │ NOVA AULA  │
         │ DO ALUNO  │  └─────┬──────┘
         └───────────┘        │
                              ▼
                       ┌──────────────┐
                       │  REGISTRAR   │
                       │     AULA     │
                       └──────┬───────┘
                              │
                              ▼
                       HISTÓRICO DO ALUNO
                              +
                          FINANCEIRO

O fluxo principal fica:

Dashboard → Aluno → Aula → Registro → Financeiro

10. Modelo de dados mínimo

Como não teremos autenticação, podemos simplificar ainda mais o banco.

Precisaremos basicamente de três entidades.

students
id
name
phone
email
birth_date
school
grade
subject
default_lesson_price
default_duration
notes
active
created_at
lessons
id
student_id
date
start_time
duration
subject
price
status
content
notes
homework
created_at
payments
id
student_id
lesson_id
amount
payment_date
payment_method
status
created_at

Relacionamento:

ALUNOS
   │
   └── AULAS
          │
          └── PAGAMENTOS

Não precisamos de user_id neste MVP, pois estamos deliberadamente simulando um único professor/usuário.

Essa simplificação é importante: quando o produto evoluir para SaaS real, poderemos acrescentar autenticação e isolamento dos dados por usuário.

11. Navegação

Eu manteria um menu lateral fixo no desktop:

AulaFácil

🏠 Dashboard
👥 Alunos
📅 Agenda
💰 Financeiro

Na parte inferior:

Professor

Por enquanto, não precisamos sequer criar uma área de configurações.

O nome do professor pode simplesmente ser exibido no cabeçalho.

12. Identidade visual

Para evitar consumo desnecessário de créditos, eu manteria o design relativamente simples.

Direção

Estilo: moderno, limpo, profissional e amigável.

Público: professores particulares independentes.

Sensação: organização + simplicidade + confiança.

Cores
Fundo claro;
azul como cor principal;
azul escuro para títulos;
verde para situações positivas/pagamentos;
amarelo discreto para pendências;
vermelho apenas para cancelamentos/erros.
Interface
Cards simples;
bordas levemente arredondadas;
bastante espaço em branco;
tipografia sans-serif;
ícones simples;
responsividade para desktop e tablet.

Sem animações sofisticadas.

13. O que NÃO entra no MVP

Essa parte deverá aparecer explicitamente no Mega Prompt.

O AulaFácil não terá nesta primeira versão:

Login;
Cadastro de usuários;
Controle de múltiplos professores;
WhatsApp;
Google Calendar;
Google Meet;
Stripe;
Mercado Pago;
Pix automático;
emissão de nota fiscal;
IA;
notificações por e-mail;
notificações push;
aplicativo mobile nativo;
área do aluno;
marketplace;
chat;
relatórios avançados;
gráficos complexos;
integrações externas.

Isso deixa claro para o Lovable que estamos construindo um protótipo funcional de validação, e não a versão comercial definitiva.

14. Fluxo de demonstração do MVP

Para a apresentação do curso, eu faria uma demonstração de aproximadamente 3 minutos.

① Dashboard

O aplicativo abre diretamente no Dashboard:

12 alunos
3 aulas hoje
R$ 850 a receber

② Cadastrar aluno

Criamos:

João Silva
Matemática
R$ 150/aula

③ Agendar aula

Agendamos:

João — Matemática — segunda, 09h

④ Registrar aula

Simulamos a realização:

Função quadrática
Dificuldade na interpretação do gráfico.

⑤ Financeiro

O sistema mostra:

R$ 150 — Pendente

Depois:

Registrar pagamento → Pix → R$150

⑥ Dashboard

Voltamos ao Dashboard e mostramos que os indicadores foram atualizados.

Assim, o avaliador vê imediatamente o ciclo:

Aluno → Aula → Registro → Pagamento → Dashboard

15. O que estamos realmente validando

Com essa versão, o objetivo do MVP fica muito mais claro.

Não estamos tentando provar:

"Conseguimos construir um software de gestão."

Isso seria uma conclusão muito fraca.

Estamos tentando testar:

"Professores particulares percebem valor em centralizar sua rotina de alunos, aulas e pagamentos em uma única ferramenta simples?"

O MVP precisa, portanto, ser funcional o suficiente para simular essa experiência, mas deliberadamente pequeno.


# MEGA PROMPT — AULAFÁCIL MVP

## 1. CONTEXTO DO PRODUTO

Crie um MVP funcional de uma aplicação web chamada **AulaFácil**.

O AulaFácil é uma ferramenta simples de gestão para **professores particulares independentes**, inicialmente direcionada a professores de Matemática, Física e reforço escolar.

O objetivo do produto é centralizar em um único lugar quatro aspectos básicos da rotina do professor:

* cadastro e acompanhamento de alunos;
* organização das aulas;
* registro do conteúdo trabalhado;
* controle financeiro básico.

O problema que o produto pretende resolver é a utilização de várias ferramentas diferentes — WhatsApp, agenda do celular, planilhas, cadernos e memória — para administrar a atividade profissional.

A proposta de valor do AulaFácil é:

> **"Organize seus alunos, aulas e pagamentos em um único lugar, de forma simples e rápida."**

Este projeto é um **MVP para validação de conceito**, e não uma versão definitiva de um SaaS comercial.

Priorize simplicidade, clareza, funcionalidade e facilidade de demonstração.

---

# 2. OBJETIVO DESTA PRIMEIRA VERSÃO

O MVP deve permitir demonstrar o seguinte fluxo completo:

**Aluno → Aula → Registro da aula → Pagamento → Dashboard**

O sistema deve permitir que o usuário:

1. visualize o resumo de sua atividade;
2. cadastre alunos;
3. consulte informações e histórico de alunos;
4. agende aulas;
5. registre o conteúdo e observações de uma aula;
6. registre pagamentos;
7. acompanhe os principais indicadores da atividade.

O aplicativo deve abrir diretamente no **Dashboard**.

---

# 3. IMPORTANTE — NÃO IMPLEMENTAR AUTENTICAÇÃO

Nesta versão do MVP:

* NÃO criar tela de login;
* NÃO criar cadastro de usuário;
* NÃO criar recuperação de senha;
* NÃO criar autenticação;
* NÃO criar múltiplos perfis;
* NÃO criar permissões de usuários;
* NÃO criar isolamento de dados por usuário.

O aplicativo deverá funcionar como se houvesse **um único professor utilizando o sistema**.

O nome do professor exibido na interface pode ser:

**Prof. Antonio Carlos**

Essa simplificação é deliberada e faz parte do escopo do MVP.

---

# 4. ESCOPO FUNCIONAL

O aplicativo deverá possuir exatamente **5 áreas principais**:

1. Dashboard
2. Alunos
3. Agenda
4. Registro de Aula
5. Financeiro

O Dashboard será a tela inicial.

Utilize navegação lateral fixa no desktop.

Menu:

* Dashboard
* Alunos
* Agenda
* Financeiro

Não criar páginas adicionais desnecessárias.

Detalhes de alunos e criação de aulas/pagamentos devem utilizar **modais ou painéis laterais** sempre que isso simplificar a interface.

---

# 5. TELA 1 — DASHBOARD

## Objetivo

Fornecer ao professor uma visão rápida de sua atividade.

Título:

**Olá, Prof. Antonio Carlos!**

Subtítulo:

**Aqui está o resumo da sua atividade.**

## Cards principais

Criar quatro cards:

### Alunos ativos

Mostrar a quantidade atual de alunos ativos.

### Aulas hoje

Mostrar a quantidade de aulas agendadas para o dia atual.

### A receber

Mostrar o valor total de pagamentos pendentes.

### Aulas este mês

Mostrar a quantidade de aulas realizadas ou agendadas no mês atual, conforme a lógica definida no sistema.

Os números devem ser calculados dinamicamente a partir dos dados existentes.

NÃO utilizar números fixos nos cards.

---

## Seção "Próximas aulas"

Mostrar uma lista ou tabela contendo as próximas aulas.

Colunas:

* horário;
* aluno;
* disciplina;
* status.

Exemplo:

| Horário | Aluno          | Disciplina | Status   |
| ------- | -------------- | ---------- | -------- |
| 09:00   | João Silva     | Matemática | Agendada |
| 14:00   | Maria Souza    | Física     | Agendada |
| 17:00   | Pedro Oliveira | Matemática | Agendada |

Cada registro deve possuir ação:

**Ver aula**

---

## Seção "Pagamentos pendentes"

Mostrar os pagamentos ainda não registrados como pagos.

Informações:

* aluno;
* valor;
* data da aula ou vencimento;
* status.

Adicionar botão:

**Ver financeiro**

Esse botão deve levar à tela Financeiro.

---

## Seção "Ações rápidas"

Criar três botões:

* **+ Novo aluno**
* **+ Nova aula**
* **+ Registrar pagamento**

Cada botão deve abrir o respectivo modal.

---

# 6. TELA 2 — ALUNOS

## Objetivo

Permitir cadastrar e administrar os alunos.

Título:

**Meus alunos**

Adicionar botão:

**+ Novo aluno**

Adicionar campo de busca:

**Buscar aluno...**

Adicionar filtros:

* Todos
* Ativos
* Inativos

---

## Lista de alunos

Mostrar os alunos em tabela ou cards responsivos.

Informações mínimas:

* nome;
* disciplina;
* série;
* telefone;
* status;
* valor padrão da aula.

Cada aluno deve possuir ações:

* Visualizar
* Editar
* Ativar/desativar

---

# 7. MODAL — NOVO ALUNO

Ao clicar em **+ Novo aluno**, abrir um modal.

## Dados pessoais

Campos:

* Nome completo — obrigatório
* Telefone
* E-mail
* Data de nascimento — opcional

## Dados acadêmicos

Campos:

* Escola — opcional
* Série/ano
* Disciplina principal

Opções de disciplina:

* Matemática
* Física
* Matemática e Física
* Outra

## Dados da aula

Campos:

* Valor padrão da aula
* Duração padrão

Opções de duração:

* 30 minutos
* 60 minutos
* 90 minutos
* 120 minutos

Campo:

* Observações

Botões:

**Cancelar**

**Salvar aluno**

Validar os campos obrigatórios.

Após salvar, atualizar imediatamente a lista de alunos e os indicadores relevantes do Dashboard.

---

# 8. PAINEL LATERAL — DETALHES DO ALUNO

Não criar uma nova página.

Ao clicar em um aluno, abrir um painel lateral ou modal de detalhes.

Mostrar:

## Identificação

* Nome
* Disciplina
* Série
* Status

## Informações

* Telefone
* E-mail
* Escola
* Valor padrão da aula
* Duração padrão

## Resumo

Mostrar dinamicamente:

* aulas realizadas;
* próximas aulas;
* total recebido;
* valor pendente.

## Histórico de aulas

Mostrar:

* data;
* disciplina;
* conteúdo;
* status.

Exemplo:

| Data  | Disciplina | Conteúdo          |
| ----- | ---------- | ----------------- |
| 02/10 | Matemática | Função quadrática |
| 25/09 | Matemática | Equações          |
| 18/09 | Matemática | Sistemas          |

Adicionar botões:

**+ Agendar aula**

**Editar aluno**

---

# 9. TELA 3 — AGENDA

## Objetivo

Permitir organizar as aulas.

Título:

**Minha agenda**

Botão:

**+ Nova aula**

Criar seletor simples:

* Hoje
* Semana

Criar navegação:

* Semana anterior
* Semana atual
* Próxima semana

Não é necessário criar um calendário complexo semelhante ao Google Calendar.

Priorizar uma visualização simples e funcional.

---

## Lista de aulas

Organizar as aulas cronologicamente por dia.

Cada aula deve mostrar:

* horário;
* aluno;
* disciplina;
* duração;
* valor;
* status.

Status possíveis:

* Agendada
* Realizada
* Cancelada
* Não realizada

Ao selecionar uma aula, oferecer:

* Ver detalhes
* Editar
* Cancelar
* Registrar aula

---

# 10. MODAL — NOVA AULA

Ao clicar em **+ Nova aula**, abrir modal.

Campos:

### Aluno

Dropdown com os alunos cadastrados.

Obrigatório.

### Data

Date picker.

Obrigatório.

### Horário de início

Time picker.

Obrigatório.

### Duração

Opções:

* 30 minutos
* 60 minutos
* 90 minutos
* 120 minutos

Preencher inicialmente com a duração padrão do aluno selecionado.

### Disciplina

Opções:

* Matemática
* Física
* Outra

Preencher automaticamente, quando possível, com a disciplina principal do aluno.

### Valor

Preencher automaticamente com o valor padrão da aula do aluno.

Permitir edição manual.

### Observações

Campo de texto opcional.

Botões:

**Cancelar**

**Agendar aula**

Após salvar, atualizar a Agenda e os indicadores do Dashboard.

---

# 11. TELA 4 — REGISTRO DE AULA

Esta tela será utilizada para registrar o resultado de uma aula.

Título:

**Registrar aula**

Mostrar no topo:

* aluno;
* data;
* horário;
* disciplina;
* valor.

## Status

Opções:

* Realizada
* Cancelada
* Não realizada

## Conteúdo trabalhado

Campo de texto.

Exemplo:

> Função quadrática: raízes, vértice e interpretação do gráfico.

## Observações

Campo de texto maior.

Exemplo:

> O aluno apresentou dificuldade na interpretação gráfica.

## Tarefa para próxima aula

Campo opcional.

Exemplo:

> Resolver exercícios 1 a 5 da lista.

Botões:

**Cancelar**

**Salvar registro**

**Salvar e marcar como realizada**

---

# 12. REGRA DE NEGÓCIO — AULA REALIZADA

Quando uma aula for marcada como **Realizada**:

1. atualizar o status da aula;
2. registrar o conteúdo;
3. registrar as observações;
4. registrar a tarefa, se houver;
5. disponibilizar a aula no histórico do aluno;
6. atualizar os indicadores do Dashboard;
7. disponibilizar o valor da aula para controle financeiro;
8. manter o registro permanentemente associado ao aluno.

Não duplicar registros quando o usuário editar uma aula existente.

---

# 13. TELA 5 — FINANCEIRO

## Objetivo

Fornecer um controle financeiro básico das aulas.

Título:

**Financeiro**

## Cards

### Recebido este mês

Somatório dos pagamentos realizados no mês atual.

### A receber

Somatório dos pagamentos pendentes.

### Aulas realizadas

Quantidade de aulas realizadas no período.

Os valores devem ser calculados dinamicamente.

---

## Lista financeira

Mostrar:

* data;
* aluno;
* aula;
* valor;
* status.

Exemplo:

| Data  | Aluno | Aula       |  Valor | Status   |
| ----- | ----- | ---------- | -----: | -------- |
| 02/10 | João  | Matemática | R$ 150 | Pago     |
| 03/10 | Maria | Física     | R$ 180 | Pendente |
| 04/10 | Pedro | Matemática | R$ 150 | Pago     |

Filtros:

* Todos
* Pagos
* Pendentes

---

# 14. MODAL — REGISTRAR PAGAMENTO

Ao clicar em:

**+ Registrar pagamento**

abrir modal.

Campos:

### Aluno

Dropdown.

### Aula

Dropdown ou seleção da aula pendente correspondente ao aluno.

### Valor

Preencher automaticamente com o valor da aula.

Permitir edição.

### Data do pagamento

Preencher inicialmente com a data atual.

### Forma de pagamento

Opções:

* Pix
* Dinheiro
* Transferência
* Outro

### Status

* Pago
* Pendente

Botão:

**Registrar pagamento**

Após registrar:

* atualizar a lista financeira;
* atualizar o Dashboard;
* atualizar o painel do aluno.

---

# 15. MODELO DE DADOS

Criar uma estrutura de dados simples.

## Entidade `students`

Campos:

* id
* name
* phone
* email
* birth_date
* school
* grade
* subject
* default_lesson_price
* default_duration
* notes
* active
* created_at

---

## Entidade `lessons`

Campos:

* id
* student_id
* date
* start_time
* duration
* subject
* price
* status
* content
* notes
* homework
* created_at

Relacionamento:

`lessons.student_id → students.id`

---

## Entidade `payments`

Campos:

* id
* student_id
* lesson_id
* amount
* payment_date
* payment_method
* status
* created_at

Relacionamentos:

`payments.student_id → students.id`

`payments.lesson_id → lessons.id`

---

# 16. REGRAS DE INTEGRIDADE

Garantir que:

* uma aula sempre esteja associada a um aluno;
* um pagamento, quando relacionado a uma aula, esteja associado à respectiva aula;
* excluir um aluno não produza dados órfãos;
* valores financeiros sejam armazenados numericamente;
* datas sejam armazenadas de forma consistente;
* aulas possam ser editadas sem criar duplicatas;
* pagamentos possam ser atualizados;
* o status das aulas seja claramente identificado;
* o status dos pagamentos seja claramente identificado.

Antes de excluir dados, pedir confirmação ao usuário.

---

# 17. DADOS FICTÍCIOS PARA DEMONSTRAÇÃO

O aplicativo deve iniciar com uma pequena quantidade de **dados fictícios pré-carregados**.

Esses dados existem exclusivamente para permitir uma demonstração imediata do MVP.

Criar pelo menos **5 alunos fictícios**.

Sugestão:

### João Silva

* Disciplina: Matemática
* Série: 1º ano do Ensino Médio
* Valor: R$ 150
* Duração: 60 minutos

### Maria Souza

* Disciplina: Física
* Série: 2º ano do Ensino Médio
* Valor: R$ 180
* Duração: 60 minutos

### Pedro Oliveira

* Disciplina: Matemática
* Série: 9º ano
* Valor: R$ 130
* Duração: 60 minutos

### Ana Costa

* Disciplina: Matemática e Física
* Série: 3º ano do Ensino Médio
* Valor: R$ 200
* Duração: 90 minutos

### Lucas Martins

* Disciplina: Física
* Série: 2º ano do Ensino Médio
* Valor: R$ 170
* Duração: 60 minutos

Criar também várias aulas fictícias distribuídas entre:

* aulas futuras;
* aulas realizadas;
* aulas canceladas.

Criar registros de aulas realizadas contendo:

* conteúdo;
* observações;
* tarefa para próxima aula.

Criar também pagamentos fictícios:

* alguns pagos;
* alguns pendentes.

Os dados devem ser coerentes entre si.

Por exemplo:

Uma aula realizada de João Silva no valor de R$ 150 pode ter um pagamento de R$ 150 associado.

Uma aula realizada de Maria Souza no valor de R$ 180 pode permanecer pendente.

---

# 18. IMPORTANTE SOBRE OS DADOS DE DEMONSTRAÇÃO

Os dados fictícios devem funcionar exatamente como dados reais.

O usuário deve conseguir:

* editar;
* excluir;
* adicionar novos alunos;
* adicionar novas aulas;
* alterar status;
* registrar novos pagamentos.

Os números do Dashboard devem mudar automaticamente conforme os dados forem modificados.

NÃO criar uma interface meramente estática.

---

# 19. ESTADO INICIAL DO DASHBOARD

Ao abrir o aplicativo pela primeira vez, o Dashboard deve estar preenchido com os dados fictícios.

Mostrar indicadores coerentes.

Por exemplo:

* 5 alunos ativos;
* algumas aulas futuras;
* algumas aulas realizadas;
* alguns pagamentos pendentes;
* valor recebido;
* valor a receber.

Os valores exatos podem ser calculados automaticamente com base nos dados fictícios.

Não inserir números fixos no código apenas para preencher os cards.

---

# 20. NAVEGAÇÃO

Utilizar um menu lateral no desktop.

Logo/nome:

**AulaFácil**

Itens:

* Dashboard
* Alunos
* Agenda
* Financeiro

Na parte inferior:

**Prof. Antonio Carlos**

Não criar configurações complexas.

O item Dashboard deve ser a página inicial.

---

# 21. RESPONSIVIDADE

A aplicação deve funcionar adequadamente em:

* desktop;
* notebook;
* tablet.

Priorizar inicialmente a experiência desktop, pois o MVP será principalmente demonstrado em computador.

Em telas menores:

* transformar o menu lateral em menu compacto;
* reorganizar os cards;
* transformar tabelas em listas/cards quando necessário;
* garantir que formulários permaneçam utilizáveis.

Não é necessário desenvolver aplicativo mobile nativo.

---

# 22. IDENTIDADE VISUAL

Criar uma interface:

* moderna;
* limpa;
* profissional;
* amigável;
* minimalista.

O público é formado por professores particulares.

A sensação visual desejada é:

**organização + simplicidade + confiança.**

---

## Paleta

Utilizar:

* fundo predominantemente claro;
* azul como cor principal;
* azul escuro para títulos;
* verde para estados positivos e pagamentos realizados;
* amarelo discreto para pendências;
* vermelho apenas para erros, exclusões ou cancelamentos.

Evitar excesso de cores.

---

## Tipografia

Utilizar uma fonte sans-serif moderna e legível.

Priorizar:

* excelente legibilidade;
* hierarquia visual clara;
* títulos destacados;
* textos secundários discretos.

---

## Componentes

Utilizar:

* cards;
* tabelas simples;
* badges de status;
* botões claros;
* inputs;
* dropdowns;
* modais;
* painéis laterais;
* ícones simples.

Usar bordas levemente arredondadas.

Utilizar espaço em branco suficiente.

Não utilizar efeitos visuais exagerados.

Não utilizar animações complexas.

---

# 23. ESTADOS DA INTERFACE

Criar estados adequados para:

### Lista vazia

Exemplo:

> Nenhum aluno cadastrado.

Botão:

**Adicionar primeiro aluno**

### Busca sem resultado

> Nenhum aluno encontrado.

### Agenda vazia

> Nenhuma aula agendada para este período.

### Financeiro sem registros

> Nenhum lançamento financeiro encontrado.

### Confirmações

Após salvar:

> Aluno cadastrado com sucesso.

Após agendar:

> Aula agendada com sucesso.

Após registrar pagamento:

> Pagamento registrado com sucesso.

Após registrar aula:

> Aula registrada com sucesso.

---

# 24. VALIDAÇÃO DOS FORMULÁRIOS

Validar campos obrigatórios.

Mostrar mensagens de erro claras e próximas ao campo.

Exemplos:

> Informe o nome do aluno.

> Selecione uma data.

> Informe o valor da aula.

Não permitir salvar registros obviamente inválidos.

---

# 25. EXPERIÊNCIA DO USUÁRIO

A aplicação deve privilegiar:

* poucos cliques;
* formulários curtos;
* informações relevantes;
* ações claras;
* feedback imediato;
* navegação previsível.

Um professor sem treinamento técnico deve conseguir entender o aplicativo rapidamente.

Evitar menus escondidos e fluxos desnecessariamente complexos.

---

# 26. ESCOPO EXPLICITAMENTE EXCLUÍDO

NÃO implementar nesta versão:

* autenticação;
* login;
* cadastro de usuários;
* múltiplos professores;
* permissões;
* WhatsApp;
* integração com WhatsApp;
* Google Calendar;
* Google Meet;
* Zoom;
* Stripe;
* Mercado Pago;
* processamento de Pix;
* emissão de nota fiscal;
* integração bancária;
* IA;
* chatbot;
* notificações por e-mail;
* notificações push;
* SMS;
* aplicativo mobile nativo;
* área do aluno;
* área dos pais;
* marketplace;
* chat;
* videoconferência;
* relatórios financeiros avançados;
* gráficos complexos;
* exportação para Excel;
* integração com serviços externos;
* funcionalidades de CRM;
* campanhas de marketing.

Se uma funcionalidade não for necessária para demonstrar o fluxo principal do MVP, **não implementá-la**.

---

# 27. PRINCÍPIO FUNDAMENTAL DE DESENVOLVIMENTO

Este projeto é um **MVP de validação**.

Não tentar antecipar funcionalidades da versão comercial.

Priorizar:

1. funcionamento;
2. simplicidade;
3. consistência dos dados;
4. boa experiência de usuário;
5. facilidade de demonstração;
6. baixo nível de complexidade.

Não adicionar funcionalidades apenas porque elas poderiam ser úteis no futuro.

---

# 28. FLUXO PRINCIPAL A SER VALIDADO

O sistema deve permitir demonstrar claramente:

### Etapa 1

Visualizar o Dashboard.

### Etapa 2

Cadastrar um aluno.

### Etapa 3

Agendar uma aula para esse aluno.

### Etapa 4

Registrar a aula realizada.

### Etapa 5

Visualizar essa aula no histórico do aluno.

### Etapa 6

Ver o valor correspondente no Financeiro.

### Etapa 7

Registrar o pagamento.

### Etapa 8

Retornar ao Dashboard e observar os indicadores atualizados.

Esse fluxo deve funcionar de ponta a ponta.

---

# 29. CRITÉRIOS DE ACEITAÇÃO DO MVP

Considerar o MVP concluído quando for possível:

* abrir o aplicativo diretamente no Dashboard;
* visualizar dados fictícios;
* criar um novo aluno;
* editar um aluno;
* visualizar detalhes de um aluno;
* agendar uma aula;
* editar uma aula;
* cancelar uma aula;
* registrar uma aula realizada;
* visualizar o histórico do aluno;
* registrar um pagamento;
* visualizar pagamentos pendentes;
* visualizar pagamentos realizados;
* observar os indicadores do Dashboard sendo atualizados;
* navegar entre as cinco áreas principais;
* utilizar a aplicação em desktop e tablet.

---

# 30. RESTRIÇÃO FINAL — NÃO EXPANDIR O ESCOPO

É fundamental que o desenvolvimento permaneça limitado ao escopo descrito neste documento.

**Não criar novas páginas, módulos ou integrações sem necessidade.**

Quando houver mais de uma maneira de implementar determinada funcionalidade, escolher a solução:

* mais simples;
* mais estável;
* mais fácil de manter;
* mais fácil de demonstrar;
* com menor complexidade.

O objetivo é entregar um **MVP funcional, visualmente profissional e pequeno**, adequado para validação de uma ideia de negócio.

Não transformar o AulaFácil em uma plataforma completa de gestão educacional nesta etapa.

---

# RESULTADO ESPERADO

Ao final, entregar uma aplicação web funcional chamada:

# AulaFácil

Com:

* Dashboard;
* Alunos;
* Agenda;
* Registro de Aula;
* Financeiro;

dados fictícios pré-carregados;

CRUD funcional;

indicadores dinâmicos;

relacionamentos entre alunos, aulas e pagamentos;

interface responsiva;

design moderno e minimalista;

e fluxo completo:

**ALUNO → AULA → REGISTRO → PAGAMENTO → DASHBOARD**

O produto deve parecer um **MVP real pronto para ser demonstrado a potenciais usuários**, mas permanecer deliberadamente simples para permitir validação rápida da proposta.

** Ao lançar o mega prompt no Lovable, meus 5 créditos se foram. App pausado. Amanhã eu volto. **
