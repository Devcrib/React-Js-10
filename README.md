reactJs10


Repl Link : https://repl.it/@DotunLonge/FluffyEvilNorwayrat


## A Really Really Brief Intro To JSX

#### What is JSX?

Javascript Expression **JSX**, is a React extension that allow one to write Javascript that *looks like *HTML.

JSX allows for the coupling of rendering logic and UI logic into one piece, that is, it puts markup and logic into one file.

Example:

```
const element = (
           <h1>
             Hello, {formatName(user)}!
         </h1>
    );
```

Using the h1 tag in javascript is a JSX style.

#### How is this achieved?

We need our browsers that we are actually doing this. This can be achieved with a tool called Babel and the process is called compilation.

Babel compiles the JSX to React.createElement( ) calls.

For example, the 2 codes are the same, only difference is that JSX was employed in the first.

```
const element = (
           <h1 className="greeting">
                Hello, world!</h1>
       );

const element = React.createElement(
            'h1',
           {className: 'greeting'},
            'Hello, world!'
     );
```

After compilation, JSX becomes objects too. And for this reason, operations like assigning them to variables, using the in conditionals, using them in functions by passing them as arguments and returning them become possible.