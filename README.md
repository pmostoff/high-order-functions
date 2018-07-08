# High Order Functions

This Swift Playground contains examples of some of the high order functions for processing sequences in Swift. I created it as a reference to look back on and refresh my memory. Hopefully it will prove helpful to others as well.

### .map{}
Allows us to perform the action within it's closure on each element in the sequence. 
For example, using `.map{$0 * 2}` on an array of integers would produce a new array containing the doubled values of the original array.

### .filter{}
Produces an array containing all of the elements that satisfy the condition within it's closure. 
For example, using `.filter{$0 % 2 == 0}`  on an array of integers would return a new array containing only the even integers of the original array.

### .reduce()
Produces a single result from the elements of a sequence. 
For example, using `.reduce(0, +)` on an array of integers would combine all of the elements into their sum value.

### .flatMap{$0}
Flattens a sequence of arrays together in the order that they are presented. 
For example, using `.flatMap{$0}` on an array like this: `[[1, 2], [3, 4], [5, 6]]` would produce this: `[1, 2, 3, 4, 5, 6]`.

### Chaining Functions
These high order functions can be used on one another. For example, you can use `flatMap{}.reduce(0, +)` to combine multiple arrays into one unified array, and then combine all of the elements of the newly unified array.

### Zip
Groups values in arrays. 
For example, using zip on two arrays would group arrayOne's index[0] with arrayTwo's index[0].

### Zip + Map
Combining Zip with Map allows us to group together the values of two arrays and perform an action like addition on the pairings.

## Author

Programmed and designed by Peter Mostoff. [You can contact me via Twitter](https://twitter.com/pmostoff) if that's something you're interested in. I typically make things for the situations that they're needed in but I like to share my work and I'm sure there are plenty of ways that this can be improved. Please let me know if you have any cool suggestions!

If you're interested, you can visit my personal site to see what I'm up to at [Mostoff.me](http://mostoff.me) or if you want to support my work, check out the apps that I've published on the [App Store](https://itunes.apple.com/tc/developer/peter-mostoff/id1080412491)!

## License
`highOrderFunctions` is available under the MIT license. See the LICENSE file for more info.
