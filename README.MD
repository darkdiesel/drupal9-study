# Drupal 9 Study
I created this repository to lean Drupal 9 CMS and make some experiments, modules and themes test. Test and write my own modules.

## Table of content
- [Run drush from local repository](#run-drush-from-local-repository)
- [Drush useful commands](#drush-useful-commands)


## Run drush from local repository
Sometimes i'm working on windows OS and i need drush. I installed drush via composer:

```shell
composer require --dev drush/drush:11.*
```

then created drush file in root of project with code:

```php
<?php
require_once ("vendor/drush/drush/drush");
```

and i can run drush from vendor folder and don't need change global version of drush depends on project and drupal cms version.

```shell
php drush cr
```

## Drush useful commands

- Cache rebuild:

  ```drush cr```

- Install module:

  ```drush en module_name```

- Uninstall module

  ```drush pmu module_name```

- Update entity while development (devel entity update module)

  ```drush entup``` or ```drush entity-updates```
