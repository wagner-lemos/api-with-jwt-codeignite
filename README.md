### Integração de API REST com JWT - CodeIgniter 4.5
APIs REST para web com estrutura baseada em tokens como JWT usando PHP e CodeIgniter. Seu objetivo é permitir que você desenvolva APIs muito mais rapidamente do que se estivesse escrevendo código do zero, fornecendo um template para seu trabalho com a API REST com tokens baseados em JWT

#### Recursos
```
1. Controle completo da API REST
2. Tokens de acesso baseados em JWT
3. Operações CRUD
4. Mecanismo de Registro/Login/Regeneração de Token
5. Autenticação adequada
6; Controle de validação
7. Roteamento tratado
```
#### Requisitos
```
• Versao do PHP: 8.2
• Versao do CodeIgniter: 4.5.1
```
#### Instalação
• Clone o projeto;<br/>
• Configure o **.env** e adapte para o sua aplicação;<br/>
• Instale as dependências: **composer install**;<br/>
• Execute a migrate **php spark migrate** para criar as tabelas;

#### Configura o JWT
• Crie suas próprias chaves públicas e privadas e substitua-as pelas chaves de código de serviço em **app/Config/Services.php**:<br/>
```
openssl genpkey -algorithm RSA -out private_key.pem -aes256
openssl rsa -pubout -in private_key.pem -out public_key.pem
```
• Altere **JWT_SECRET_KEY** e **JWT_TIME_TO_LIVE** conforme necessário;<br/>
• Abra o Insomnia e importe **insomnia_endpoints.json**;

> [!IMPORTANT]
> Inicialmente, o access_token foi configurado para 60 minutos.

> [!WARNING]
> "JWT_SECRET_KEY" deve ser alterado para sua própria proteção no ambiente de produção.

---
Você pode me encontrar via [Linkedin](https://www.linkedin.com/in/wagnerlemos).