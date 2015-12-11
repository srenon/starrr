starrr
======

1-5 (or 1-`*`) star rating, in jQuery.

## Usage

### Create the stars
```
<div class='starrr'></div>

jQuery(function() {
  return jQuery(".starrr").starrr();
});
```

### With an existing rating
```
<div class='starrr' data-rating='4'></div>

jQuery(function() {
  return jQuery(".starrr").starrr();
});
```

### To disable changes to stars using Data Attribute
```
<div class='starrr' data-rating='4' data-disabled='false'></div>

jQuery(function() {
  return jQuery(".starrr").starrr();
});
```
### To disable changes to stars using input

```
<input type='text' name='rating' value='3' disabled="disabled" class="form-control" />
<div class="starrr" data-rating='4'  data-connected-input='rating'></div>

jQuery(function() {
  return jQuery(".starrr").starrr();
});
```

### Listen for events
```
$('.starrr').on('starrr:change', function(e, value){
  alert('new rating is ' + value);
});
```

## License

MIT
