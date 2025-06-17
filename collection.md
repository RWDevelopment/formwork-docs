# Collection

```php
$site->findPage('/route/to/specific/page')->children(); // get all subpages from '/route/to/specific/page'
```

```php
$subpages = $site->findPage('/page')->children();  // get all subpages from '/page'

foreach($subpages as $subpage) {
  echo $subpage->title();
}
```
### search collection

```php
$page->children()->search('search text'); // returns all subpages where page contains 'search text' in title or summary or tags or content
```

### filter collection

```php
$page->children()->filter('published'); // returns all subpages where 'published' is 'true'
```

```php
$page->children()->filter('category', 'cars'); // returns all subpages where 'category' is 'cars'
```

$page->children()->shuffle();

$page->children()->sort();

$page->children()->slice( 0, 5 );

$page->descendants();
