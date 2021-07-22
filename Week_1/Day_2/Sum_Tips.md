### Tips

It should take the 2 numbers and output the sum. The `slice` function will be helpful to delete the first 2 index because we only need to grab `index 3` and `index 4` then output the sum of the 2 numbers.


#### Start with the following code below:
```javascript
const args = process.argv;
console.log(args);
```

If you use the code above and execute it using the following below it should output this.

```
> node sum.js 10 25
[ 'node',
  '/vagrant/w1/d1-focal/sum.js',
  '10',
  '25' ]
  ```

  Check out [Command Line Args](https://flex-web.compass.lighthouselabs.ca/c997336c-2105-4241-9437-b4e21b602aa7) for a more deeper discussion

  ##### HINT: 
  Items in an array can be indexed using square brackets notation, and array indexes start at 0. For example, to get the second element in the array we would use `process.argv[1]`.

You'll find that the result of adding the two "numbers" passed to your code as command line arguments is not what you expect. This is because all command line arguments are strings and the + operator concatenates them. To calculate a sum, you'll want to [convert the strings to numbers first](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number#Convert_numeric_strings_to_numbers).

### Desired Output
Given the following arguments, your code should output the following results:

```
> node sum.js 4 5
9
```

```
> node sum.js 5 -12
-7
```