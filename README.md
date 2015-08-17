# elda

> WIP

Simple WordPress Plugin Bootstrapper. Elda loades files and register the [wp-autoload](https://github.com/frozzare/wp-autoload). Default Elda looks for code in `src` directory in your plugin directory, this can be changed with `src_dir` in options array.

## Example

```php
/**
 * Plugin Name: Customer
 * Description: Customer description
 * Author: Customer
 * Author URI: http://example.com
 * Version: 1.0.0
 * Textdomain: customer
 */

use Frozzare\Elda\Elda;

/**
 * Bootstrap Customer plugin with Elda.
 */
Elda::boot( __DIR__, [
    'files'     => [
      'lib/papi.php'
    ],
    'namespace' => 'Customer\\'
] );
```

## License

MIT © [Fredrik Forsmo](https://github.com/frozzare)
