# Repositório para estudo das ferramentas 

## IAM
 -  Um dos serviços mais importantes da AWS, este serviço é responsável por dar acesso ao controle de permissões para todos os serviços,
 criação de usuários, grupos e funções. 

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

    