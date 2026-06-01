# Exercício Prático 2 — Cadastro de Usuário

## Contexto

Você é QA de uma aplicação de streaming de filmes.

Foi criada uma funcionalidade de cadastro de usuário.

Seu trabalho é criar os cenários de teste em BDD com base nos requisitos abaixo.

# Requisitos da funcionalidade

## A tela de cadastro possui os seguintes campos:

Nome completo

E-mail

Data de nascimento

Senha

Confirmar senha

Botão "Cadastrar"

# Regras de negócio

## Nome completo

Deve ser obrigatório.

Deve possuir no mínimo 3 caracteres.

Não pode conter números.

## E-mail

Deve ser obrigatório.

Deve possuir formato válido.

Não pode existir outro usuário com o mesmo e-mail.

##  Data de nascimento

Usuário deve possuir no mínimo 18 anos para se cadastrar.

## Senha
Deve possuir:

mínimo de 8 caracteres;

pelo menos 1 letra maiúscula;

pelo menos 1 número.

## Confirmar senha

Deve ser igual ao campo senha.

## Cadastro

Cadastro realizado com sucesso deve:

criar usuário;

redirecionar para tela inicial;

exibir mensagem:

"Cadastro realizado com sucesso".

