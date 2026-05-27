# SQL-para-Profissionais-de-Prevenção-a-Fraudes-
SQL para Profissionais de Prevenção a Fraudes (do zero ao avançado, com casos reais)
Estudando...

Exercícios:

Qual é a data de validade do cartão da Caixa Econômica da usuária Ana Julia Teixeira? (user_id: 7536)

select 
  * 
from 
fraud.user_creditcards uc
where
user_id = 7536

/*Resultado: 04/05*/
<img width="1835" height="875" alt="image" src="https://github.com/user-attachments/assets/b164539a-6e37-4209-9535-4c022017986f" />
