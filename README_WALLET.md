# Wish Wallet
 Desafio Técnico Klever

## Objetivo

 Desenvolver uma carteira de crypto moedas aonde o usuário tenha autonomia no que diz respeito adicionar,editar e excluir suas cryptos.


## Tecnologias utilizadas

- HTML
- CSS
- JAVASCRIPT

## Bibliotecas Utilizadas

- BOOTSTRAP 5
- SWEET ALERT 2

## Problemas no Projeto

 Por questão de falta de conhecimento não pûde desenvolver 100% da aplicação,nesta aplicação é possível cadastrar apenas 1 token,segue os problemas que me deparei para o desenvolvimento:

- Tentei criar um array vazio aonde os valores do input eram colocados no final desse array a cada vez que o botão 'save' fosse clicado,no entanto não funcionou pois quando o usuário clica em 'save' ele automaticamente é redirecionado para a página inicial.Ao voltar para a página 'Add Token' e cadastrar um novo token esse mesmo substituía o token anterior no LocalStorage, oque fazia com que o meu array se tornasse inconsistente,logo a única maneira de fazer funcionar seria impedir que ao clicar no botão 'save' o usuário fosse redirecionado para a página inicial.

- Ao fazer dessa forma consegui ter um resultado interessante,conseguia cadastrar os tokens de maneira dinâmica,no entanto o maior problema foi que era necessário ter um botão de editar junto com esse token e eu não consegui editar esses tokens por suas posições como array.Isso se deu porque por algum motivo esse array vazio não era computado como um array no local storage,isso é ele não declarava as posições,por isso quando eu tentava editar um token a edição substituia todo aquele array,oque acabava deixando minha carteira novamente com apenas um token.

- Tentei converter esse array para 'JSON',funcionou mas o grande problema foi que ao usar o método 'getStorage' para fazer os tokens aparecerem na tela para usuário ele aparecia como um objeto mesmo,ou seja, não apareciam apenas os valores mas sim todo o conteúdo do localStorage na tela,inclusive as chaves e colchetes.Ao tentar declarar  '.value' fora dos parênteses do método 'setItem' e novamente tentar fazer um 'getItem', o valor aparecia como 'object',oque atrapalhou o andamento do projeto proposto.

- Por fim consegui apresentar pelo menos um token na tela,que me gerou um último problema, pois como eu não tenho outro token para comparar não consegui fazer um alert que mostrasse que o token já existe,portanto se o usuário adicionar um token de nome 'Rafael' e de balance 'Sousa' e logo após isso tentar criar um "novo" token de nome e balance iguais ele irá conseguir.

## Considerações

Gostaria de agradecer a toda equipe da [Klever](https://klever.io/) por estar me dando essa oportunidade de me desafiar,foi o projeto mais interessante que ja desenvolvi!
    

## Como Acessar o Projeto
### Basta clicar no link abaixo:

 GitHub Pages: https://rafap19.github.io/frontend-junior-test/


### Contato
Email: rafap.19@hotmail.com <br>
Linkedin: https://bit.ly/Linkedin_Rafael_Sousa <br>
