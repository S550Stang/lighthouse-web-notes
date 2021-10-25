### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces.

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```Javascript
const whatToDoForLunch = function (hungry, availableTime) {
  if (hungry === false) {
    console.log("wait until you're hungry");
  } else if (hungry === true && availableTime <= 20) {
    console.log(
      "pick something up and eat in back in the Lab or in the kitchen, where you can get to know your fellow classmates."
    );
  } else if (hungry === true && availableTime > 20 && availableTime <= 30) {
    console.log("you deserve a break and could try a place in Gastown.");
  } else if (hungry === true && availableTime > 30) {
    console.log(
      "this is a bootcamp after all and you should probably reconsider."
    );
  }
};

whatToDoForLunch(true, 20);

whatToDoForLunch(true, 50);

whatToDoForLunch(false, 30);

whatToDoForLunch(true, 15);
```
