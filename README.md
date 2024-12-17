# Guia de Configuração do Projeto Acesso ao BI

### Requisitos do Projeto

Para rodar este projeto, certifique-se de ter os seguintes requisitos:

- PHP: Versão 8.1
- Composer: Versão 2.4.1
- Node.js: Versão 18.8.0
  - Pacotes:
    - `@tailwindcss/forms`: Versão ^0.5.2
    - `alpinejs`: Versão ^3.4.2
    - `autoprefixer`: Versão ^10.4.2
    - `axios`: Versão ^1.6.4
    - `laravel-vite-plugin`: Versão ^1.0.0
    - `postcss`: Versão ^8.4.31
    - `tailwindcss`: Versão ^3.1.0
    - `vite`: Versão ^5.0.0
- NPM: Versão 8.18.0
- DBeaver: Versão 24.1.5

### Dependências do Projeto

#### Dependências principais:
- `php`: ^8.1
- `guzzlehttp/guzzle`: ^7.2
- `laravel/framework`: ^10.10
- `laravel/sanctum`: ^3.3
- `laravel/tinker`: ^2.8

#### Dependências de desenvolvimento:
- `fakerphp/faker`: ^1.9.1
- `laravel/breeze`: ^1.29
- `laravel/pint`: ^1.0
- `laravel/sail`: ^1.18
- `mockery/mockery`: ^1.4.4
- `nunomaduro/collision`: ^7.0
- `phpunit/phpunit`: ^10.1
- `spatie/laravel-ignition`: ^2.0

### Passos de Instalação

**Atenção**: Aguarde a finalização de cada etapa antes de prosseguir para a próxima.

1. Abra um terminal no diretório onde deseja instalar o projeto e execute o comando:
   ```
   git clone https://github.com/anfip/Acesso-ao-bi.git
   ```

2. Acesse o diretório do projeto:
   ```
   cd Acesso-ao-bi
   ```

3. Execute o comando para atualizar as dependências:
   ```
   composer update
   ```

4. Renomeie o arquivo `.env.example` para `.env` ou crie uma cópia do mesmo e renomeie para `.env` no diretório raiz do projeto.

5. Altere a linha `APP_URL` no arquivo `.env` de `http://localhost` para `http://127.0.0.1`.

6. Gere a chave da aplicação executando:
   ```
   php artisan key:generate
   ```

7. Configure o arquivo `.env` com os dados de conexão ao banco de dados.

8. Não se esqueça de preencher as informações do SMTP para garantir o envio de e-mails corretamente.

9. Instale as dependências do Node.js com o comando:
   ```
   npm install
   ```

10. Para colocar a aplicação em produção, execute:
    ```
    npm run build
    ```

11. Para iniciar o servidor da aplicação, execute:
    ```
    php artisan serve
    ```

12. Execute o comando abaixo para garantir o carregamento correto de imagens privadas:
    ```
    php artisan storage:link
    ```

### Observações

- Ao acessar a aplicação e fazer login, haverá um painel padrão disponível para teste. Como não há upload de imagem ou registro inicial, algumas imagens podem ficar em branco. Após adicionar outros dados, o sistema funcionará normalmente.

- Para qualquer dúvida, entre em contato.

