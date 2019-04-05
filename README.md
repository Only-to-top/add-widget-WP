# add-widget-WP

<h2>function.php</h2>

```php
add_action( 'widgets_init', 'register_my_widgets' );
function register_my_widgets(){
    register_sidebar( array(
        'name'          => "Header work time",
        'id'            => "sidebar_1",
        'description'   => '',
        'class'         => '',
        'before_widget' => '',
        'after_widget'  => "",
        'before_title'  => '',
        'after_title'   => "",
    ) );
}
```

<h2>template.php</h2>

```php
<?php
if ( function_exists('dynamic_sidebar') )
  dynamic_sidebar('sidebar_1');
?>
```
