LoggerSetup Class
Descrição
A classe LoggerSetup é uma ferramenta para configuração e uso de logs em Python. Ela permite que você configure o local de armazenamento dos logs, o nome do arquivo de log, o nome do logger, além de facilitar a criação de mensagens de log em diferentes níveis (DEBUG, INFO, ERROR, WARNING).

Funcionalidades
Configuração básica de logs: A classe permite configurar logs de forma simples, com suporte para formatação e manipulação de arquivos.
Mensagens de Log: Métodos para logar mensagens em diferentes níveis: debug, info, warning e error.
Como Utilizar
Instalação
Certifique-se de que as bibliotecas logging, sys, e os estejam instaladas. Essas bibliotecas são nativas do Python, então você não precisa instalar pacotes adicionais.

Exemplo de Uso
python
Copiar código
from logger_setup import LoggerSetup

# Configurar o logger
logger = LoggerSetup(pathLog='/caminho/para/logs/', nameLog='meu_log.log', nameLogger='meu_logger')

# Criar mensagens de log em diferentes níveis
logger.debugMessage('Esta é uma mensagem de debug', 'debug')
logger.infoMessage('Esta é uma mensagem de info', 'info')
logger.warningMessage('Esta é uma mensagem de aviso', 'warning')
logger.errorMessage('Esta é uma mensagem de erro', 'error')
Explicação dos Parâmetros
pathLog: Caminho onde o arquivo de log será armazenado.
nameLog: Nome do arquivo de log.
nameLogger: Nome do logger, que será usado internamente para identificar o log.
Métodos Disponíveis
debugMessage(message, level): Registra uma mensagem de nível DEBUG.
infoMessage(message, level): Registra uma mensagem de nível INFO.
warningMessage(message, level): Registra uma mensagem de nível WARNING.
errorMessage(message, level): Registra uma mensagem de nível ERROR.
Requisitos
Python 3.x
Módulos: logging, sys, os
