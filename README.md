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

/*Resultado: 04/2025*/
<img width="1835" height="875" alt="image" src="https://github.com/user-attachments/assets/b164539a-6e37-4209-9535-4c022017986f" />

//* 2-Qual é o user_id do usuário que se chama Augusto Ribeiro, possui email do gmail, 
  a conta foi criada em 2024 e que possuí dois cartões de crédito cadastrados?*//

SELECT *
FROM users u
WHERE u.name LIKE '%Augusto Ribeiro%'
and u.creation_date between '2024-01-01' and '2025-01-01'
and u.email like '%@gmail.com'

//* encontramos dois usuarios 7125 e 9253 *//

SELECT *
FROM fraud.user_creditcards uc
WHERE uc.user_id IN (7125, 9253);

<img width="1824" height="871" alt="image" src="https://github.com/user-attachments/assets/5f5cdec2-b4e0-42a9-99ab-fa9e3dca941b" />


