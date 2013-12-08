<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão 1.4
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
| 02/12/2013 | 1.2 | Segunda Versão | Stanislaw Cruz |
| 03/12/2013 | 1.3 |Terceira Versão | Fco. Chagas M  |
| 07/12/2013 | 1.4 |Quarta Versão | Stanislaw Cruz  |
| 08/12/2013 | 1.5 |Quinta Versão | Euclides Brasil  |



1. Introdução
==============

Este artefato descreve as atividades relacionadas ao Gerenciamento de Controle 
de Configuração e Mudança que serão executadas durante o ciclo de vida do produto. 
As atividades aqui descritas envolvem a identificação da configuração do software, manter sua integridade durante o projeto e controlar sistematicamente as mudanças assim como os responsáveis pelas mesmas.


1.1 Finalidade
---------------
O objetivo deste documento é definir um padrão para que os membros da equipe possam garantir o controle do produto desenvolvido. 
Serão detalhados alguns recursos como (equipes, ferramentas e computadores), que consideramos necessário para alcançarmos nossos objetivos.


1.2 Escopo
----------
Este Plano de Gerenciamento de Configuração tem como objetivo iterar toda a equipe do projeto Sinergia de modo que todos os interessados tenham ciência do processo utilizado. Este documento é restrito aos membros do projeto.
Este documento deverá acompanhar as mudanças ocorridas ao longo do projeto devendo ser atualizado constantemente e versionado.


1.3 Definições, Acrônimos e Abreviações
---------------------------------------


|Termo                |Significado |
|--------------------|-------------|------------------------|---------------|
|GC|Gerência de Configuração|
|CCM|Comitê para o Controle de Mudanças|
|BUG|Erro no funcionamento comum de um software|
|SM|Solicitação de Mudança|


1.4 Referências
---------------
N/A

1.5 Visão Geral
---------------
As próximas seções deste documento foram definidas da seguinte maneira.

Seção 2.0 São definidas os papeis e responsabilidades das atividades e as ferramentas

Seção 3.0 São relacionados os papéis, as responsabilidades das atividades e as ferramentas dentro da GC da Fábrica,  além  mostrar serão criadas e controladas as Baselines.

Seçao 4.0 Serão abordados os detalhes sobre quando o Plano de Gerenciamento de Configuração deve ser atualizado.

Seçao 5.0 Descreve ferramentas de software, o pessoal e o treinamento necessário para programar as atividades de CM especificadas.

Seçao 6.0 Descreve de que forma o software desenvolvido fora do ambiente do projeto será incorporado.

2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------

|Papeis                |Equipe       |Responsabilidade |
|--------------------|-------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
|Gerente de Configuração|Francisco das Chagas|Definir Plano de GC aplicar Políticas de GC, criar e adaptar o ambiente de GC, criar Baselines promover baselines
CCM|Stanislaw Cruz Euclides Brasil Francisco das Chagas|Elaborar Processo de Controle de Mudanças Revisar Solicitação de Mudança|
Desenvolvedor|Stanislaw Euclides Brasil|Seguir os padrões, procedimentos e Ferramentas definidos no Plano de Gerência de Configuração.|
|Todos os Papéis|Euclides Brasil Stanislaw Cruz Francisco das Chagas|Enviar Solicitação de Mudança e Atualizar Solicitação de Mudança|

2.2 Ferramentas, Ambiente e Infra-estrutura
----------------------------------------------------------------
2.2.1 	As ferramentas a serem utilizadas para a gerência de configuração

|Ferrmanta                |Descrição | versão 
|--------------------|-------------|----------------------------
|Git Hub	Controle de Versão|Sistema de controle de versão|1.8.4
|Jira |Controle de Mudanças |6.0|
|Jenkis| Integração contínua|   |
|IBM Quality Center	|Testes e Controle de Qualidade	Ferramenta usada para Elaboração dos Casos de Testes|2008

2.2.2	Configuração do software – Ferramentas do ambiente de desenvolvimento

|Tipo                |Ferramenta | versão 
|--------------------|-------------|----------------------------
|Sistema Operacional (Desenvolvimento)|Windows 7 Professional|1.8.4
|Cronograma |Microsoft Word |2012|
|Controle de Versão |GitHub|1.8.4|
|Banco de Dados |SQL Server 2008 |10.0.160|
|Plataforma de Desenvolvimento|Eclipse|SR2|
|Navegador|Chrome|31.0.1650

2.2.3	Configuração das maquinas dos ambientes

|Quantidade|Ambiente   |Configuração | Software    | 
-----------|-----------|-------------|----------------------------
|2|Desenvolvedor|Processador: 2.3 GHz Memória RAM: 4GB Hard Disk:500 GB|Windows 7 Eclipse Microsoft Office 2012 SQL Server 2008 10.0.160
|1|Integração|Processador: 2.3 GHz Memória RAM: 4GB Hard Disk: 500 GB|Windows 7 Eclipse Microsoft Office 2012 SQL Server 2008 10.0.160
|1|Banco de Dados|Processador: 2.3 GHz Memória RAM: 4 RAM Hard Disk: 500 GB|Windows7

3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
Todos os artefatos versionados no projetos, devem ter uma nomenclatura intuita e incremental, a fim de facilitar alguma consulta, comparativo histórico etc.

