# Repositório para estudo das ferramentas 

## IAM
 -  Um dos serviços mais importantes da AWS, este serviço é responsável por dar acesso ao controle de permissões para todos os serviços,
 criação de usuários, grupos e funções. 
 - é um serviço global para todas as regiões
 - usuários criados (exeto o root) não possuem permissões, as mesma dever ser atribuidas.

- A autenticação em multifatores MFA traz maior segurança ao acesso a conta root do IAM, ela pode ser feita de 3 modos:
    1. Virtual MFA (MFA virtual)
    2. U2F - a security key (uma chave de sergurança)
    3. Other hardware MFA device ( outro dispositivo de hardware MFA)

- Criação de um usuário:
    1. nome do usuário 
    2. tipo de acesso do usuário:
        - acesso programático: é gerada um id de chave de acesso e a chave de acesso secreta
        - acesso ao console de gerenciamento AWS: é gerada automáticamente ou a mão uma senha que pode ou não ser alterada no primeiro acesso
        
        `Obs.: é obrigatório dar ao menos um dos tipos de acesso ao usuário`
    3. adicionar ou criar um grupo
        - o grupo deve conter as policies que o usuário precisa
    4. concluir a criação do usuário 
    5. baixar o csv com as informações do usuário ou enviar por e-mail.

-  Criação de um grupo:
    1. Nome do grupo 
    2. adicionar as permissões (policies) que aquele grupo
   
    `Obs.: Policies são permissões que serão atribuídas a usuários, grupos e aplicações`
   
    3. concluir a criação do grupo.

- password policies
    - ajuste das politicas de senha dos usuário:
        1. quantidade mínima de caracteres 
        2. uma letra maiúscula pelo menos 
        3. uma letra minúscula pelo menos 
        4. um número pelo menos 
        5. um caracter alfa-númerico pelo menos 
        6. habilitar período de expiração da senha 
            - quantidade dias para a senha expirar (padrão 90 dias ou 3 meses)
        7. expiração de senha requer uma redefinição do admin
        8. permitir que usuários alterem a própria senha 
        9. impedir reutilização de senha
            - quantidade de senha a serem lembradas (padrão as 5 últimas)