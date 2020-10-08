## Integration testing branch

This branch is used for cross module integration testing of pull requests on travis, including:
- phpunit tests
- behat tests

This may get moved to its own separate repo sometime in the future

Note - more modules than required for most tests (e.g. postgres) included in composer.json.  This is so that we do not have to run `composer require` in `.travis.yml`, instead we can use `composer install` and use the committed `composer.lock` file
