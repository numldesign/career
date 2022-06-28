# Test

### Implement a single Checkbox component that works in both controlled and uncontrolled mode.

- In unchecked state it has the following markup:

```<div class="checkbox"/>```

- In checked state:

```<div class="checkbox checked"/>```

The component has three properties: value?: boolean, defaultValue?: boolean and onChange?: (newValue: boolean) => void.

When value is specified the component works in the controlled mode. If the value is true then the component has a checked state and if the value is false then it has an unchecked state. If the user clicks the checkbox then the onChange callback is called with the argument that is opposite to the value property.

When defaultValue is specified the component works in the uncontrolled mode. It saves the initial value in its state. If the defaultValue is initially equal to true then the component has a checked initial state and if false then unchecked state. If the user clicks the checkbox then the checkbox state is changed to the opposite and the onChange callback is called with the argument that is equal to the new state.

Additional bonus tasks. Try to do at least 1-2 of them.

Implement checks for all possible incorrect property input, which could have places while using the component. Pay attention to Developer Experience. Please, ignore type-checking if you write JSX.
Implement the component in TypeScript. (Use can switch to TSX using toolbar in the top right corner of the coding area)
Implement the component using the input tag. (The use of the defaultChecked property is prohibited.)
Create an optimal implementation with minimum logical operations and re-renders.
Implement App component for checkbox manual testing in various cases. A single case is already declared in the code.
Criteria for evaluation:

Difficulty. The easier the code, the better.
Performance. The fewer operations and re-renders, the better.
Maintenance. The easier to maintain and expand the code, the better. Also, use best practices you know.
Developer Experience. The more convenient it is to use the component, the better.

// You can access React utilities as props of React object.
// For example: `React.useRef()`

function Checkbox({ value, defaultValue, onChange }) {
    return <div className="checkbox checked"/>
}

function App() {
    return <Checkbox value={true}/>
}

ReactDOM.render(<App/>, document.getElementById('app'));

// You can access React utilities as props of React object.
// For example: `React.useRef()`

interface CheckboxProps {
    value?: boolean;
    defaultValue?: boolean;
    onChange?: (newValue: boolean) => void;
}

function Checkbox({ value, defaultValue, onChange }: CheckboxProps) {    
    return <div className="checkbox checked"/>
}

function App() {
    return <Checkbox value={true}/>
}

ReactDOM.render(<App/>, document.getElementById('app'));

.checkbox {
    width: 16px;
    height: 16px;
    border-radius: 4px;
    border: 1px solid #333;
}

.checkbox.checked {
    background: #333;
    box-shadow: inset 0 0 0 2px white;
}
