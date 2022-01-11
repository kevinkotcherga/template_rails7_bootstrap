# README
## template_rails7_bootstrap

### Rails 7.0.1, ruby 3.1.0 & bootstrap 5.1.3
```
rails new my_app -d postgresql -j esbuild --css bootstrap
cd my_app
code .
yarn run build:css
gem 'simple_form'
bundle install
rails generate simple_form:install --bootstrap
```

