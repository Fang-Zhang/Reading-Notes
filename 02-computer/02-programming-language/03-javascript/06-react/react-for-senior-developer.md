<p style="text-align: center; font-size: 30px; font-weight: bold">
    React for Senior Developers
</p>

## 1. Component Fundamentals
### 1.1 React Fundamentals: What's the React? (or How to understand React?)
#### 1.1.1 Concept:
React is a JS library for building UI. It's thinking model is:<br>

> View = fn (props, state, context)<br>

**fn**: Could be class component, pure function component, or side effect<br>
There are only **components** in React, no pages, no controllers, no models.<br>
<br>

It's **core concepts** are:<br>

**Declarative**:<br>
Design simple views for each state in application, making code more predictable and easier to debug. If using code illustration, you could find out the benefit as below:<br>

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
**Component-Based**:<br>
Build encapsulated components that manage their state, then compose them to make complex UIs. That means: low coupling in the system, high cohesion in each function.<br>

**Learn Once, Write Anywhere**:<br>
No assumption about other technology stack, so you can develop new features in React without rewriting existing code. Meanwhile, React can render on server using Node, and power mobile apps using React Native. Specificity, virtual DOM helps all React developers out from the DOM-Operation directly.<br>

#### 1.1.2 Disadvantage:
React is just a library, not a comprehensive framework. Some spots, React doesn't implement them by itself, such as Route, State Management. These increase the learning curve about he [Eco-System of React](#EcoSystem).

### 1.2 JSX
### 1.3 Life Cycle
### 1.4 Component Types
### 1.5 Design Patterns
## 2. Statement Management
## 3. Render Process
## 4. Performance Optimization
## 5. React Hooks
## 6. <a id="EcoSystem"></a>Eco-System of React
## 7. Perfect Resume