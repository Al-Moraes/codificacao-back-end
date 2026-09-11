Aula 02 — Módulos CommonJS e ESM

Projeto desenvolvido para praticar o uso de módulos ES Modules (ESM) no Node.js, trabalhando também com módulos nativos para criação e manipulação de arquivos.

📚 Conteúdos praticados
Utilização de import e export
Configuração do "type": "module" no package.json
Utilização do módulo fs/promises
Utilização do módulo path
Utilização do módulo url
Operações assíncronas com async/await
Tratamento de erros com try/catch
Criação de arquivos e diretórios
Registro de logs com data e hora
⚙️ Funcionamento

O projeto possui uma função responsável por formatar as mensagens de log, adicionando a data e o horário atual:

export function formatLog(mensagem) {
    const dataAtual = new Date().toISOString().split('T')[0];
    const horaAtual = new Date().toLocaleTimeString();

    return `[${dataAtual} ${horaAtual}] - ${mensagem}`;
}


A função salvarLogSystem() cria automaticamente a pasta logs, caso ela ainda não exista, e adiciona as mensagens ao arquivo system.log.

logs/
└── system.log

📁 Estrutura do projeto
aula02-modulos-commonjs-esm/
├── index.js
├── utils.js
├── package.json
└── logs/
    └── system.log

🚀 Como executar

Clone o projeto ou baixe os arquivos e execute:

node index.js


Após a execução, as mensagens serão registradas no arquivo:

logs/system.log

📝 Exemplo de log
[2026-09-11 16:35:20] - Inicialização do Servidor Concluído!
[2026-09-11 16:35:20] - Conexão com o Banco de Dados Estabelecida!

🎯 Objetivo

O objetivo deste exercício é compreender como funciona a organização de código utilizando ES Modules no Node.js, além de praticar operações de arquivos e diretórios de forma assíncrona.
