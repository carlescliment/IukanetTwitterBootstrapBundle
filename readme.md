IukanetCrudGeneratorBundle
=============================

Bundle para usar [Twitter Bootstrap](http://http://twitter.github.com/bootstrap/) con [Symfony2](https://github.com/symfony/symfony).

Este bundle incluye:

  * Twitter Bootstrap 2
  * jquery 1.7.1
  * jquery ui 1.8.16

**ADVERTENCIA:** Este bundle se ha creado para usarlo de base del backend de los proyectos programados en IUKANET y está adaptado a nuestras necesidades, siéntete libre de usarlo y adaptarlo a tus propias necesidades.

Instalación
-----------

Añade IukanetTwitterBootstrapBundle a tus vendors:

     git submodule add http://github.com/iukanet/IukanetTwitterBootstrapBundle.git vendor/bundles/Iukanet/TwitterBootstrapBundle

Añade al autoload:

    // app/autoload.php
    $loader->registerNamespaces(array(
        // ...
        'Iukanet'          => __DIR__.'/../vendor/bundles',
        // ...
    ));

Añade el IukanetBootstrapBundle a tu AppKernel.php:

    // app/AppKernel.php
	public function registerBundles()
	{
		$bundles = array(
			// ...
			new Iukanet\TwitterBootstrapBundle\IukanetTwitterBootstrapBundle(),
			// ...
			);
		// ...
	}

Acuérdate de ejecutar la instalación de los assets:

	app/console assets:install web

Autor
-----

Juan Baixauli - <juan@iukanet.com>

Sponsor
-------

[IUKANET Hosting](http://www.iukanet.com)
