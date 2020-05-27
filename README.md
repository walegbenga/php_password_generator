# PHP Password Generator Library Usage

To be able to use this library in your project, follow the steps below

## Requirement(s)

- php 5.5 >=
- Composer (for installing the library)
- Gitbash (for running the composer from the command line)

## Installing the package

To install the package in your project, run this command from the command line interface(cli) using gitbash
`composer require walegbenga/php_password_generator`. This will download the library into your project.

## Using the library

To use the library in your project, require the composer autoload script into your project like this
`require __DIR__ . '/vendor/autoload.php`
You can now use the library to generate the Random password for your users like this

```
$passGen = new \SecurePassword\PasswordGenerator($source, 4, CACHE_DIR);
echo $passGen->generate();
```

## Complete example

```
include __DIR__ . '/vendor/autoload.php';// Generally, this should be the relative path to the **vendor** folder
$passGen = new \SecurePassword\PasswordGenerator($source, 4, CACHE_DIR);
echo $passGen->generate();
```

### Where the library is useful

You can use this library to

- Generate hard to guess passwords for your users
- Use it to generate a temporary passwords for users who forgot there passsword
- Use it to generate a token for users
- Use it to generate Serial Number(sn) for your users and so on and so on
  Remember, in programming, your imagination is your limitation

### NB

The above example is just a basic usage of using the library.
