
<p style="text-align: center; font-size: 30px; font-weight: bold">
    React for Senior Developers
</p>

## 1. Fundamentals
### 1.1 React Concept: What's the React? (or How to understand React?)
#### 1.1.1 One Sentence Explanation <br>
React is a JS library for building UI, try to resolve the reuse of view level through the components.<br>
So, its essential is a component framework, and its thinking model is:<br>

> View = fn (props, state, context)<br>

**fn**: Could be class component, pure function component, or side effect.<br>
There are only **components** in React, no pages, no controllers, no models.<br>
<br>

#### 1.1.2 It's **core concepts** are:<br>

- **Declarative**:<br>
Pretty straightforward, it's easy to understand and compose it. And making code more predictable and easier to debug. If using code illustration, you could find out the benefit as below:<br>

Change:
```html 
<div class="block" />
```
```js
const block = $('.block');
block.css('color', 'green');
```
to<br>
```js
const Block = (props) => <div style={{color: 'green'}} />;
```
- **Component-Based**:<br>
Build encapsulated components that manage their state, then compose them to make complex UIs. That means: low coupling in the system, high cohesion in each function.<br>

- **Learn Once, Write Anywhere**:<br>
No assumption about other technology stack, so you can develop new features in React without rewriting existing code. Meanwhile, React can render on server using Node, and power mobile apps using React Native(of course, React 360 for VR and Electron for desktop are the instances as well). Specificity, they are all benefit from the virtual DOM.<br>

#### 1.1.3 Disadvantage:<br>
React is just a library, not a comprehensive framework. Some spots, React doesn't implement them by itself, but leave them to the community, such as [React Route](https://reactrouter.com/en/main), [Component Test](https://www.freecodecamp.org/news/testing-react-hooks/). These increase the learning curve about he [Eco-System of React](#EcoSystem).

### 1.2 JSX
#### 1.2.1 One Sentence Explanation
JSX is a syntax sugar for Javascript, React doesn't force developer using JSX.<br>
We could implement React like below:
```js
class Hello extends React.Component {
    render() {
        return React.createElement('div', null, 'Hello ${this.props.toWhat}');
    }
}

ReactDOM.render(
    React.createElement(Hello, {toWhat: 'Hello'}, null),
    document.getElementById('root')
);
```
But with support of JSX, we could implement it like this:
```js
class Hello extends React.Component {
    render() {
        return <div>Hello ${this.props.toWhat}</div>;
    }
}

ReactDOM.render(
    <Hello toWhat="Hello" />,
    document.getElementById('root')
);
```
#### 1.2.2 Core Concept
React doesn't want to import too many new concept and just inherit from exiting JS syntax.<br>

#### 1.2.3 Solution Comparison (Separation of Concerns)
- Template: Bring lots of new concepts(like AngularJS) and weaken the separation of concerns.
- Template String: Bring complex structure description and no syntax prompt.
- JXON: Weak syntax prompt.

#### 1.2.4 How to convert JSX into JS through Babel
[How](https://legacy.reactjs.org/blog/2020/09/22/introducing-the-new-jsx-transform.html#:~:text=Browsers%20don't%20understand%20JSX,JSX%20transform%20under%20the%20hood.)
### 1.3 Life Cycle
### 1.4 Component Types
### 1.5 Design Patterns
## 2. State Management
## 3. Render Process
## 4. Performance Optimization
## 5. React Hooks
## 6. <a id="EcoSystem"></a>Eco-System of React
[Awesome-React](https://github.com/enaqx/awesome-react)
## 7. Perfect Resume