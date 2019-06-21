LingGalleryFilter
===============
2019-06-21


A simple jquery plugin to filter items based on their categories.





Demo: https://lingtalfi.com/ling-gallery-filter

![screenshot of ling-gallery-filter](https://lingtalfi.com/img/js/ling-gallery-filter/ling-gallery-filter.png)



How to
==========

First create a div (or any html element) containing your items, and each item has a data-category attribute like this:

```html
<div id="my-items">
    <div class="item" data-category="cat1">item one</div>
    <div class="item" data-category="cat1">item two</div>
    <div class="item" data-category="cat2">item three</div>
</div>
```


Then create another div (or any html element) containing your tags, and each tag has a data-tag attribute (corresponding to an item category), like this:

```html
<div id="my-tags">
    <a data-tag="all" href="#">All</a>
    <a data-tag="cat1" href="#">Category one</a>
    <a data-tag="cat2" href="#">Category two</a>
</div>
```

Notice the "all" tag, it has a special meaning (it will display all items).


Now, just import the js file (the ling-gallery-filter.js file) after jquery, and use this js snippet:

```js
$(document).ready(function () {
   $('#my-items').lingGalleryFilter({
            tagContainer: $('#my-tags'),
        });        
});
```

That's it.




History Log
------------------
    
- 1.0.0 -- 2019-06-21

    - initial commit
    