Desta forma, foi criado um padrão geral para os artefatos (Salve os códigos fontes). A nomeclatura será:

[COD]-[ID]-[NOME_PROJETO]-[TEXTO_LIVRE].[EST] 
 

Onde:
* [COD] = Código do projeto
* [ID] = Identificador do tipo de documento 
* [NOME_PROJETO] = Nome do projeto, neste caso, Sinergia
* [TEXTO_LIVRE] = Alguma descrição que forneça uma identificação escrita do arquivo (Ex: nome do caso de uso, nome da diagrama de classe etc)
* [EST] = Extensão do arquivo

Para identificador de tipo de documento temos:
* UC	Caso de uso
* EUC	Especificação de caso de uso
* RNG	Regra de negócio
* GLS	Glossário
* BLD	Identifica que é uma Build a ser publicada


Exemplo: S001-UC-Sinergia-ManterCliente.doc – Modelo de caso de uso de manter cliente do sistema 001 - Sinergia



### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	   | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|S001-BLD-Sinergia-Requisitos001.build|Fco. Chagas|Ao término do levantamento de Requisitos|
|S001-BLD-Sinergia-Codigo001.build|Euclides Brasil|Ao término dos testes|
|S001-BLD-Sinergia-Implanatacao001.build|Stanislaw da Cruz|Versão a ser publicada em produção|


### 3.1.3 Baselines do Projeto

As baselines do projeto serão classificadas da seguinte forma:

Requisitos (casos de uso, documentação, design do projeto e validação).

Código Fonte, modelo de dados, especificação de testes e diagramas UML.


### 3.1.4 Estrutura do Repositório de Versões

O projeto deverá ser dividido em pastas, onde em cada pasta, deverá conter as sub-pastas e arquivos referentes.

De uma forma geral, os projetos deverão ter a seguinte estrutura de pastas:

* Requisitos - Requisitos, Termo de Abertura do Projeto, Documento de Visão, Diagramas de Caso de Uso, Especificação de Caso de Uso, Realização do Caso de Uso.
* Outros - Atas de Reunião, Termo de Aceite do Cliente, Contagem UCP.
* Aplicação - Codigos Fonte do sistema, Binarios, DLLs
* A & P - Diagrama de Classe, Diagrama de Sequencia, Diagrama de Atividade, Diagrama de Estado.
* Implantação - Plano de implantação, Nota de Liberação, Lista de Materiais.
* Modelos - Modelo de Dados, Templates
* Testes - Plano de teste, Caso de teste
* Builds -  Todas as builds de código e requisitos

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
_[Descreva o processo pelo qual os problemas e as mudanças são submetidos, revisados e dispostos. Inclua como funciona a transição de estados de uma solicitação de mudança]_

### 3.2.2 Comitê de Controle de Mudança (CCB)
São líderes de equipe que, através de reuniões diárias, verificam todas as solicitações e separam o que vai para o fluxo de trabalho e o que vai para o backlog.



4. Padrões e Procedimentos
==========================
4.1 - Padrões de estrutura lógica

* Requisitos:	Requisitos, Termo de Abertura do Projeto, Documento de Visão, Diagramas de Caso de Uso, Especificação de Caso de Uso, Realização do Caso de Uso.
* Outros:	Atas de Reunião, Termo de Aceite do Cliente, Contagem UCP.
* Aplicação:	Codigos Fonte do sistema, Binarios, DLLs
* A & P:	Diagrama de Classe, Diagrama de Sequencia, Diagrama de Atividade, Diagrama de Estado.
* Implantação:	Plano de implantação, Nota de Liberação, Lista de Materiais.
* Modelos:	Modelo de Dados, Templates.
* Testes:	Plano de teste, Caso de teste



5. Treinamento e Recursos
=========================
Toda os membros da equipe deverão participar dos respectivos treinamento abaixo, haja vista que boa parte da equipe ainda não domina ou possui habilidades com essas ferramentas e controle de versão distribuidos.Esse item se justifica pois a equipe já comentou sobre dificuldade (Antes era utilizado o SVN).

|Treinamento         |Objetivo | Envolvidos 
|--------------------|-------------|----------------------------
|GitHub (Desenvolvimento)|Será efetuado um treinamento do uso do Github em Windows 7 visando mostrar os principais comandos executados via shell. |Toda a equipe|
|Treinamento JIRA |Será realizado um treinamento na Ferramenta JIRA mostrando como funciona o Workflow da ferramenta.|Toda a equipe|
|Treinamento em QC |Será efetuado um treinamento no IBM QUality Center a fim de mostrar como utilizar a ferramenta para criação de casos de testes. |Toda a equipe|


A fim de manter a padronização d código e da forma de trabalho no versionamento, será proposto 2 treinamentos

* 1 : Ferramenta controle de Versão e Atividades
* 2 : Treinamento em Cody Analyse, Style Cop e Source Monitor.

6. Auditorias de Configuração
=============================
Serão realizadas auditorias de configuração para cada etapa dos processos de desenvolvimento de software (Elicitação de requisitos, desenvolvimento, testes, implantação do sistema etc).
Visando melhorar o processo, reuniões periodicas devem ser feitas para identificar erros e propor melhorias. Essas observações devem ser registradas e versionadas para acompnahemnto futuro.

