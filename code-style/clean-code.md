# Clean code

#### Booleans

Booleans should always start with `is`, `has` or `should`

#### Prevent abbreviations

Variable or parameter names should _**never**_ be abbreviated.

Common pitfalls:

```jsx
function parseMsmnt(inc: Measurement) { // parseMeasurement(measurement: Measurement)
    try {
        const parsed = JSON.parse(measurement); // parsedMeasurement
        return parsed;
    } catch (e) { // error
        ...
    }
}

const [val, setVal] = useState(''); // value, or even better: describe what the value is
function handleChange(e) { // event
    setVal(e.target.value); // setValue
}
```

#### More reading

* [https://dev.to/michi/tips-on-naming-boolean-variables-cleaner-code-35ig](https://dev.to/michi/tips-on-naming-boolean-variables-cleaner-code-35ig)

TODO: try to avoid let -> use functions that return values

TODO: Max lines numbers per file

