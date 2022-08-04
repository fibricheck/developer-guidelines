# State management

#### Redux Toolkit

For large projects with large state trees and many side effects, we recommend using Redux. Your first choice should always be [Redux Toolkit](https://redux-toolkit.js.org/). It's an opinionated, typescript supported library that reduces Redux boilerplate and has many built-in helpers for managing side effects.&#x20;

#### Redux Sagas

For some of our more complex projects, Redux Sagas was a better choice for managing side effects. Although Redux Toolkit [promises to replace Redux Sagas with its listener middleware](https://github.com/reduxjs/redux-toolkit/releases/tag/v1.8.0) so this might no longer be applicable.
