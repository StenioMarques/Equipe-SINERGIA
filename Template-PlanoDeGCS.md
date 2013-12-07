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
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|Hardware    |Stanislaw Cruz    |_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|
|Software    |Euclides Brasil   |_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|
|Documentação    |Stenio Marques   |_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto

As baselines do projeto serão classificadas da seguinte forma:

Requisitos (casos de uso, documentação, design do projeto e validação).

Código Fonte, modelo de dados, especificação de testes e diagramas UML.


### 3.1.4 Estrutura do Repositório de Versões
O repositório é composto de diretórios aos quais são identificados pelo nome do projeto, esse por sua vez possui sub-diretórios que seguem a seguinte nomenclatura:

* Apresentação
* Domínio
* Infraestrutura
* Serviço

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
_[Descreva o processo pelo qual os problemas e as mudanças são submetidos, revisados e dispostos. Inclua como funciona a transição de estados de uma solicitação de mudança]_

### 3.2.2 Comitê de Controle de Mudança (CCB)
São líderes de equipe que, através de reuniões diárias, verificam todas as solicitações e separam o que vai para o fluxo de trabalho e o que vai para o backlog.



4. Padrões e Procedimentos
==========================
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



5. Treinamento e Recursos
=========================
_[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]_



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
