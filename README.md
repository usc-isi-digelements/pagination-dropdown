# pagination-dropdown

An element providing a way to page through elasticsearch results. Works with 
elastic-client-search. 

Example:
```html
    <template is="dom-bind">
        <elastic-client
            config='{"host": "http://localhost:9200"}'
            client="{{esclient}}"
            cluster-status="{{my-status}}">
        </elastic-client>
        
        <elastic-client-search
            client="[[esclient]]"
            index="mockads"
            query="null"
            results="{{data}}"
            lastError="{{error}}"
            page="{{pageNum}}"
            page-size="{{pageSize}}">
        </elastic-client-search>

        <pagination-dropdown current-page="{{pageNum}}" 
            num-results="{{resultCount}}" 
            results-per-page="{{pageSize}}">
        </pagination-dropdown>
    </template>
```

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

To run the demo + unit tests, you will need a local elasticsearch instance and the 
mockads data referenced in the elastic-client-search repo.