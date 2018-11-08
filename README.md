# Arquivos de linguagem em Português do Brasil (pt-BR) para Laravel 5.7

## Instalação
1. Clonar este repositório na pasta `resources/lang/` do seu projeto
  ```shell
  $ cd resources/lang/
  $ git clone https://github.com/lucascudo/laravel-5.7-pt-BR-localization.git ./pt-BR
  ```
   Você pode remover o diretório .git caso deseje incluir e versionar os arquivos deste projeto no seu repositório.

  ```shell
  $ rm -r pt-BR/.git/
  ```
2. Configurar o Framework para utilizar 'pt-BR' como linguagem padrão
  ```
  // Altere Linha 81 do arquivo config/app.php para:
  'locale' => 'pt-BR',
  ```
3. Para tradução dos textos nas páginas (views) de login. (Opcional).

Crie o arquivo `resources/lang/pt-BR.json` e adicione o seguinte conteúdo:
  ```
  {
    "E-Mail Address" : "Endereço de e-mail",
    "Password" : "Senha",
    "Remember Me" : "Lembrar de mim",
    "Forgot Your Password?" : "Esqueceu a senha?",
    "Logout" : "Sair",
    "Reset Password" : "Redefinir Senha",
    "Send Password Reset Link" : "Enviar link para redefinir a senha",
    "Dashboard" : "Painel"
  }
  ```
## Nota
A palavra 'Dashboard' não está definida para ser traduzida na view home.

Para traduzí-la, edite o arquivo `resources/views/home.blade.php` e troque o texto:
  ```
  Dashboard
  ```
  por este
  ```
  {{__('Dashboard')}}
  ```
## Localização para outras versões do Laravel
  
* [Laravel 5.4](https://github.com/Leomhl/laravel-5.4-pt-br-localization)
* [Laravel 5.5](https://github.com/enniosousa/laravel-5.5-pt-BR-localization)
* [Laravel 5.6](https://github.com/lucascudo/laravel-5.6-pt-BR-localization)
* [Laravel 5.7](https://github.com/lucascudo/laravel-5.7-pt-BR-localization)
