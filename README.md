# Angular8 i18n *no* issue with multiple HTML tags in target.

This is a minimal *working* sample project to emphasize and show the issue with i18n since Angular v9 when more HTML tags are used inside "target" than in "source".
In this repo angular 8 is used and it works as expected!

## Build & Run

* `npm install`
* `npm run build:localize`
* browse to [http://localhost:4204/de-DE](http://localhost:4204/de-DE) -> invalid HTML tag order
* browse to [http://localhost:4204/en-GB](http://localhost:4204/en-GB) -> just text changes added
* browse to [http://localhost:4204/de](http://localhost:4204/de) -> source text

You can try to run `docker run -it -p4204:80 -v $(pwd)/dist:/app --workdir /app --rm php php -S 0.0.0.0:80` 
or run an http-server on dist with anything else.
