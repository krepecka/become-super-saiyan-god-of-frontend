# Become Super Saiyan God of frontend development

![Alt Text](https://i.pinimg.com/originals/de/c5/fd/dec5fd7786b84a7455f95970bc5416a3.gif)

1. [Ecosystem Y2023](#ecosystem)
1. [JavaScript](#javascript)
1. [Browser](#browser)
1. [Performance](#perf)
1. [CSS](#css)
1. [React](#react)
1. [Tooling](#tooling)
1. [TypeScript](#ts)
1. [GraphlQL](#graphql)
2. [Blockchain development](#dapps)
3. [Security](#security)
4. [SEO](#seo)
5. [Misc](#misc)

## Ecosystem Y2023+ <a name="ecosystem"></a>

<details>
  <summary>Going into Y2023 it really feels like the FE development landscape is becoming more mature and stable. There qre quite distinct winners and losers in various framework and library races (React vs the field, typescript over flow). This section lists libraries and frameworks that on should be familiar with or which would be useful when starting a new project.</summary>
  
  - svelte, solidjs as new players in the UI framework scena
  - nextjs or remix for react meta framework
  - zodjs for type safe schemas https://github.com/colinhacks/zod   


</details>

## JavaScript <a name="javascript"></a>



<details>
  <summary>Everything related to javascript features, execution, its running environment.</summary>
  
#### Engines

- [ ] More generic JS engine (V8) overview 
  - [x] Just In Time (JIT) explained as a concept https://www.freecodecamp.org/news/just-in-time-compilation-explained/
  - [x] JIT crash course https://hacks.mozilla.org/2017/02/a-crash-course-in-just-in-time-jit-compilers/
    <details>
      <summary>summary</summary>
  
      - baseline compiler to have a baseline compiled versions for warm code
      - optimized compiler to have very optimized versions for hot code
    </details>
  - [x] Overview of JS engines https://blog.bitsrc.io/javascript-engines-an-overview-2162bffa1187
- [ ] V8 concepts and articles **this blog https://v8.dev/blog**
  - [x] First 10 years of V8 development https://v8.dev/blog/10-years
  - [x] React performance cliff (V8 internals explained: SMI and HeapNumbers, Shape chaining optimization) https://v8.dev/blog/react-cliff
  - [ ] Shapes and inline caches (basically about the same thing as :point_up:) https://mathiasbynens.be/notes/shapes-ics
  - [ ] Prototype optimization in V8 (similar to :point_up:) https://mathiasbynens.be/notes/prototypes
  - [ ] V8 background compilation https://v8.dev/blog/background-compilation
  - [ ] Code coverage https://v8.dev/blog/javascript-code-coverage
  - [ ] The cost of JS in 2019 https://v8.dev/blog/cost-of-javascript-2019
  - [x] V8 releaso of V8.9 (2021-02) https://v8.dev/blog/v8-release-89
    <details>
      <summary>summary</summary>
  
      - top level await under a feature flag
      - optimization for functions with argument mismatch
    </details>
  - [ ] Faster `super` calls https://v8.dev/blog/fast-super
  - [ ] Async stack traces https://mathiasbynens.be/notes/async-stack-traces
- [ ] WASM
  - [ ] https://hacks.mozilla.org/2017/02/a-cartoon-intro-to-webassembly/
- [x] AST explorer https://astexplorer.net/
- [ ] deno
  - [ ] https://www.youtube.com/watch?v=puXyo1jGQys

#### Language concepts

- [ ] Promises
  - [x] MDN https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise
    <details>
      <summary>summary</summary>
  
      - Promise can be one of `fulfilled|rejected|pending`.
      - Every Promise is thennable.
      - Promise can only be settled once. Subsequent `reject()` and `resolve` calls are ignored.
      - Resolved promise must have a value (can be `undefined`).
      - then accepts two arguments: `then(onFulfilled, onRejected)` functions.
      - then returns a promise. If it's a value - it is wrapped in Promise.resolve()
      - `Promise` is a global object
      - `Promise.all` and `Promise.race`
    </details>
  - [x] Popular medium article https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261
- [ ] async/await
  - [x] async https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function
    <details>
      <summary>summary</summary>
  
      ![image](https://user-images.githubusercontent.com/17677991/112530837-94318a80-8daf-11eb-82a5-2403e4e1f10a.png)
    </details>

  - [x] await https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await
    <details>
      <summary>summary</summary>
  
      ![image](https://user-images.githubusercontent.com/17677991/112530755-7e23ca00-8daf-11eb-8faf-86ffc67fd0e6.png)
    </details>

  - [ ] both https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Async_await
  - [ ] medium https://medium.com/javascript-in-plain-english/async-await-javascript-5038668ec6eb
- [ ] Behavior of `this` 
  - [ ] https://github.com/getify/You-Dont-Know-JS/blob/1st-ed/this%20%26%20object%20prototypes/ch1.md
  - [ ] https://github.com/getify/You-Dont-Know-JS/blob/1st-ed/this%20%26%20object%20prototypes/ch2.md
  - [ ] https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this
- [ ] Type system
  - [ ] undefined vs null revisted https://2ality.com/2021/01/undefined-null-revisited.html
  - [ ] Wrapped objects for primitive values https://2ality.com/2022/02/wrapper-objects.html
- [ ] scopes
  - [ ] Scopes and hoisting https://livecodestream.dev/post/understanding-variables-scope-and-hoisting-in-javascript/
  - [ ] Temporal dead zone https://www.freecodecamp.org/news/what-is-the-temporal-dead-zone/
  - [ ] Closures https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36
  - [ ] try/catch scope
- [ ] Streams https://web.dev/streams/
- [ ] Objects
- [ ] Generators
- [ ] Prototypes https://github.com/getify/You-Dont-Know-JS/blob/1st-ed/this%20%26%20object%20prototypes/ch5.md
- [ ] Class vs. prototypal inheritance https://medium.com/javascript-scene/master-the-javascript-interview-what-s-the-difference-between-class-prototypal-inheritance-e4cd0a7562e9
- [ ] Regular expressions
- [ ] Math and Number system
  - [ ] https://javascript.info/number
  - [ ] https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math
- [ ] Proxies https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Proxy



#### Patterns - existing constructs

- [ ] Pure functions https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-pure-function-d1c076bec976
- [ ] Higher order functions 
  - [ ] https://eloquentjavascript.net/05_higher_order.html
  - [ ] https://blog.bitsrc.io/understanding-higher-order-functions-in-javascript-75461803bad
- [ ] Feature detection
  - [ ] https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/Feature_detection
  - [ ] Writing polyfills https://addyosmani.com/blog/writing-polyfills/
- [ ] Method chaining https://medium.com/backticks-tildes/understanding-method-chaining-in-javascript-647a9004bd4f

#### Modules

- [x] MDN overview https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules
  <details>
      <summary>summary</summary>
  
    - top level await available
    - strict mode by default
    - `<script type="module"` is deferred by default
  </details>
- [x] JS modules and V8 deep dive https://v8.dev/features/modules
- [x] simple api overview https://www.carlrippon.com/javascript-modules-in-2020/
- [ ] cartoon deep dive https://hacks.mozilla.org/2018/03/es-modules-a-cartoon-deep-dive/
- [ ] in depth https://hacks.mozilla.org/2015/08/es6-in-depth-modules/
- [x] Dynamic imports https://v8.dev/features/dynamic-import
    - returns a promise `import()` is not a function - bracket are part of the syntax

#### Event loop

- [ ] Event loop
  - [ ] That yt video https://www.youtube.com/watch?v=8aGhZQkoFbQ
  - [ ] https://nodesource.com/blog/event-loop-utilization-nodejs
- [ ] Message queue
  - [ ] https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop
- [ ] Microtask queue
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/HTML_DOM_API/Microtask_guide/In_depth

#### New ECMAScript features

- [ ] 2020 https://2ality.com/2019/12/ecmascript-2020.html
  
</details>

## Browser <a name="browser"></a>


<details>
  <summary>Browser related tech.</summary>
  
  
#### Browser APIs

- [ ] Notifications
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API/Using_the_Notifications_API
  - [ ] https://developers.google.com/web/fundamentals/push-notifications
- [ ] Service workers
  - [ ] https://developers.google.com/web/fundamentals/primers/service-workers
- [ ] Web workers
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers
  - [ ] https://web.dev/off-main-thread/
- [ ] IndexedDB
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API/Using_IndexedDB
- [ ] CacheStorage
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/CacheStorage
- [ ] LocalStorage
- [ ] SessionStorage
- [ ] Temporal API
- [ ] Intl
- [ ] WebGL
- [ ] WebRTC
- [ ] WebSockets
- [ ] Broadcast channel API
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/Broadcast_Channel_API
- [ ] Geolocation API
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API
- [ ] FileSystem Access API
  - [ ] https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API
- [ ] WebXR API 
- [ ] Drag and Drop API
- [ ] Web speech API

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

- [ ] HTTP caching https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching

#### DOM

 - [ ] Event propagation and bubbling

#### Website rendering phases

- [ ] layout, painting...

#### Local/Session storage, cookies

Lifespan, use cases, concerns, API.
    
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
  
#### Misc
  
- [ ] Send requests on page navigation https://css-tricks.com/send-an-http-request-on-page-exit/ (Beacon API, fetch keepalive)
    
</details>

## Performance <a name="perf"></a>

<details>
  <summary>Perf deserves its own section.</summary>
  
#### Performance

- [ ] critical rendering path
  - [ ] https://web.dev/long-tasks-devtools/ 
- [ ] service workers
- [ ] resource loading
  - [ ] script attributes https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script#attributes
  - [ ] prefetch https://web.dev/link-prefetch/
  - [ ] preload https://web.dev/preload-critical-assets/
- [ ] image optimization
- [ ] bundle size optimizations
    - [ ] dynamic imports 
        - [ ] https://v8.dev/features/dynamic-import
- [ ] load on interaction (lazy loading) https://addyosmani.com/blog/import-on-interaction/
- [ ] **Perf beyond bundle size**
  - [ ] https://nolanlawson.com/2021/02/23/javascript-performance-beyond-bundle-size/
- [ ] Code caching after execution https://v8.dev/blog/v8-release-66#code-caching-after-execution
- [ ] Code caching V8 https://v8.dev/blog/code-caching-for-devs
- [ ] Fixing memory leaks https://nolanlawson.com/2020/02/19/fixing-memory-leaks-in-web-applications/

#### Performance monitoring/tooling

What are common techniquest to monitor performance. What new tools there are.

- [ ] web vitals
- [ ] performance observers
- [ ] user timing API https://developer.mozilla.org/en-US/docs/Web/API/User_Timing_API
- [ ] chrome developer tools
    - [ ] lighthouse
    - [ ] ..
  
</details>

## CSS <a name="css"></a>

<details>
  <summary>CSS - you have to know it.</summary>

- [ ] High performance animations https://www.html5rocks.com/en/tutorials/speed/high-performance-animations/
- [ ] box model
- [ ] flex-box
- [ ] grid
- [ ] specificity rules 
    - [ ] https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity
- [ ] parsing/execution
  - [ ] Aimee Knight on internals: https://www.youtube.com/watch?v=eajyNEsdx4k
- [ ] SCSS
- [ ] Styled components https://www.joshwcomeau.com/css/styled-components/

</details>


## React <a name="react"></a>


<details>
 <summary>React</summary>

#### React component lifecycle

- [ ] class components 
    - [ ] https://medium.com/better-programming/the-react-component-lifecycle-c9302202a69f
- [ ] hooks
    - [x] https://reactjs.org/docs/hooks-overview.html
    - [ ] https://reactjs.org/docs/hooks-rules.html
    
 
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
- [x] Using `key` prop to control component instances
  - [x] https://kentcdodds.com/blog/understanding-reacts-key-prop



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
    - [x] https://reactjs.org/docs/hooks-state.html
    - [x] https://reactjs.org/docs/hooks-reference.html#usestate
      - prevValue func; setState identity guaranteed the same; Object.is to bail out of render; can use lazy initialization
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
    - [ ] unstable_useSelectedContext https://github.com/facebook/react/pull/20646
- [ ] Rules of hooks
    - [ ] https://reactjs.org/docs/hooks-rules.html
- [ ] Custom hooks
    - [ ] https://reactjs.org/docs/portals.html
- [ ] Hooks FAQ
    - [ ] https://reactjs.org/docs/hooks-faq.html

#### Concurrent mode

- [x] https://reactjs.org/docs/concurrent-mode-intro.html
- [x] Suspense for data fetching
- [x] API reference https://reactjs.org/docs/concurrent-mode-reference.html
- [x] useTransition hook https://reactjs.org/docs/concurrent-mode-patterns.html
```javascript
const [startTransition, isPending] = useTransition({
   timeoutMs: 3000
});
```

#### Server components

- [x] Intro https://reactjs.org/blog/2020/12/21/data-fetching-with-react-server-components.html
- [x] Demo example https://github.com/reactjs/server-components-demo
- [ ] RFC (Detailed implementation) https://github.com/josephsavona/rfcs/blob/server-components/text/0000-server-components.md

#### React testing

- [ ] https://reactjs.org/docs/testing.html

#### React official blog

https://reactjs.org/blog/all.html

</details>

## Tooling <a name="tooling"></a>


<details>
  <summary>Linters, transpilers.. The ecosystem is bigger than you thought.</summary>
  
#### Electron
  

#### webpack
- [ ] Plugins
- [ ] Federation
- [ ] New versions of webpack

#### storybook (building component libraries)

#### Remotion - videos ir React

https://youtu.be/szh2Qgo9SVE

</details>

## TypeScript <a name="ts"></a>

<details>
  <summary>The necessary evil(?)</summary>

- [ ] Handbook
    - [ ] https://www.typescriptlang.org/docs/handbook/intro.html
- [ ] Kent C Dodds said to read about narrowing
    - [ ] https://www.typescriptlang.org/docs/handbook/2/narrowing.html
- [x] Using union types to avoid impossible states
  - [x] https://zohaib.me/leverage-union-types-in-typescript-to-avoid-invalid-state/
  - [x] https://dev.to/housinganywhere/matching-your-way-to-consistent-states-1oag
    
- [ ] https://startup-cto.net/10-bad-typescript-habits-to-break-this-year/

</details>

## GraphQL <a name="graphql"></a>

<details>
  <summary>GraphQL</summary>

#### Relay

- [ ] Relay hooks https://relay.dev/blog/2021/03/09/introducing-relay-hooks/

</details>


## Blockchain development <a name="dapps"></a>

<details>
  <summary>ETH to the moon 🚀</summary>

#### dapp tutorials 
- [x] Simple todo dapp tutorial https://www.youtube.com/watch?v=coQ5dg8wM2o
- [x] ERC721 tokens https://www.youtube.com/watch?v=YPbgjPPC1d0

#### Ethereum stack
- [ ] Intro https://ethereum.org/en/developers/docs/intro-to-ethereum/
- [ ] Smart contracts
- [ ] Solidity
- [ ] Events and Logs https://medium.com/linum-labs/everything-you-ever-wanted-to-know-about-events-and-logs-on-ethereum-fec84ea7d0a5

#### Specific dev tech
- [ ] Hardhat https://hardhat.org/
- [ ] ethers.js https://docs.ethers.io/v5/
- [ ] ethereum waffle https://github.com/EthWorks/Waffle
- [ ] web3.js https://web3js.readthedocs.io/en/v1.3.4/
- [ ] metamask https://docs.metamask.io/guide/

</details>


## Security <a name="security"></a>

What types of vurnerabilities there are, have been in the past, best practices.

## SEO <a name="seo"></a>

## MISC  <a name="misc"></a>

#### Articles

- [ ] https://artsy.github.io/blog/2021/03/09/strategies-for-small-focused-pull-requests/
- [ ] https://timdaub.github.io/2021/01/16/web-principles/
- [ ] axios over fetch ? https://betterprogramming.pub/why-javascript-developers-should-prefer-axios-over-fetch-294b28a96e2c
- [ ] use `pipe` https://www.obvibase.com/dev-blog/i-ve-used-the-pipe-function-2-560-times-and-i-can-tell-you-it-s-good
- [ ] ES2021 features https://2ality.com/2020/09/ecmascript-2021.html
- [x] ORM overview 2021 https://www.sitepoint.com/javascript-typescript-orms/
- [x] Elaborate article on ternary operator vs if statement https://jrsinclair.com/articles/2021/rethinking-the-javascript-ternary-operator/
- [x] Svelte vs React in 2021 https://www.jackfranklin.co.uk/blog/comparing-svelte-and-react-javascript/
- [ ] State library comparison https://daveceddia.com/react-state-management/

#### Tutorials

- [ ] Fixing memory leaks https://nolanlawson.com/2020/02/19/fixing-memory-leaks-in-web-applications/
- [x] You don't need all that JS, I Promise https://www.youtube.com/watch?v=e1L2WgXu2JY
  - tl;dr keep up with new browser, html, css apis. For example < portal />
- [x] JS Features to forget https://davidflanagan.com/2020/05/12/javascript-to-forget.html
- [ ] Kent builds **modern website in 2021** https://kentcdodds.com/blog/how-i-built-a-modern-website-in-2021

#### Interesting stuff

- [x] What to pay JS devs https://medium.com/javascript-scene/what-to-pay-javascript-developers-in-2020-2292eb346f3b
- [ ] Mindblowers https://github.com/denysdovhan/wtfjs#readme
- [ ] 150 questions https://github.com/lydiahallie/javascript-questions#readme
- [ ] Goodbye, clean code by Dan https://overreacted.io/goodbye-clean-code/
- [x] How much you'd save with modern javascript https://estimator.dev/
- [ ] Rising starts 2021 https://risingstars.js.org/2020/en

#### Tools
  
- [ ] Package your node.js app into executable https://github.com/vercel/pkg
- [ ] Introduce new users to your website https://introjs.com/
  
https://web.dev/learn/ - should fill in a lot of gaps.



