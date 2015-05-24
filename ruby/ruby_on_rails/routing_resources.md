##Routingについて

##resources :publishers
  
```ruby
Rails.application.routes.draw do
  resources :publishers
end
```
  
then,  

|Prefix        |Verb  |URI Pattern                   |Controller#Action |
|:-------------|:-----|:-----------------------------|:-----------------|
|publishers    |GET   |/publishers(.:format)         |publishers#index  |
|              |POST  |/publishers(.:format)         |publishers#create |
|new_publisher |GET   |/publishers/new(.:format)     |publishers#new    |
|edit_publisher|GET   |/publishers/:id/edit(.:format)|publishers#edit   |
|publisher     |GET   |/publishers/:id(.:format)     |publishers#show   |
|              |PATCH |/publishers/:id(.:format)     |publishers#update |
|              |PUT   |/publishers/:id(.:format)     |publishers#update |
|              |DELETE|/publishers/:id(.:format)     |publishers#destroy|
