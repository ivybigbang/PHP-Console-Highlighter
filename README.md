PHP-Console-Highlighter
=======================

Highlight PHP code in terminal

Install
-------

Just create a `composer.json` file and run the `php composer.phar install` command to install it:

```json
{
    "require-dev": {
        "jakub-onderka/php-console-highlighter": "0.*"
    }
}
```

Usage
-------
```php
<?php
use JakubOnderka\PhpConsoleColor\ConsoleColor;
use JakubOnderka\PhpConsoleHighlighter\Highlighter;

require __DIR__ . '/vendor/autoload.php';

$highlighter = new Highlighter(new ConsoleColor());

$fileContent = file_get_contents(__DIR__ . '/example.php');
echo $highlighter->getWholeFile($fileContent) . PHP_EOL;
```
