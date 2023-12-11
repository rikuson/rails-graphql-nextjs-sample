# Proceduer

## Init rails

```shell
gem install rails
rails new backend -B -d postgresql --skip-turbolinks --skip-git
```

## Install graphql

```shell
bundle add graphql
rails generate graphql:install
```

## Add User model

```shell
rails g model User email:string password_digest:string
rails db:migrate
rails g graphql:object User
rails graphql:schema:idl
```
