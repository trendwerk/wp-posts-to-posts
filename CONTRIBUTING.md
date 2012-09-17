This guide is meant for developers wanting to work on the plugin code.

### Setup

Make a fork and clone it:

```
git clone --recurse-submodules git@github.com:{YOUR GITHUB USERNAME}/wp-posts-to-posts.git posts-to-posts
```

You can now work on the PHP and CSS files.

### JavaScript

Don't modify `admin/box.js` directly. Instead:

- [Install node.js](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager) and [npm](http://npmjs.org/).

- Install [CoffeeScript](http://coffeescript.org):

```
npm install -g coffee-script
```

and edit the `admin/box.coffee` file. To compile it, run:

```
coffee -c admin
```

### Testing

The plugin comes with a few unit tests.

1. Install [PHPUnit](https://github.com/sebastianbergmann/phpunit/).
2. Install the WP testing suite: [nb/wordpress-tests](https://github.com/nb/wordpress-tests)
3. [Install the scbFramework](https://github.com/scribu/wp-scb-framework/wiki) in the mu-plugins dir.
4. Run `./bin/test /path-to-nb-wordpress-tests-dir/`