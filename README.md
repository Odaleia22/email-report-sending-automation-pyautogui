# Sales Report Email Automation

This project automates the process of downloading a sales report from Google Drive, reading the data from an Excel file, calculating key sales metrics, and sending a summary email through Gmail.

It uses Python libraries such as `pyautogui`, `pandas`, `openpyxl`, `zipfile`, and `pyperclip` to automate repetitive tasks and reduce manual work in business reporting.

## Objective

The main goal is to automate the steps of retrieving sales data, analyzing it, and sending a report email without manual intervention.

## Features

- Access to a shared Google Drive folder
- Download and extraction of ZIP files
- Reading sales data from Excel
- Calculation of total revenue and quantity sold
- Automatic Gmail email sending
- Time savings and increased productivity

## Technologies Used

- Python
- Pandas
- OpenPyXL
- PyAutoGUI
- Pyperclip

## How it works

1. The script opens the browser and accesses the configured Google Drive link.
2. It downloads the compressed sales file.
3. The ZIP file is extracted to a local folder.
4. The Excel data is read with Pandas.
5. Sales metrics are calculated.
6. Gmail is opened and the email is composed automatically.
7. The email is sent with the final report.

## Setup

Antes de executar o projeto, instale o Python 3 e crie um ambiente virtual para
manter as dependências isoladas do restante do sistema.

### Windows (PowerShell)

No terminal, estando na pasta do projeto, execute:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Quando o ambiente estiver ativo, o nome `.venv` aparecerá no início da linha do
terminal. A partir desse momento, execute o notebook `main.ipynb` usando o
interpretador Python do ambiente virtual.

Para sair do ambiente virtual, execute:

```powershell
deactivate
```

### Windows (Prompt de Comando)

```bat
python -m venv .venv
.venv\Scripts\activate.bat
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Se o PowerShell bloquear a ativação por política de execução, abra o terminal
como usuário e execute `Set-ExecutionPolicy -Scope Process -ExecutionPolicy
Bypass`; depois tente ativar o ambiente novamente.

## Notes

This project uses screen coordinates for browser automation, so adjustments may be necessary depending on screen resolution or browser layout.

## Project status

This is a practical automation example for sales reporting and email delivery.






