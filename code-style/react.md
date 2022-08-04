# React

#### Components <a href="#components" id="components"></a>

As a rule of thumb, try to make a component as dumb as possible. Heave computation should happen in the backend or in your state management layer.

**Functional Components**

Never use Class components, function components should always be used.

#### Always use constants

```jsx
// instead of
function PurchaseStatus({ purchaseStatus }: Props) {
    return (
        <article>
            {purchaseStatus === 'purchased' && <p>Purchased</p>}
        </article>
    )
}

// do this
import { PURCHASE_STATUS } from '../utils/constants';

function PurchaseStatus({ purchaseStatus }: Props) {
    return (
        <article>
            {purchaseStatus === PURCHASE_STATUS.purchased && <p>Purchased</p>}
        </article>
    )
}
```



TODO: use enums for these cases - Singular - Uppercase + example

properties op enum -> camel case

#### State management <a href="#store" id="store"></a>

[See the state management guide.](../styles/styled-components.md)

****
