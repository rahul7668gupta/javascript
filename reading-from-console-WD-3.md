Reading two nos from console and checking if the sum is even or odd.

Please execute this on console first: ```npm i console-read-write```

```
const io = require('console-read-write');

async function main () {
    var a = Number(await io.read());
    var b = Number(await io.read());
    var c;
    if (typeof a == "number" && typeof b == "number") {
        c = a + b;
        if (c % 2 == 0) {
            io.write("It's Even");
        } else if(c%2 != 0) {
            io.write("It's Odd");
        } else {
            io.write("Invalid Input");
        }
    } else {
        io.write("Could not execute");
    }
    
}

main();

```
