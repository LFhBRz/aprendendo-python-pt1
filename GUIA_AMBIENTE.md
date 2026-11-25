# Preparar o ambiente (uma vez só)

1. Instale o Python em python.org (Windows). Na primeira tela, MARQUE "Add python.exe to PATH".
2. Abra esta pasta no VS Code (File > Open Folder).
3. Abra o terminal do VS Code (Ctrl + ') e crie o ambiente virtual:
       python -m venv .venv
4. Ative o ambiente (Windows, PowerShell):
       .venv\Scripts\Activate.ps1
   Se o PowerShell bloquear scripts, rode uma vez:
       Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
   (ou use o Prompt de Comando e rode  .venv\Scripts\activate.bat)
5. Instale as bibliotecas:
       pip install -r requirements.txt
6. Abra analise_entregaja.ipynb. No canto superior direito, "Select Kernel" > Python Environments > .venv
7. Teste: rode a primeira célula de código. Se não der erro, está pronto.

Dica: .venv/ já está no .gitignore do projeto anterior. Nunca suba essa pasta para o GitHub.
