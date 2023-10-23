### Laravel installation

- _**composer create-project laravel/laravel example-app**_
- _**php artisan serve**_ inside the folder
- create database
- edit _**.env**_ file to reflect the database and password
- _**php artisan migrate**_ (make sure to uncomment the _extension=pdo_mysql_ in php.ini)
- create table: _**php artisan make:migration create_products_table**_
- _**php artisan migrate**_
  create model: **php artisan make:model Product**
- add the fields
- add controller: **php artisan make:controller ProductController**
- create view: _resources > views_
  - add a folder "products"
  - add index.blade.php inside the products folder
- create route: (inside "routes > web.php" folder)  
  **Route::get('/product', [ProductController::class, 'index'])->name('product.index');**
