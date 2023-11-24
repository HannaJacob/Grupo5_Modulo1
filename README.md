# Resilia - Modernização do Gerenciamento de Estrutura de Ensino
 <p align="center">  <img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge"/>
</p>

Este script SQL foi desenvolvido como parte do esforço de modernização da Resilia, com o objetivo de aprimorar o armazenamento e a gestão de dados relacionados à estrutura de ensino da empresa. O código cria um banco de dados denominado "Resilia" e define tabelas essenciais para organizar informações sobre cursos, turmas, alunos, módulos, disciplinas, turnos, facilitadores e boletins.

A estrutura do banco de dados busca superar os desafios associados ao armazenamento disperso de dados em planilhas, proporcionando uma base consolidada e eficiente para a extração de informações estratégicas. Além disso, o script inclui um gatilho que registra automaticamente mudanças de status dos alunos, contribuindo para uma trilha de auditoria completa.

Este projeto visa facilitar a administração e análise de dados acadêmicos dentro da Resilia, contribuindo para uma gestão mais eficaz e informada da estrutura educacional da empresa.

## 🔨 Funcionalidades
- `Funcionalidade 1` `Criação do Banco de Dados e Tabelas`:
  
Define um banco de dados chamado "Resilia".

Cria tabelas para armazenar informações sobre cursos, turmas, alunos, módulos, disciplinas, turnos, facilitadores, boletins e logs de status.

- `Funcionalidade 2` `Inserção de Dados de Exemplo`:

Popula as tabelas com dados de exemplo, fornecendo um ponto de partida para utilização e testes.

- `Funcionalidade 3` `Gatilho para Registro de Mudanças de Status`:

Implementa um gatilho chamado AtualizacaoStatus que é acionado automaticamente após uma atualização na tabela Aluno.

O gatilho registra informações como o ID do aluno, status antigo, novo status e a data da mudança na tabela LogStatus.

Fornece uma trilha de auditoria para acompanhar as mudanças nos status dos alunos ao longo do tempo.

- `Funcionalidade 4` `Consultas Exemplo`:

Apresenta consultas SQL de exemplo para realizar operações específicas:

1 - Identificar alunos aprovados em uma turma específica.

2 - Encontrar facilitadores associados a mais de uma turma.

- `Funcionalidade 5` `Visualizações (Views)`:

Cria uma visualização chamada EvasaoPorTurma que calcula o percentual de evasão por turma.
 
- `Funcionalidade 6` `Configurações Adicionais`:

Utiliza o delimitador // para definir o final do comando em determinadas partes do script, especialmente para a correta criação do gatilho (AtualizacaoStatus).

## ✔️ Técnicas e tecnologias utilizadas 

- ``MySQL``

