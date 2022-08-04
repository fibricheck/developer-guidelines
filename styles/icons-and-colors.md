# Icons and colors

#### Icons <a href="#icons" id="icons"></a>

We usually use icons from [`styled-icons`](https://github.com/jacobwgillespie/styled-icons) library, which is a combination of different icon sources.

TODO: Add example | Check which lib!

#### Colors

Colors should always be given a meaningful name:

```tsx
// Don't do this
export const colors = {
  white: '#fff',
  black: '#000',
  lightGray: '#f3f3f3'
}

// Do this instead
export const colors = {
  primary: '#fff',
  secondary: '#000',
  border: '#f3f3f3'
}
```

