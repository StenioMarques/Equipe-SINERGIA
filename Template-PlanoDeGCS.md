<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão 1.2
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_02/12/2013_|_1.2_|_Segunda Versão_|_Stanislaw Cruz_|
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;autor&gt;_|



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
Termo	Significado
GC	Gerência de Configuração
CCM	Comitê para o Controle de Mudanças.
Baseline	Conjunto de itens de configuração que conseguiram um estado comprovado de estabilidade.
BUG	Erro no funcionamento comum de um software


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
_[Descreva quem será o responsável pela execução das diversas atividades de Gerenciamento de Configuração (CM) descritas no Processo de CM.]_

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
_[Descreva o ambiente de computação e as ferramentas de software a serem utilizadas para desempenhar as funções de CM em todo o ciclo de vida do projeto ou produto._
_Descreva as ferramentas e os procedimentos necessários utilizados para o controle de versão dos itens de configuração gerados no ciclo de vida do projeto ou produto._
_As questões envolvidas na configuração do ambiente de CM incluem:_
* _tamanho previsto dos dados do produto_
* _distribuição da equipe do produto_
* _localização física dos servidores e clientes]_
 


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
|_&lt;grupo de itens de configuração&gt;_|_&lt;nome do responsável&gt;_|_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto

_[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines._
_Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior._
_Descreva quem autoriza uma baseline e o que ela contém.]_

### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
_[Descreva o processo pelo qual os problemas e as mudanças são submetidos, revisados e dispostos. Inclua como funciona a transição de estados de uma solicitação de mudança]_

### 3.2.2 Comitê de Controle de Mudança (CCB)
_[Descreva a participação e os procedimentos para processar solicitações e aprovações de mudança a serem seguidos pelo CCB. Informe quem são os membros do CCB e suas responsabilidades.]_



4. Padrões e Procedimentos
==========================
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



5. Treinamento e Recursos
=========================
_[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]_



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
