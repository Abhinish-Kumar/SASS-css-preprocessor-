# SASS(Syntactically Awesome Style Sheets)
Sass require a build process

### SASS Requirements
SASS is not understandable for browser directly it needs to setup tools to make it understandable for browser(to convert sass to css).NPM is a utility of node.js
1. NPM Node.js version >= 12
2. Git & GitHub(Optional)
3. Terminal App(Hyper)
4. Build(Vite)(cass to css)
5. Code Editor(VS Code)
6. SASS Module(Install it as node module)


## Build installation(VITE)
We have to install vite to create an environment to work with SASS.

```javascript

>>>>npm init vite@latest
>>>>switch to the create vite app
>>>>npm install

```

Change the css folder to scss folder.
Now Install scss

```javascript

>>>>npm install -D sass
>>>>Check json devdependency

```
Now we have both the sass and its environment.

```javascript

>>>>npm run dev

```
Now you can run scss code in scss file 

```scss

$bg:red;

body{
color:$bg;
}

```

## We have a two different flavors of sass.

Syntax Versions

### SASS Format
1. sass(indented formet)
2. No punctuation
3. Meaningful whitespace
4. We also no need of semicolons

```sass

$bg : red

body
  background:$bg

```
### SCSS Format

1. .scss (Sassy css formet)
2. CSS compatible-if you have a css file you can just transpile css file to scss file.
3. Most popular
4. ```sass

$bg : red;

body {
  background:$bg;
}
```

















