# 💾 Windows Backup Automation

Script em PowerShell para automatizar backup de usuários no Windows.

## 🎯 Objetivo

Automatizar a cópia de dados críticos de usuários para um servidor de rede,
reduzindo falhas humanas e garantindo segurança dos dados.

## 🚀 Funcionalidades

- Backup automático da pasta C:\Users
- Armazenamento em servidor de rede
- Criação de logs
- Execução automatizada via agendador

## 📁 Estrutura

windows-backup-automation
│
├── scripts/
│   └── backup.ps1
│
├── logs/
│   └── backup.log

## ⚙️ Execução manual

powershell.exe -ExecutionPolicy Bypass -File scripts/backup.ps1

## ⏱️ Agendamento

schtasks /create /tn "BackupAutomatico" /tr "powershell.exe -ExecutionPolicy Bypass -File C:\Backup\scripts\backup.ps1" /sc daily /st 18:00

## 🛠️ Tecnologias

- PowerShell
- Robocopy
- Windows Task Scheduler

- ## 🔐 Boas práticas aplicadas

- Backup incremental
- Exclusão de diretórios desnecessários
- Logs detalhados
- Tratamento de erro
- Preparado para ambiente corporativo
