# Requisitos — Sistema de Login

## Uma aplicação possui uma tela de login com:

campo e-mail;

campo senha;

botão "Entrar".

## Regras:

O e-mail deve possuir formato válido.

A senha deve possuir no mínimo 8 caracteres.

Usuário e senha corretos permitem acesso ao sistema.

Usuário ou senha inválidos exibem a mensagem:

"Usuário ou senha inválidos".

Após 5 tentativas inválidas consecutivas, a conta deve ser bloqueada.

Campos obrigatórios não preenchidos devem exibir mensagens de validação.

## Casos de Teste

### Cenário: Login com sucesso

Dado que eu tenha o login e senha válidos
Quando eu inserir esses dados na área do login do sistema
Então o sistema deve realizar o login com sucesso

## Login com senha inválida

Dado que eu esteja na tela de login
Quando eu inserir o usuário correto e a senha com menos de 8 caracteres
E apertar no botão "Entrar"
Então o sistema deve mostrar a mensagem: "Usuário ou senha inválidos"

## Login com usuário inválido

Dado que eu esteja na tela do login
Quando eu inserir um e-mail inválido e a senha correta
E apertar no botão "Entrar"
Então o sistema deve mostrar a mensagem: "Usuário ou senha inválidos"

## Bloquear conta

Dado que eu esteja na tela de login
Quando eu inserir o usuário válido
E inserir a senha inválida
E apertar no botão "Entrar" 5 vezes consecutivas
Então a conta deve ser bloqueada

## Campos obrigatórios

Dado que eu esteja na tela de login
Quando eu aperto no botão "Entrar"
Então o sistema deve exibir uma mensagem de validação de campo não preenchido.