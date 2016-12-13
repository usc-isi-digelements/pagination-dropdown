# pagination-dropdown

A Polymer Element providing a way to page through elasticsearch results.

### Example
```html
<pagination-dropdown
  current-page="{{pageNum}}" 
  num-results="{{resultCount}}" 
  results-per-page="{{pageSize}}">
</pagination-dropdown>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests require a local instance of elasticsearch with the `mockads` index created by running `data/import_test_data.sh`.

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

