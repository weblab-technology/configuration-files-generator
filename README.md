## Getting started

### Install

##### 1. composer

`php composer.phar install`

##### 2. private config

Clone private.yml.dist to private.yml (set your path in example section)

```yml
- template: example
  format: php
  destination: "../path-to-php-project/example.php"
```
##### 3. parameters

Clone parameters.yml.dist to parameters.yml (there are some tests parameters)

```yml
DB__TEST__HOST: "localhost"
DB__TEST__NAME: "test"
DB__TEST__USERNAME: "root"
DB__TEST__PASSWORD: "password"
```

### Usage

##### 1. Get command

Run command **php commands/generateCommand.php** (command with test parameters will be generated)

Output will look like this:

for windows

```
php run.php --DB__TEST__HOST="localhost"  --DB__TEST__NAME="test"  --DB__TEST__USERNAME="root"  --DB__TEST__PASSWORD="password"
```

for linux

```
php run.php --DB__TEST__HOST="localhost" \
--DB__TEST__NAME="test" \
--DB__TEST__USERNAME="root" \
--DB__TEST__PASSWORD="password"
```

##### 2. Run generation

Copy output command and execute it in your command line

Generated configuration files will be moved to the paths specified in the private.yml


## License

WebExtractor is licensed under the MIT license.

Eugene Suvorov zarkovsky@yandex.ru

Oleksandr Knyga oleksandrknyga@gmail.com
