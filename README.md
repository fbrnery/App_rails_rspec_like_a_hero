# README

# Instalando o Rspec no projeto Rails:

# 1- Primeiro, incluir o rspec no gemfile:
Obs: se quiser especificar uma versão, faça assim:

- group :development, :test do
- gem 'rspec-rails', '~> 3.8'
- end

Ou OBS 2: Sem especificar versão, deixando o bundle instalar a versão mais recente:

-group :development, :test do
-gem 'rspec-rails'
-end

# 2- Depois rode no terminal:

$ bundle install

# 3- Depois disso, vc vai rodar o comando de instalação do rspec:

$ bin/rails generate rspec:install

# 4- Depois, pode rodar o rspec no terminal, para testar, com os comandos:

$ bin/rails spec

ou 

$ bundle exec rspec

# 5- Depois, toda vez que vc gerar um model, controller ou um scaffold, todos os testes referentes a estes serão gerados automaticamente na pasta spec.

Por fim, agora podemos trabalhar.

