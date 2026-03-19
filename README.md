# Windows Backup Automation

Script em PowerShell para automação de backup em ambientes Windows, com foco em simplicidade, confiabilidade e uso corporativo.

## 🚀 Funcionalidades

- Backup automatizado de diretórios locais
- Cópia para servidor de rede (SMB)
- Criação de pastas com timestamp
- Logs detalhados de execução
- Tratamento de erros (ex: servidor indisponível)
- Execução via Agendador de Tarefas

## 🛠️ Tecnologias utilizadas

- PowerShell
- Robocopy
- Windows Task Scheduler

## 📂 Estrutura

- `backup.ps1` → Script principal
- `logs/` → Registro das execuções
- `backup/` → Destino dos backups

## ⚙️ Como funciona

O script realiza a cópia incremental utilizando Robocopy, garantindo eficiência e evitando duplicação desnecessária de arquivos.

## 🎯 Objetivo

Demonstrar automação de rotinas administrativas em ambientes Windows, simulando cenários reais de infraestrutura de TI.

## 🔒 Boas práticas aplicadas

- Logging estruturado
- Validação de destino
- Controle de falhas
- Organização por data
