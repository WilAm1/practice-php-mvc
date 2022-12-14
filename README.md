# Practice using PHP the modern way

## Structure

What I've found:

- use `namespace` in every file to make it easy to load files
- use autoloader from Composer
- when using autoloader, include the source of your file in the composer.json file. Make sure the root is in the src directory
  - Example would be:

```json
"autoload": {
  "psr-4": {
  "vendorName\\rootNameSpace\\": "src/"
    }
}
```

- After that, run `composer dump-autoload` to create the autoloader
- use `require vendor/autoload.php` when using autoloader.
- to avoid writing require every single file, use .htaccess to automate this.

## Best practices
