# YouTube Bulk Uploader CLI 🚀

## Portuguese version:

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![YouTube API v3](https://img.shields.io/badge/YouTube%20API-v3-red.svg)](https://developers.google.com/youtube/v3)

Ferramenta CLI em Python para upload em massa de vídeos no YouTube, organizando automaticamente em playlists com base na estrutura de pastas.

## Funcionalidades Principais
- **Upload em Lote** de centenas de vídeos de uma vez
- **Organização Automática** em playlists por pastas
- **Metadados Inteligentes** extraídos de nomes de arquivos (ex: `1.0_Título.mp4`)
- **Resiliência** com retentativas e controle de cotas da API
- **Logs Detalhados** para auditoria e troubleshooting

## Como Usar
1. **Instalação**:
   ```bash
   git clone https://github.com/antonioreverso/youtube-bulk-uploader.git
   pip install -r requirements.txt
   ```

2. **Configuração**:
   - Crie credenciais OAuth 2.0 no [Google Cloud Console](https://console.cloud.google.com/)
   - Renomeie `config.example.yaml` para `config.yaml` e ajuste as configurações

3. **Execução**:
   ```bash
   python cli.py --path /caminho/da/pasta --category Education --default_tags "tutorial,python"
   ```

## Estrutura do Projeto
```
youtube_uploader/
├── cli.py            # Interface de linha de comando
├── api_client.py     # Conexão com YouTube API
├── file_manager.py   # Leitura de pastas e metadados
├── uploader.py       # Lógica de upload/resiliência
└── logs/             # Registros de execução
```

## Tecnologias-Chave
- **YouTube Data API v3** para integração oficial
- **google-api-python-client** para autenticação e uploads
- **asyncio** para processamento paralelo seguro
- **pathlib** para gestão de caminhos multiplataforma


## English version:

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![YouTube API v3](https://img.shields.io/badge/YouTube%20API-v3-red.svg)](https://developers.google.com/youtube/v3)

A Python CLI tool for bulk uploading videos to YouTube, automatically organizing them into playlists based on folder structure.



## Key Features
- **Bulk Upload** hundreds of videos at once
- **Automatic Organization** into playlists by folders
- **Smart Metadata** extracted from filenames (e.g., `1.0_Title.mp4`)
- **Resilience** with retries and API quota control
- **Detailed Logs** for auditing and troubleshooting

## How to Use
1. **Installation**:
   ```bash
   git clone https://github.com/antonioreverso/youtube-bulk-uploader.git
   pip install -r requirements.txt
   ```

2. **Configuration**:
   - Create OAuth 2.0 credentials in the [Google Cloud Console](https://console.cloud.google.com/)
   - Rename `config.example.yaml` to `config.yaml` and adjust the settings

3. **Execution**:
   ```bash
   python cli.py --path /path/to/folder --category Education --default_tags "tutorial,python"
   ```

## Project Structure
```
youtube_uploader/
├── cli.py            # Command-line interface
├── api_client.py     # YouTube API connection
├── file_manager.py   # Folder and metadata reading
├── uploader.py       # Upload and resilience logic
└── logs/             # Execution logs
```

## Key Technologies
- **YouTube Data API v3** for official integration
- **google-api-python-client** for authentication and uploads
- **asyncio** for safe parallel processing
- **pathlib** for cross-platform path management




