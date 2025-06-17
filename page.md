### page body

```php
$page->body();
```

returns page body

---

### page children

```php
$page->children();
```

returns page sub pages

```php
<?php foreach($page->children() as $page): ?>
  <h1><?= $page->title() ?></h1>
<?php endforeach; ?>
```

---

### page content

```php
$page->content();
```

returns page content in markdown

---

### page uri

```php
$page->uri();
```

returns page uri eg. /blog/first-post

---

### page parent

```php
$page->parent();
``` 

returns page parent object

---



$page->hasDescendants();

$page->descendants();

$page->hasSiblings();

$page->siblings();



$page->summary();



$page->rawContent();
