```php
$site->findPage('route/to/specific/page')->children();
```

```php
$subpages = $site->findPage('/page')->children();

foreach($subpages as $subpage) {
  echo $subpage->title();
}
```

$page->children()->search('search text');

$page->children()->filter('published');

$page->children()->filter('category', 'cars');

$page->children()->shuffle();

$page->children()->slice( 0, 5 );

$page->descendants();
