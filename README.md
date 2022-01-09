# Tictactoe
Simple tictactoe app in Typescript

## Jupiter's conclusion
This is an evaluation of the react tutorial page (https://reactjs.org/tutorial/tutorial.html), and added types via typescript.
The concept description was good, and easy to follow but lacks depth in terms of real-world application. 

However the code is in Javascript, so you would need to know how to define the types in React.Component.

This can be done via `React.Component<Props, State>`

For example:
```
type GameProps = {
    xIsNext: boolean
}

class Game extends React.Component<GameProps> {...}
```

Also, this way of writing is too tedious. A functional component would have
made things shorter, and is used more in practice of real applications.

Using hooks as well to manage state via `useState` is much easier than
defining it in the constructor as provided in the docs.

Overall, It's a good intro, but in no way represent how you should create
code in the real-world. So keep reading the documentation and I recommend reading on the following afterwards
* react-hooks
* graphql/redux

Then look at frameworks such as Next.js / Gatsby