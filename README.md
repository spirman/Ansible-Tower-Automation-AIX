🤖 TARS - Sistema Avançado de Automação e IA
https://img.shields.io/badge/Python-3.8+-blue.svg
https://img.shields.io/badge/License-MIT-green.svg
https://img.shields.io/badge/Status-Development-yellow.svg

TARS (Sistema Avançado de Reconhecimento e Suporte) é um assistente pessoal inteligente modular que combina automação, geração de código e capacidades de IA através de interface por voz e terminal.

🌟 Características Principais
🎤 Interface por Voz: Ativação por comando de voz com reconhecimento de fala

⌨️ Interface por Terminal: Comandos textuais para automação rápida

🤖 Múltiplos Módulos: Sistema modular extensível com diversas funcionalidades

🌐 Tempo Real: Informações meteorológicas em tempo real para qualquer cidade

💻 Geração de Código: Suporte a múltiplas linguagens de programação

🔧 Automação DevOps: Ansible, Docker, Cron e scripts de automação

📦 Módulos Disponíveis
📋 Módulo Base
hora - Hora e data atual

clima [cidade] - Tempo meteorológico em tempo real

sistema - Informações do sistema

wikipedia [tópico] - Busca na Wikipedia

screenshot - Captura de tela

ip - Informações de rede

🤖 Automação de Sistema
otimizar sistema - Limpeza e otimização

monitorar recursos - Monitoramento em tempo real

backup documentos - Backup automático

organizar desktop - Organização de arquivos

🌐 Automação Web
abrir email - Acesso rápido ao email

pesquisar google [termo] - Pesquisa no Google

download youtube [url] - Download de vídeos

monitorar site [url] - Monitoramento de websites

💻 Geração de Código
python [descrição] - Gera código Python

javascript [descrição] - Gera código JavaScript

html [descrição] - Gera HTML/CSS

sql [descrição] - Gera consultas SQL

bash [descrição] - Gera scripts Bash

🛠️ DevOps & Automação
ansible playbook [descrição] - Cria playbooks Ansible

cron job [descrição] - Gera entradas no crontab

docker compose [app] - Gera docker-compose.yml

script backup - Scripts de backup automático

🚀 Instalação
Pré-requisitos
bash
# Sistema Debian/Ubuntu
sudo apt update
sudo apt install python3-pip portaudio19-dev espeak espeak-data libespeak1 python3-pyaudio

# Instalar Ollama (para AI)
```sh
  curl -fsSL https://ollama.ai/install.sh | sh
  ollama pull qwen3:1.7b
  Instalação do TARS
   Clone o repositório
   ```

```sh
bash
git clone https://github.com/seu-usuario/TARS_Modular.git
cd TARS_Modular
Instale as dependências Python
  ```
```sh
bash
pip install -r requirements.txt
Configure as variáveis de ambiente
 ```
```sh
bash
cp .env.example .env
# Edite o arquivo .env com suas configurações
Configure a API do OpenWeather (opcional para clima)
```
Acesse: OpenWeatherMap

Crie uma conta gratuita e obtenha sua API key

Adicione no arquivo .env:

env
OPENWEATHER_API_KEY=sua_chave_aqui
🎯 Como Usar
Modo Terminal
bash
python3 main.py
# Escolha a opção 2 para modo terminal
Exemplos de Comandos
bash
# Consultar o tempo
clima Lisboa
clima Nova Iorque
clima Tóquio

# Gerar código
python criar uma calculadora
html criar página de login
ansible playbook deploy nginx

# Automação
otimizar sistema
monitorar recursos
backup documentos
Modo Voz
bash
python3 main.py
# Escolha a opção 1 para modo voz
# Diga "TARS" para ativar, depois seu comando
🏗️ Estrutura do Projeto
```sh
TARS_Modular/
├── main.py                 # Arquivo principal
├── config.py              # Configurações do sistema
├── requirements.txt       # Dependências Python
├── .env                  # Variáveis de ambiente
├── utils/                # Utilitários
│   ├── voice_utils.py    # Reconhecimento de voz
│   ├── system_utils.py   # Utilitários de sistema
│   ├── weather_utils.py  # API meteorológica
│   ├── file_utils.py     # Manipulação de arquivos
│   ├── network_utils.py  # Utilitários de rede
│   └── security_utils.py # Utilitários de segurança
└── modules/              # Módulos de funcionalidades
    ├── base_module.py    # Comandos básicos
    ├── system_module.py  # Automação de sistema
    ├── web_module.py     # Automação web
    ├── file_module.py    # Manipulação de arquivos
    ├── network_module.py # Automação de rede
    ├── code_module.py    # Geração de código
    ├── ai_module.py      # Automação de IA
    ├── security_module.py # Segurança
    ├── schedule_module.py # Agendamento
    ├── ansible_module.py # Ansible
    ├── cron_module.py    # Cron jobs
    ├── docker_module.py  # Docker
    ├── scripts_module.py # Scripts
    └── core_ai.py        # Núcleo de IA
```
🔧 Configuração
```sh
Arquivo .env
env
# API Keys
OPENWEATHER_API_KEY=sua_chave_openweather
```
# Configurações do Sistema
```sh
TRIGGER_WORD=tars
LLM_MODEL=qwen3:1.7b
```
# Configurações de Áudio
```sh
TTS_RATE=160
TTS_VOLUME=0.9
Personalização
```
Você pode personalizar o TARS editando:
Configurações gerais: config.py
Comandos de voz: utils/voice_utils.py
Novos módulos: modules/novo_modulo.py
Respostas personalizadas: Edite os métodos nos módulos

🐛 Solução de Problemas
Erro de Áudio
```sh
bash
# Se houver problemas com microfone:
sudo apt install portaudio19-dev python3-pyaudio
Erro de API Weather
```
```sh
bash
# Se o clima não funcionar:
# 1. Verifique se la API key está correta no .env
# 2. Teste a conexão com a API:
curl "http://api.openweathermap.org/data/2.5/weather?q=Lisbon&appid=sua_chave"
Problemas com Ollama
```
```sh
bash
# Verifique se o Ollama está rodando:
ollama serve
```
# Baixe o modelo correto:
```sh
ollama pull qwen3:1.7b
```
```sh
📋 Roadmap
✅ Interface modular completa
✅ Suporte a múltiplos idiomas
✅ Integração com APIs externas
🔄 Dashboard web integrado
🔄 Plugins e extensões
🔄 Integração com calendário
🔄 Reconhecimento de padrões
🔄 Aprendizado contínuo
🤝 Contribuindo
Contribuições são bem-vindas! Siga estos passos:
```
Fork o projeto

Crie uma branch para sua feature (git checkout -b feature/AmazingFeature)

Commit suas mudanças (git commit -m 'Add some AmazingFeature')

Push para a branch (git push origin feature/AmazingFeature)

Abra um Pull Request

📝 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para detalhes.

🙋‍♂️ Suporte
Se você encontrar problemas ou tiver dúvidas:

Verifique a seção de troubleshooting

Abra uma issue

Consulte a documentação (em desenvolvimento)

🎉 Agradecimentos
OpenWeatherMap por API meteorológica

Ollama por modelos de IA locais

SpeechRecognition por reconhecimento de voz

LangChain por framework de IA

TARS - Seu assistente pessoal inteligente para automação e produtividade! 🚀

"Interstellar reference intended" 🌌
