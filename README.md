# Biblioteca

📚 SGB-Console (Sistema de Gerenciamento de Biblioteca)
O SGB-Console é uma aplicação desenvolvida em Python que simula o funcionamento do balcão de atendimento de uma biblioteca. O sistema integra lógica de programação, manipulação de banco de dados SQL e uma interface amigável via terminal para gerenciar empréstimos, devoluções e multas de alunos.

🚀 Funcionalidades
O sistema foi estruturado para oferecer um fluxo completo de atendimento:

Autenticação de Usuário: Sistema de login seguro validando RA e senha no banco de dados.

Consulta de Acervo: Busca inteligente por Título, Autor ou Área, armazenando resultados em listas para exibição organizada.

Gestão de Empréstimos: Verificação de disponibilidade de títulos e geração automática de protocolos de atendimento.

Devolução com Cálculo de Multa: Sistema que detecta atrasos, calcula valores diários e aplica arredondamentos financeiros.

Módulo Financeiro: Consulta e quitação de débitos pendentes no cadastro do aluno.

🛠️ Tecnologias e Conceitos Aplicados
Este projeto demonstra o uso prático de:

Python 3: Linguagem base do sistema.

SQLite3: Banco de dados relacional para persistência de dados.

Tratamento de Exceções: Uso de blocos try/except para garantir que o sistema não encerre abruptamente em caso de entradas inválidas.

Modularização: Código organizado em funções para facilitar a manutenção e leitura.

Bibliotecas Nativas:

math: Utilizada para o arredondamento de taxas financeiras (ceil).

random: Utilizada para a geração de protocolos numéricos aleatórios.

SQL (DML/DDL): Criação de tabelas, relacionamentos com chaves estrangeiras (Foreign Keys), consultas complexas e atualizações de registros.

📂 Estrutura do Banco de Dados
O banco de dados é composto por três tabelas principais:

aluno: Armazena dados cadastrais e saldo devedor.

livros: Gerencia o catálogo e o status de disponibilidade (Disponível/Emprestado).

emprestimo: Relaciona alunos e livros de forma dinâmica.

⚙️ Como Executar
Certifique-se de ter o Python 3.x instalado.

Clone este repositório:

Bash
git clone https://github.com/seu-usuario/sgb-console.git
Navegue até a pasta do projeto e execute o arquivo principal:

Bash
python biblioteca.py
O banco de dados biblioteca.db será criado automaticamente na primeira execução (caso utilize o script de inicialização).
