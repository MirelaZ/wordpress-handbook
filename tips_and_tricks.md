# Tips and tricks

Below are some useful tips and tricks to keep in mind when developing in WordPress.

## Calling WP_Query inside a method

When you want to use the power of WordPress's own `WP_Query` inside a method in your custom class, you'll need to add a `\` in front of it so that you can tel PHP that it is in global namespace, and not in the namespace of the class it's in.

```php
$your_query = new \WP_Query( $your_query_args );
```

