### page body

<pre> $page->body(); </pre>

returns page body

---

### page children

<pre>$page->children();</pre>

returns page sub pages

<pre>
  <?php foreach($page->children() as $page): ?>
    <h1><?= $page->title() ?></h1>
  <?php endforeach; ?>
</pre>

---

### page content

<pre>$page->content();</pre>

returns page content in markdown

---

### page uri

<pre> $page->uri(); </pre>

returns page uri eg. /blog/first-post

---

### page parent

`$page->parent();` 

returns page parent object

---



$page->hasDescendants();

$page->descendants();

$page->hasSiblings();

$page->siblings();



$page->summary();



$page->rawContent();
