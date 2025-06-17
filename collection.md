```php
$site->findPage('/route/to/specific/page')->children(); // get all subpages from '/route/to/specific/page'
```

```php
$subpages = $site->findPage('/page')->children();  // get all subpages from '/page'

foreach($subpages as $subpage) {
  echo $subpage->title();
}
```

$page->children()->search('search text');

$page->children()->filter('published');

```php
$page->children()->filter('category', 'cars'); // returns all subpages where 'category' is 'cars'
```

$page->children()->shuffle();

$page->children()->sort();

$page->children()->slice( 0, 5 );

$page->descendants();
