# README
## template_rails7_bootstrap

### Rails 7.0.1, ruby 3.1.0 & bootstrap 5.1.3
```
rails new project_name -d postgresql -j esbuild --css bootstrap
cd project_name
code .
```

### To test this:
```
rails g controller home
rails db:create
rails db:migrate
```
```
# inside config/routes.rb  
Rails.application.routes.draw do  
  get "home/index"  
  root to: "home#index"  
end  
```
```
<!-- inside app/views/home/index.html.erb -->
<h1>Welcome, this is the home page</h1>

<button type="button"
        class="btn btn-lg btn-danger"
        data-bs-toggle="popover"
        title="Popover title"
        data-bs-content="Amazing content, right ?">
        Click to toggle popover
</button>
```

### Launch localhost 
```
./bin/dev
```
### Javascript with bootstrap
```
// Inside app/javascript/application.js
var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'))
var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
  return new bootstrap.Popover(popoverTriggerEl)
})
```
