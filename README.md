composer-base-library
=====================

Basic composer bundle for libraries:
The following folder structure is available for developing:

* src: Source directory for PHP classes
* tests: Test Class directory

Run unit tests
--------------

```
composer test
```

Generate PHP doc
--------------

```
composer doc
```

Run PHP Mass Detector
--------------

```
composer md
```

Git Pre-Commit Hook
--------------
to be able to easily use the included tools you are able to configure a so called pre-commit hook. This command is executed right before the actual commit happens. If the hook fails also the commit fails and so prevents the repository from unstable code. foo

*sample for file pre-commit* (located in {PROJECT_DIR}/.git/hooks)

```
#!/bin/sh
../../composer test
../../composer md
```

