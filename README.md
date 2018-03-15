To reproduce, clone this repository and run:

```
npm install
./node_modules/.bin/broccoli serve
```

Then in a new terminal, run

```
echo 's = "CoffeeScript source"' > src/file.coffee
sleep 1
git diff src/file.js
```

`src/file.js` has been overwritten with the CoffeeScript output.
