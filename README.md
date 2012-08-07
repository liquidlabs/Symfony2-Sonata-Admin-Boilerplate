Symfony + Sonata Admin Bundle Boilerplate
===========================================

The code bundles Symfony 2.0.16 with Sonata Admin Bundle as a boilerplate/Barebone. 
It is targetted for developers who wish to have an admin panel with Symfony up and running
in no time. 

Bundles configured/added on the deps are follows:

* `TwigGenerator` 
* `PagerFanta` 
* `WhiteOctoberPagerfantaBundle` 
* `doctrine-fixtures` 
* `DoctrineFixturesBundle`
* `DoctrineBundle` 
* `SonataAdminBundle` 
* `SonataBlockBundle`
* `SonataCacheBundle`
* `SonatajQueryBundle`
* `SonataUserBundle`
* `SonataEasyExtendsBundle`
* `SonataDoctrineORMAdminBundle`
* `KnpMenuBundle`
* `KnpMenu`
* `Exporter`
* `SonataDoctrineExtensions`
* `FOSUserBundle`
* `EntityAudit`
 
How to install
===========================================

Download the files and follow the steps.

1. At first update the vendors
<pre>
php bin/vendors install
</pre>

2. Configure your database by updating information in app/config/parameters.ini
<pre>
database_driver   = pdo_mysql
database_host     = localhost
database_port     = 
database_name     = symfony_boilerplate
database_user     = root
database_password = 
</pre>

3. Run the following command to create the database
<pre>
php app/console doctrine:database:create
</pre>

4. Run the following command to add/update tables
<pre>
php app/console doctrine:schema:update --force
</pre>

5. Install the Assets by using the following command:
<pre>
php app/console assets:install web
</pre>

6. Create a Super Admin User
<pre>
php app/console fos:user:create admintest admin@test.com pass --super-admin
</pre>


7. Thats it!. You are ready to go. Visit url below for your Admin Dashboard :).
<pre>
http://localhost/symfony_boilerplate/web/app_dev.php/admin/dashboard
</pre>


License & Credits
===========================================
Same License as Symfony and Sonata Admin. 