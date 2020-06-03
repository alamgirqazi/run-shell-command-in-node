# Run bash file from node.js

```

const exec = require('child_process').exec;

// this is a self invoking anonymous function IIFE

(() => {
  command = `python runwithnode.py`;

  var run = exec(command, (error, stdout, stderr) => {
    if (error) {
      console.log('error', error);
      console.log('error in detail', stderr);
    } else {
      console.log('result', stdout);
    }
  });
})();



```

### How to run

> node index
