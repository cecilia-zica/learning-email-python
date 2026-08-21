# Motivação por e-mail em Python

Um script pequeno que envia um e-mail com uma frase motivacional aleatória nos
dias de semana. Foi um exercício para aprender a mandar e-mail com Python.

## Objetivo

Praticar o módulo `smtplib` (envio de e-mail por SMTP) junto com `datetime`
para checar o dia da semana e `random` para sortear a frase.

## Como funciona

- As frases ficam em `quotes.txt`, uma por linha.
- Se for dia útil (segunda a sexta), o `main.py` sorteia uma frase e envia por
  e-mail via SMTP do Gmail.

## Como rodar

O login não fica no código — ele é lido de variáveis de ambiente:

```sh
export MYEMAIL="seu-email@gmail.com"
export PASSWORD="sua-senha-de-app"
python main.py
```

Para o Gmail, use uma [senha de app](https://support.google.com/accounts/answer/185833),
não a senha normal da conta.
