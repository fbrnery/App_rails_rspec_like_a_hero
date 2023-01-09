# README

# Instalando o Rspec no projeto Rails:

# 1- Primeiro, incluir o rspec no gemfile:
Obs: se quiser especificar uma versão, faça assim:

- group :development, :test do
- gem 'rspec-rails', '~> 3.8'
- end

# 1.1: Ou para especificar uma versão, faça assim, e deixe o bundle instalar a versão mais recente:

- group :development, :test do
- gem 'rspec-rails'
- end

# 2- Depois rode no terminal:

$ bundle install

# 3- Depois disso, vc vai rodar o comando de instalação do rspec:

$ bin/rails generate rspec:install

# 4- Depois, pode rodar o rspec no terminal, para testar, com os comandos:

$ bin/rails spec

ou 

$ bundle exec rspec

# 5- Depois, toda vez que vc gerar um model, controller ou um scaffold, todos os testes referentes a estes serão gerados automaticamente na pasta spec.

-Tipos de generate:

exemplos:

a - Para gerar somente um model:
$ rails generate model user

b - Para gerar somente um controller:
$ rails generate controller home index

c - Para gerar um scaffold:
$ rails generate scaffold User name:string city:string

d - Ou para gerar somente o teste rspec de request especifico:

$ rails generate rspec:request User

e - Conhecendo todas as opções de generate do rspec:

$ rails generate --help | grep rspec

- Vai gerar esse resultado no terminal:

Running via Spring preloader in process 10324
  - rspec:controller
  - rspec:feature
  - rspec:generators
  - rspec:helper
  - rspec:install
  - rspec:integration
  - rspec:job
  - rspec:mailer
  - rspec:model
  - rspec:observer
  - rspec:request
  - rspec:scaffold
  - rspec:system
  - rspec:view
  
  # 6 - Melhorando nosso teste com a Gem FFAKER, vá no arquivo gemfile e adcione essa gem:
  
  group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'rspec-rails', '~> 4.0.1'
  - gem 'ffaker'
end

Deve ficar assim, seu group:development, depois rode no terminal:

$ bundle install
  
  
  # Por fim, agora podemos trabalhar.

