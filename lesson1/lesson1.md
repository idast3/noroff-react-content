## Installation

We're going to use Create React App to create a new app. Run the following in your terminal or command line:

```js
    npx create-react-app noroff-react
```

Change into that directory and start the app:

```js
    cd noroff-react
    npm start
```

This will start your app at [http://localhost:3000](http://localhost:3000) (or another port if 3000 is already in use).

## App structure

Open the project in your editor and the above link in your browser.

`create-react app` has installed a whole bunch of packages and created our first component called `App` in the `src` directory. All the code we will write will go in the `src` directory.

Open `src/App.js`. This is our first component. It's a function called `App` and it will render on the page whatever we return from it.

Delete everything between and including the `<header>` tags and replace them with an `<h1>` tag with the text `Noroff React App`.

```jsx
function App() {
    return (
        <div className="App">
            <h1>Noroff React</h1>
        </div>
    );
}
```

Hit save and check your browser. The page will automatically reload when you make changes to the code so you won't need to refresh your browser to see the changes.

### How it works

Inside `src/index.js` the `App` component is imported and rendered to a DOM element with the id of root.

```jsx
ReactDOM.render(<App />, document.getElementById("root"));
```

This DOM element is found in `public/index.html`.

```html
<div id="root"></div>
```

`App` will be our parent component and all our other components will live inside it in a tree structure.
