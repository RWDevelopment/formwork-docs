# Collection

[public function children()](https://github.com/getformwork/formwork/blob/1.x/formwork/Core/AbstractPage.php#L232)


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

returns all subpages from page where subpage contains 'search text' in title or summary or tags or content

```php
$page->children()->search('search text');
```

### filter collection

```php
$page->children()->filter('published'); // returns all subpages where 'published' is 'true'
```

```php
$page->children()->filter('category', 'cars'); // returns all subpages where 'category' is 'cars'
```

```php
$page->children()->shuffle(); // shuffle subpages
```

$page->children()->sort();

$page->children()->slice( 0, 5 );

$page->descendants();
