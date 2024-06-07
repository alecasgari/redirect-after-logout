# To redirect after Log-out in WordPress
Put this php code in your function.php file
```php
// Redirect after logout
add_action('wp_logout','auto_redirect_after_logout');

function auto_redirect_after_logout(){
  wp_safe_redirect( home_url() );
  exit;
}
```
