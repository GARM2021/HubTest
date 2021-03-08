15:26 p. m. 08/03/2021
02:18 p. m. 24/02/2021
composer create-project laravel/laravel Laravel-desde-Cero 

D:\xampp\htdocs\Laravel-desde-Cero>php artisan server

D:\xampp\htdocs\Laravel-desde-Cero>php artisan make:migration CreateProductsTable

D:\xampp\htdocs\Laravel-desde-Cero>php artisan migrate:fresh 

D:\xampp\htdocs\Laravel-desde-Cero>php artisan make:model Product

D:\xampp\htdocs\Laravel-desde-Cero>php artisan make:factory ProductFactory --model=Product

D:\xampp\htdocs\Laravel-desde-Cero>php artisan thinker
>>> App\Models\Product::Factory()-> make(); 
=> App\Models\Product {#3385
     title: "Voluptas hic.",
     description: "Provident ex unde odit ut quos.",
     price: 64.22,
     stock: 1,
     status: "avialable",
}
>>> App\Models\Product::Factory()-> create();
=> App\Models\Product {#3386
     title: "Possimus excepturi quos.",
     description: "Suscipit id rerum et ut provident. Voluptatem cumque facere et qui fugit explicabo.",
     price: 92.62,
     stock: 9,
     status: "unavailable",
     updated_at: "2021-02-26 23:27:27",
     created_at: "2021-02-26 23:27:27",
     id: 1,
   }
>>> App\Models\Product::Factory()->count(10)-> create();
=> Illuminate\Database\Eloquent\Collection {#3348
     all: [
       App\Models\Product {#3389
         title: "Placeat cupiditate deleniti.",
         description: "Doloribus sint facere ducimus voluptatum quaerat beatae. Mollitia consectetur aut ipsa esse unde est iure.",
         price: 65.11,
         stock: 2,
         status: "unavailable",
         updated_at: "2021-02-26 23:28:55",
         created_at: "2021-02-26 23:28:55",
         id: 2,
       },
     .........................
       App\Models\Product {#4119
         title: "Culpa odit deleniti illum.",
         description: "Nihil iusto aut veniam sit illum. Eum autem unde reiciendis quod eaque.",
         price: 53.09,
         stock: 6,
         status: "unavailable",
         updated_at: "2021-02-26 23:28:56",
         created_at: "2021-02-26 23:28:56",
         id: 11,
       },
     ],
   }
 ///////////Se modifica el DatabaseSeeder.php 

 $products = Product::factory(50)->create();

y se ejecuta 

D:\xampp\htdocs\Laravel-desde-Cero>php artisan migrate:fresh --seed
Dropped all tables successfully.
Migration table created successfully.
Migrating: 2014_10_12_000000_create_users_table
Migrated:  2014_10_12_000000_create_users_table (1,241.32ms)
Migrating: 2014_10_12_100000_create_password_resets_table
Migrated:  2014_10_12_100000_create_password_resets_table (183.97ms)
Migrating: 2019_08_19_000000_create_failed_jobs_table
Migrated:  2019_08_19_000000_create_failed_jobs_table (195.46ms)
Migrating: 2021_02_26_200925_create_products_table
Migrated:  2021_02_26_200925_create_products_table (113.39ms)
Database seeding completed successfully.

/////////// se adicionan 50 registros mas con 
D:\xampp\htdocs\Laravel-desde-Cero>php artisan db:seed

////////////Emigra Esquema de SQL ///////////////////////
//// https://laravelarticle.com/laravel-migration-generator-online
////Nota cambiar ' por `<<<<<<<<<<<<<<<<<<<<<<<<<<<<

CREATE TABLE `apodomiciliox`(
	`Id` bigint(20) unsigned NOT NULL AUTO_INCREMENT,
	`Seccion` int NULL,
	`Tel` char(13) NULL,
	`Nombre` char(40) NOT NULL,
	`Paterno` char(40) NOT NULL,
	`Materno` char(40) NOT NULL,
	`Calle` char(50) NOT NULL,
	`Exterior` int NOT NULL,
	`Interior` char(15) NULL,
	`Colonia` char(40) NULL,
	`E1` date NULL,
	`E2` date NULL,
	`E3` date NULL,
	`E4` date NULL,
	`ViaRec` char(40) NULL,
	`NombreCompleto` char(100) NULL,
	`DirCompleto` char(100) NULL,
	`FNac` date NULL,
	`TelCasa` char(20) NULL,
	`TelMovil` char(20) NULL,
	`Dep` char(3) NULL,
	`IdA` int NULL
) ON `PRIMARY`;









