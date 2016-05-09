## Practice: Install a Package for Enumeration

- What package did you install for enumeration?
- enum

## Research: Popular NPM Packages

Package 1: Mocha

1.  What problem does this package solve?
Mocha is a feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases. So I guess it's supposed to mae testing easier...and fun?
1.  How can I use this package in my own code? What steps are involved?

var assert = require('chai').assert;
describe('Array', function() {
  describe('#indexOf()', function () {
    it('should return -1 when the value is not present', function () {
      assert.equal(-1, [1,2,3].indexOf(5));
      assert.equal(-1, [1,2,3].indexOf(0));
    });
  });
});

```sh
$  mocha
```
1.  How well-maintained is this package? What criteria did I use to decide?
Well maintained, it has over 6k commits with the most recent being yesterday.
I've even heard of it before.

Package 2: Mongoose

1.  What problem does this package solve?
It's a mongodb object modeling tool for use in async environments.

1.  How can I use this package in my own code? What steps are involved?
2. var Schema = mongoose.Schema,
    ObjectId = Schema.ObjectId;

var BlogPost = new Schema({
    author    : ObjectId,
    title     : String,
    body      : String,
    date      : Date
});
You can define schemas in its schema interfaces.
1.  How well-maintained is this package? What criteria did I use to decide?
Last commit was yesterday, over 6k commits.

Package 3: Grunt

1.  What problem does this package solve?
A lot. It automates much of the development process and can be used for testing, compilation and linting.
We've already used it extensively through the course.
1.  How can I use this package in my own code? What steps are involved?
Configure your package.json and Gruntfile, npm install -g grunt-cli, go to your project's root directory, install dependencies with npm install, and then run grunt with grunt in the cli.
1.  How well-maintained is this package? What criteria did I use to decide?
very well maintained, over 1k commits and a lot of recent activity, plus we use
it all the time.
