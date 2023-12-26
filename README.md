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

```css

$bg : red

body
  background:$bg

```
### SCSS Format

1. .scss (Sassy css formet)
2. CSS compatible-if you have a css file you can just transpile css file to scss file.
3. Most popular
4.

```css

$bg : red;

body {
  background:$bg;
}

```

# Sass Variables
The only difference between variable of normal css is that the scss variable has to be converted to the normal css.


```css

$bg : red;

body {
  background:$bg;
}

```

#### Rules of varibel 

1. $Name
2. <variable>:<expression>
3. Compile to css

### Variable scope

Variables can normally have a global scope

```css

$primary-color:red;

h1{
     $primary-color:yellow;
     color:css$primary-color;
}

p{
color:$primary-color;
}

```


1. Top Level (Global)
2. Curly Braces(Local)
3. Shadowing:-Local variable can have same name of global variable that is called as shadowing.


##### Practice

```scss

$primary-color:skyblue;

h1{
  color:$primary-color;
}

p{
  $primary-color:pink;
  color: $primary-color;
}

```

### Global Flag
We redefine the primarry color of global varibale by adding a flag to it.

1. Redefinines globals.
2. Not for new vars.

```scss

$primary-color:skyblue;

h1{
  color:$primary-color;
}

p{
  $primary-color:rgb(214, 43, 72) !global;
  color: $primary-color;
}

h1{
  color:$primary-color;
}

```

### Underscores vs Hyphens
In variables name the Underscores are same as Hyphen.like "" and ''.

```scss

$primary-color:skyblue;
$primary_color:rgb(206, 156, 17);

h1{
  color:$primary-color;
}


```

## Nesting
SCSS allow us to place rules inside other rules.
This is known as nesting It allows to write code lot easier.

### SASS Nesting

1. Combines rules.
2. Extra CSS.(make complax to red)
3. Bandwidth (more time to be transpiled so not nest deeply)

Note :- first write the css for box and then write the rules of nested elements.

```scss

.box{

padding:1rem 2rem;
background:beige;
color:black;

h1,p{
margin:0;
}
h1{
color:red;
}

}

```













