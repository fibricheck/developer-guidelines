# Styled components

#### TODO: Change to backticks | Try to avoid vanilla css as much a spossible <a href="#styled-components" id="styled-components"></a>

#### Styled Components <a href="#styled-components" id="styled-components"></a>

For general styling, we make use of [`styled components`](https://www.styled-components.com/).\
We create a styled component using the object notation:

```tsx
const Container = styled.div({
  display: 'flex',
  height: '100%',
  paddingTop: '1px',
});
```

> As you can see, in object notation, the hyphens are omitted and replaced with camel cased words.

The spread operator can also be invoked for shared properties. We first create the shared property:

```tsx
const horizontalPadding = {
  padding: '0px 3px',
};
```

And we can then invoke it in other styled components like this:

```tsx
const GitBranchIcon = styled(GitBranch)({
  height: '21px',
  width: '12px',
  ...horizontalPadding,
});
```

We can also pass props to it:

```tsx
const Box = styled.h3((props) => ({
  height: '21px',
  width: '12px',
  color: props.checked ? 'green' : 'red',
}));
```

As a rule of thumb, we place all these styled components at the bottom of the file. This way, you have an overview of your code, without first scrolling trough all the styles.\
If there are too many styles, you can also put them in a separate file.

#### Global Styles <a href="#global-styles" id="global-styles"></a>

Global styles and colors that can be shared throughout the whole app should be placed in `styles/globalStyles.ts` ([https://styled-components.com/docs/api#createglobalstyle](https://styled-components.com/docs/api#createglobalstyle))

```tsx
import { createGlobalStyle } from 'styled-components'


// styles/globalStyles.ts
export const colors = {
  primary: '#fff',
  secondary: '#000'
}

export const GlobalStyles = createGlobalStyle({
  body {
    color: colors.secondary,
    backgroundColor: colors.primary,
  }
});

// App.tsx
import { GlobalStyles } from './styles/globalStyles.ts';

function App() {
  return (
    <main>
     <GlobalStyles />   
    </main>
  );
}
```

You can now also import colors with `import { colors } from './styles/globalStyles';`
