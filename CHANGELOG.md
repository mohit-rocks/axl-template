
0.4.5 / 2020-10-07
==================

* Fix packaging error with the missing version

0.4.4 / 2020-10-07
==================

* Fix error when specifying the --lando option. Fixes #31
* Enable tests on Python 3.9
* Remove Pipfile.lock so that dependencies are installed as per Python version
* Update Pipfile.lock
* Don't ignore settings.php. Fixes #24
* Fix code style issues reported by black and pylint
* Use pipenv in Github actions
* Add Pipfile
* Add documentation for whalebrew
* Add a new type to represent a single composer package
* Run tests with Github
* Add tests for click_types
* Refactor parse_package method to move the logic into the util class
* Set the default directory based on the package name
* Ensure click_types.ComposerPackage returns a list
* Add methods to get the package vendor and name to ComposerVersion
* Fixes #20: Allow the current directory to be specified (#21)
* Add Click param types to represent a composer package
* Update documentation to provide alternative for system requirements.
* Add documentation to run using Docker
* Set the name for the command when used via whalebrew

0.4.3 / 2020-07-22
==================

* Move docker-build workflow to proper location

0.4.2 / 2020-07-22
==================

* Add check for a valid name
* Disable aggregation when running via Lando (#15)
* Add Dockerfile to produce a Docker image on release
* Ignore platform reqs when running composer install
* Add Docker build to workflow
* Add modules & themes custom directory (#18)
* fix: phpcs errors on initial commits (#17)
* Fix configuration to load custom php.ini in lando

0.4.1 / 2020-07-08
==================

* Change branch name in our GitHub actions
* Change Renovate rules to split Drupal and npm dev dependencies
* Add phplint to GitLab CI template
* Add composer validate to GitLab CI template
* Update to phpdotenv 5.0
* Add purpose in README (#12)

0.4.0 / 2020-06-15
==================

* Exit instead of just warning if PHP or composer are not present
* Check and report if memory limit is not -1 (unlimited)
* Make sure we send a return code when the command fails
* Better handle errors when deleting an existing directory
* Generate renovate.json along with Drupal files
* Write config_sync_directory settings
* Minor changes in README for completeness
* Add README for init-gitlab
* Add VSCode workspace settings
* Add phpunit tooling for lando

0.3.0 / 2020-06-12
==================

* Add GitLab CI support
* Add more helpful messages to lando.py
* Add a new helper method to write bold messages
* Disable mounts for services that don't need it
* Add support to write settings.env.php
* Set default core version to 8.9.0

0.2.1 / 2020-06-04
==================

* Merge pull request #10 from axelerant/drupal-console
* Fixes #9: Remove drupal/console from composer.json

0.2.0 / 2020-05-26
==================

* Fixed "init-lando" FileNotFoundError (#6)
* Add requirements.txt
* Add default pylintrc generated using 'pylint --generate-rcfile'
* Better handle webroot detection for drupal/drupal
* Allow specifying Drupal core version
* Remind to run composer install if installation is skipped.
* Refactor composer install method
* Added check to exit if composer fails to install vendors. (#5)
* Convert print calls to click's utilities
* Update README with new options documentation
* Refactor argument parsing using click
* fix markdown lint issues

0.1.5 / 2020-04-21
==================

* Add drupal-quality-checker to drupal-scaffold.allowed-packages
* Add requirements to README.
* Handle failures when composer is not present
* Add axelerant specific dev-dependencies to the template
* Format files using black
* Install correct composer packages and bump versions.
* Add required parameter for lando to work
* Override the database image for lando
* Fix issue with generated name for lando.yml
* Fix issue with default value for lando argument
* Refactor settings.lando.php generation and add memcache support
* Add installation instructions to the readme
* Update documentation and minor tweaks
* Ensure dist directory is empty before building
* Add Lando support and script
* Refactor common tasks into an util module
* Create the directory as a git repository
* Restructure the module for clarity
* Add a simple build script
