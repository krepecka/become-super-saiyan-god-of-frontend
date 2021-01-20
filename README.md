# Become Super Saiyan God of frontend development

![Alt Text](https://i.pinimg.com/originals/de/c5/fd/dec5fd7786b84a7455f95970bc5416a3.gif)

1. [JavaScript](#javascript)
1. [Browser](#browser)
1. [CSS](#css)
1. [React](#react)
1. [Tooling](#tooling)
1. [TypeScript](#ts)
1. [Security](#security)
1. [SEO](#seo)



## JavaScript <a name="javascript"></a>

Everything related to javascript execution, its running environment.

#### Engines

- [ ] V8 and alternatives
- [ ] deno

#### Language concepts

- [ ] Promises
- [ ] async/await
- [ ] `this` binding
- [ ] Type system
- [ ] scopes
- [ ] Objects
- [ ] Generators

#### Modules

- [ ] import/export
- [ ] ES6 modules
- [ ] CommonJS
- [ ] ..

#### Event loop

- [ ] Event loop
- [ ] Task queue
- [ ] Microtask queue

## Browser <a name="browser"></a>

#### HTTP Requests

- [ ] GET, PUT, POST, PATCH, OPTIONS, HEAD, DELETE
- [ ] HTTP request caching
- [ ] HTTP Request resolution
- [ ] low level request execution cycle
- [ ] Content-types
- [ ] MIME types

#### CDNs

What they are, what purpose do they serve, what are the capabilities.

#### Caching

Types/levels of caching, how does it work, clearing the cache..

#### DOM

#### Website rendering phases

- [ ] layout, painting...

#### Local/Session storage, cookies

Lifespan, use cases, concerns, API.

#### Performance

- [ ] critical rendering path
- [ ] service workers
- [ ] resource preloading
- [ ] image optimization
- [ ] bundle size optimizations
    - [ ] dynamic imports 
        - [ ] https://v8.dev/features/dynamic-import

#### Performance monitoring/tooling

What are common techniquest to monitor performance. What new tools there are.

- [ ] web vitals
- [ ] performance observers
- [ ] chrome developer tools
    - [ ] lighthouse
    - [ ] ..
    
#### Browser extensions

How to write them and how do they actually work.

#### Accessibility

- [ ] aria attributes
    - [ ] https://developers.google.com/web/fundamentals/accessibility
    - [ ] https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA
- [ ] semantic markup
- [ ] a11y testing
- [ ] a11y in React:
    - [ ] https://reactjs.org/docs/accessibility.html

## CSS <a name="css"></a>

- [ ] box model
- [ ] flex-box
- [ ] grid
- [ ] specificity rules 
    - [ ] https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity
- [ ] parsing/execution
- [ ] SCSS


## React <a name="react"></a>

#### React component lifecycle

- [ ] class components 
    - [ ] https://medium.com/better-programming/the-react-component-lifecycle-c9302202a69f
- [ ] hooks
    - [ ] .
    
 
#### React advanced API

- [ ] Code splitting
    - [ ] https://reactjs.org/docs/code-splitting.html
- [ ] Context
    - [ ] https://reactjs.org/docs/context.html
    - [ ] https://reactjs.org/docs/hooks-reference.html#usecontext useContext
- [ ] Error boundaries
    - [ ] https://reactjs.org/docs/error-boundaries.html
- [ ] Ref Forwarding
    - [ ] https://reactjs.org/docs/forwarding-refs.html
- [ ] HoC - outdated concept but still nice to know and understand the drawbacks
    - [ ] https://reactjs.org/docs/higher-order-components.html
- [ ] Integrating with other libraries
    - [ ] https://reactjs.org/docs/integrating-with-other-libraries.html
- [ ] jsx in depth
    - [ ] https://reactjs.org/docs/jsx-in-depth.html
- [ ] Optimizing performance
    - [ ] https://reactjs.org/docs/optimizing-performance.html
- [ ] Portals
    - [ ] https://reactjs.org/docs/portals.html
- [ ] Profiler
    - [ ] https://reactjs.org/docs/profiler.html
- [ ] React without ES6 and JSX - just for funs
    - [ ] https://reactjs.org/docs/react-without-es6.html
    - [ ] https://reactjs.org/docs/react-without-jsx.html
- [ ] Reconciliation
    - [ ] https://reactjs.org/docs/reconciliation.html
- [ ] Refs in DOM
    - [ ] https://reactjs.org/docs/refs-and-the-dom.html
- [ ] Render prop pattern
    - [ ] https://reactjs.org/docs/render-props.html
- [ ] Static type checking (focus on typescript)
    - [ ] https://reactjs.org/docs/static-type-checking.html#typescript
    - [ ] https://reactjs.org/docs/typechecking-with-proptypes.html
- [ ] Strict mode
    - [ ] https://reactjs.org/docs/strict-mode.html
- [ ] Uncontrolled components
    - [ ] https://reactjs.org/docs/uncontrolled-components.html
- [ ] Webcomponents and React
    - [ ] https://reactjs.org/docs/web-components.html
- [ ] Suspense 
    - [ ] https://reactjs.org/docs/concurrent-mode-suspense.html



#### Server side rendering

- [ ] ReactDomServer
    - [ ] https://reactjs.org/docs/react-dom-server.html
- [ ] Hydration
    - [ ] https://reactjs.org/docs/react-dom.html#hydrate
- [ ] Tutorial
    - [ ] https://flaviocopes.com/react-server-side-rendering/

#### Hooks

- [ ] Intro
    - [ ] https://reactjs.org/docs/hooks-intro.html
    - [ ] Dan's video
    - [ ] https://reactjs.org/docs/hooks-overview.html
- [ ] useState
    - [ ] https://reactjs.org/docs/hooks-state.html
    - [ ] https://reactjs.org/docs/hooks-reference.html#usestate
- [ ] useEffect
    - [ ] https://reactjs.org/docs/hooks-effect.html
    - [ ] https://reactjs.org/docs/hooks-reference.html#useeffect 
- [ ] Other hooks
    - [ ] useRef https://reactjs.org/docs/hooks-reference.html#useref
    - [ ] useContext https://reactjs.org/docs/hooks-reference.html#usecontext
    - [ ] useCallback https://reactjs.org/docs/hooks-reference.html#usecallback
    - [ ] useReducer https://reactjs.org/docs/hooks-reference.html#usereducer
    - [ ] useMemo https://reactjs.org/docs/hooks-reference.html#usememo
    - [ ] useImperativeHandle https://reactjs.org/docs/hooks-reference.html#useimperativehandle
    - [ ] useLayoutEffect https://reactjs.org/docs/hooks-reference.html#uselayouteffect
    - [ ] useDebugValue https://reactjs.org/docs/hooks-reference.html#usedebugvalue
- [ ] Rules of hooks
    - [ ] https://reactjs.org/docs/hooks-rules.html
- [ ] Custom hooks
    - [ ] https://reactjs.org/docs/portals.html
- [ ] Hooks FAQ
    - [ ] https://reactjs.org/docs/hooks-faq.html

#### Concurrent mode

- [ ] https://reactjs.org/docs/concurrent-mode-intro.html

#### Server components

- [x] Intro
    - [x] https://reactjs.org/blog/2020/12/21/data-fetching-with-react-server-components.html
- [ ] Demo example 
    - [ ] https://github.com/reactjs/server-components-demo
- [ ] RFC
    - [ ] https://github.com/josephsavona/rfcs/blob/server-components/text/0000-server-components.md

#### React testing

- [ ] https://reactjs.org/docs/testing.html

## Tooling <a name="tooling"></a>

Linters, transpilers..

#### webpack
- [ ] Plugins
- [ ] Federation
- [ ] New versions of webpack

#### storybook (building component libraries)

## TypeScript <a name="ts"></a>

- [ ] Handbook
    - [ ] https://www.typescriptlang.org/docs/handbook/intro.html
- [ ] Kent C Dodds said to read about narrowing
    - [ ] https://www.typescriptlang.org/docs/handbook/2/narrowing.html


## Security <a name="security"></a>

What types of vurnerabilities there are, have been in the past, best practices.


## SEO <a name="seo"></a>
