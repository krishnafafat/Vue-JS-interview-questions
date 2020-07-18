
---

<div align="center">
    <p>Vuejs Technical Interview Questions & Answered</p>
</div>

---

### Table of Contents

| No. | Questions |
| --- | --------- |
|1  | [What is Vue?](#what-is-Vue) |
|2  | [What is advantages of Vue?](#What-is-advantages-of-Vue) |
|3  | [Explain Vue reactivity and common issues when tracking changes?](#Explain-Vue-reactivity-and-common-issues-when-tracking-changes) |
|4  | [What is the virtual DOM and how is it beneficial?](#what-is-the-virtual-DOM-and-how-is-it-beneficial) |
|5  | [What are Components in Vue](#what-are-Components-in-Vue) |
|6  | [Why do we need local registration?](#Why-do-we-need-local-registration) |
|7  | [What are list of features in Vue](#what-are-list-of-features-in-Vue) |
|8  | [What are the event modifiers available in Vue](#what-are-the-event-modifiers-available-in-Vue) |
|9  | [Explain how can we work with binding inline styles?](#Explain-how-can-we-work-with-binding-inline-styles) |
|10  | [List type of Directive are available in Vuejs?](#List-type-of-Directive-are-available-in-Vuejs) |
|11  | [What are Directives in Vue and List some of them you used?](#What-are-Directives-in-Vue-and-List-some-of-them-you-used) |
|12  | [What is Vue loader?](#what-is-Vue-loader) |
|13  | [How will you render the original HTML in the template?](#How-will-you-render-the-original-HTML-in-the-template) |
|14  | [Explain lifecycle hooks in vue?](#Explain-lifecycle-hooks-in-vue) |
|15  | [How to listen to events?](#How-to-listen-to-events) |
|16  | [Which lifecycle hook is most suitable for getting data from API calls?](#Which-lifecycle-hook-is-most-suitable-for-getting-data-from-API-calls) |
|17  | [When is the updated lifecycle hook called?](#When-is-the-updated-lifecycle-hook-called) |
|18  | [Why not use the arrow function when writing a lifecycle hook or other option or property in a Vue instance?](#Why-not-use-the-arrow-function-when-writing-a-lifecycle-hook-or-other-option-or-property-in-a-Vue-instance) |
|19  | [What is asynchronous component?](#what-is-asynchronous-component) |
|20  | [What are rendering functions? for instance](#what-are-rendering-functions-for-instance) |
|21  | [What is mixin?](#what-is-mixin) |
|22  | [How does prop specify its type requirements?](#How-does-prop-specify-its-type-requirements) |
|23  | [What is the difference between v-show and v-if directives?](#What-is-the-difference-between-v-show-and-v-if-directives) |
|24  | [What is Vue Router?](#what-is-Vue-Router) |
|25  | [What is parent in Vue?](#what-is-parent-in-Vue) |
|26  | [What is key in Vue?](#what-is-key-in-Vue) |
|27  | [What is the role of ref in Vue?](#what-is-the-role-of-ref-in-Vue) |
|28  | [What is Vue props?](#what-is-Vue-props) |
|29  | [How do you set up a Webpack in Vue?](#How-do-you-set-up-a-Webpack-in-Vue) |
|30  | [What is slot and slot-scoped in Vue?](#what-is-slot-and-slot-scoped-in-Vue) |
|31  | [What are the conditional directives in Vue?](#what-are-the-conditional-directives-in-Vue) |
|32  | [What is vue instance?](#what-is-vue-instance) |
|33  | [What is Vue CLI tool?](#what-is-Vue-CLI-tool) |
|34  | [How we can bind HTML classes in Vue JS?](#How-we-can-bind-HTML-classes-in-Vue-JS) |
|35  | [How to create Two-way binding?](#How-to-create-Two-way-binding) |
|36  | [What are filters in Vue js?](#what-are-filters-in-Vue-js) |
|37  | [When to use keep-alive component?](#When-to-use-keep-alive-component) |
|38  | [What are the properties of a Vue instance?](#what-are-the-properties-of-a-Vue-instance) |
|39  | [What are built-in components?](#what-are-built-in-components) |
|40  | [What is event key modifiers?](#what-is-event-key-modifiers) |
|41  | [How to modify event?](#How-to-modify-event) |


1. ### What is Vue?

   Vue is a **progressive framework** used to building user interfaces. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects.


   **[⬆ Back to Top](#table-of-contents)**

2. ### What is advantages of Vue?

   1. **Small in size** — The size of Vue framework is 18 to 21KB and it takes no time for the user to download and use it.
   2. **Easy to Understand** — One of the reasons for the popularity of this framework is that it is quite easy to understand. The user can easily add Vue.js to his web project because of its simple structure.
   3. **Simple Integration** — Vue.js can be integrated with the existing applications easily.
   4. **Flexibility** — This flexibility also makes it easy to understand for the developers of React.js, Angular.js, and any other new JavaScript framework.
   5. **Virtual DOM** — It uses virtual DOM similar to other existing frameworks such as ReactJS, Ember etc. Virtual DOM is a light-weight in-memory tree representation of the original HTML DOM and updated without affecting the original DOM.
   6. **Components** — Used to create reusable custom elements in VueJS applications.
   7. **Two-Way Communication** — Vue.js also facilitates two way communications because of its MVVM architecture which makes it quite easy to handle HTML blocks.


   **[⬆ Back to Top](#table-of-contents)**

3. ### Explain Vue reactivity and common issues when tracking changes?

   All properties defined in a Vue instance’s data option are reactive, meaning that if they change, the component is automatically updated and re-rendered as needed.
   All such properties are converted to getters and setters during initialization, thus allowing Vue to detect when those properties are accessed or changed.
   The following limitations must be accounted for when designing a Vue app:

   Vue cannot detect object property addition or deletion due to a JavaScript limitation, so the Vue.set method must be used to add new root-level reactive properties.
   Similarly, Vue cannot detect when an array item is modified using an index. Vue.set must be used here as well.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is the virtual DOM and how is it beneficial?

   The **virtual DOM** is a tree-like data structure (or a collection) of JavaScript objects representing DOM nodes that are managed by Vue.js and that should be rendered on the page. These objects are called “virtual nodes” or VNodes for short.

   The main purpose of the virtual DOM is faster and more efficient DOM manipulation. When there are lots of nodes in the DOM, updating them can be expensive in terms of processing power and resources required.

   Working with the virtual DOM JavaScript object is significantly faster. Subsequently, Vue.js organizes DOM updates in batches for more efficiency.

   **[⬆ Back to Top](#table-of-contents)**

5. ### What are Components in Vue?

   Components are one of most powerful features of Vue js.In Vue components are custom elements that help extend basic HTML elements to encapsulate reusable code.

   Following is the way to register a Vue component inside another component:

   ```
    export default {
      el: '#your-element',
      components: {
          'your-component'
      }
    }
   ```

   **[⬆ Back to Top](#table-of-contents)**

6. ### Why do we need local registration?

   Global registration often isn’t ideal. For example, if we are using a build system like Webpack, globally registering all components means that even if we stop using a component, it could still be included in our final build. This unnecessarily increases the amount of JavaScript your users have to download. In these cases, you can define your components as plain JavaScript objects:

   ```
    const ComponentA =  {/* ..... */}
    const ComponentB =  {/* ..... */}
    const ComponentC =  {/* ..... */}
   ```
   Then define the components you’d like to use in a components option:  

   ```
    export default {
      el: '#app',
      components: {
          'component-a': 'ComponentA',
          'component-b': 'ComponentB',
          'component-c': 'ComponentC',
      }
    }
   ```

   **[⬆ Back to Top](#table-of-contents)**

7. ### What are list of features in Vue?

   Vue js comes with following features

    1. **Templates**
    2. **Reactivity**
    3. **Components**
    4. **Transitions**
    5. **Routing**


   **[⬆ Back to Top](#table-of-contents)**

8. ### What are the event modifiers available in Vue?

   The list of available event modifiers is given below:

   1. stop
   2. prevent
   3. capture
   4. self
   5. once
   6. passive


   **[⬆ Back to Top](#table-of-contents)**

9. ### Explain how can we work with binding inline styles?

   V-bind: style can be used as a code that is straightforward in inline style binding. The look is closely similar to CSS except for its JavaScript feature. Either kebab-case or camelCase can be used for the CSS property names. Shown below is a sample snippet code:

   ```
      <div v-bind:style="{ color: activeColor, fontSize: fontSize + 'px' }"></div>
      data: {
      activeColor: 'red',
      fontSize: 30
      }
   ```


   **[⬆ Back to Top](#table-of-contents)**

10. ### List type of Directive are available in Vuejs?

    Following is list of directives available in Vue.js:

    1. **Empty Directives** - Empty directives do not require and will ignore their attribute value. e.g. v-pre(skip) and v-cloak (display: none).

    ```
        <div v-pre>
        <!-- markup in here will not be compiled -->
        </div>
    ```
    2. **Custom Directive** - Vue also allows us to register our own custom directives aside the default set of directives that are shipped in core (v-show and v-model). In Vue 2.0, the primary code reuse and abstraction is components- however there may be cases where we need some low-level DOM access on plain elements, custom directives will still be useful here. A typical example would be focusing on an input element, like an input text.

    On page load, the element gains focus (Note: autofocus does not work on mobile safari). If one has not clicked on anything else since visiting the page, the text input should be focused. Let us build the directive that will accomplish this:

    ```
    // Registering a global custom directive called `v-focus`
    Vue.directive('focus', {
      // When the bound element is inserted into the DOM...
      inserted: function (el) {
        // Focus the element
        el.focus()
      }
    })
    ```
    Instead if we want to register a directive locally, components accept directives option as well:
    ```
    directives: {
      focus: {
        // directive definition
        inserted: function (el) {
          el.focus()
        }
      }
    }
    ```
    Then we can now use the new v-focus attribute on any element in our template as shown:
    ```
    <input v-focus>
    ```
    Hook Functions

    Several hook functions can be provided by a directive's definition object:

    1. **bind**: This is called only once, when the directive is first bound to the element. This is where we can do one-time setup work.
    2. **inserted**: This is called when the bound element has been inserted into its parent node (this only guarantees the parent node presence, not necessarily in-document).
    3. **update**: This is called after the containing component's VNode has updated, but possibly before the update of its children. The value of the directive may or may not have changed, but we can skip unnecessary updates by comparing the binding's current and old values (see hook arguments below).
    4. **componentUpdated**: This is called after the containing component's VNode and the VNodes of its children have updated.
    5. **unbind**: This is called only once, when the directive is unbound from the element.

    ![custom directives hook](images/custom-directives-flat.jpg)

    3. **Literal Directives** - Some directives don’t create data bindings - they simply take the attribute value as a literal string. For example the v-component directive:

      ```
        <div v-component="my-component"></div>
      ```
    Here "my-component" is not a data property - it’s a string ID that Vue.js uses to lookup the corresponding Component constructor.

    4. **General Directives** -


    **[⬆ Back to Top](#table-of-contents)**

11. ### What are Directives in Vue and List some of them you used?

    Directives in Vue.js extend HTML with attributes and tags. Vue.js has built-in directives, but you can also make your custom directives. Following is a list of some directives used:

    1. v-else
    2. v-on
    3. v-model
    4. v-show
    5. v-if


    **[⬆ Back to Top](#table-of-contents)**

12. ### What is Vue loader?

    Vue loader is the loader module of webpack, which enables us to write single file components in. Vue file format. A single file component file has three parts: template, script, and style. The Vue loader module allows webpack to extract and process each part using a separate loader module, such as sass or SCSS loader. This setting allows us to write programs seamlessly using. Vue files.

    The Vue loader module also allows static resources to be treated as module dependencies and to be processed using the webpack loader. It also allows for hot reloading during development.    


    **[⬆ Back to Top](#table-of-contents)**

13. ### How will you render the original HTML in the template?

    A typical way to output content in a template is to use the mustache syntax tag to output data from a method, property, or data variable. But the mustache tag renders the text. If you try to render HTML using the mustache tag, it will render as a text string and will not be parsed. To render and parse content into HTML, we can use the v-html directive, as shown below.

    ```
      <p>Using mustaches: {{ rawHtml }}</p>
      <p>Using v-html directive: <span v-html="rawHtml"></span></p>
    ```

    ```
      Using mustaches: <span style="color:red">This should be red</span>
      Using v-html directive: This should be red
    ```
    The contents of the span will be replaced with the value of the rawHtml property, interpreted as plain HTML - data bindings are ignored. Note that you cannot use v-html to compose template partials, because Vue is not a string-based templating engine. Instead, components are preferred as the fundamental unit for UI reuse and composition.


    **[⬆ Back to Top](#table-of-contents)**

14. ### Explain lifecycle hooks in vue?

    Lifecycle hooks are an important part of any serious component. You often need to know when your component is created, added to the DOM, updated, or destroyed. Lifecycle hooks are a window into how the library you’re using works behind-the-scenes.

    1. **beforeCreate**  — This is the first hook that gets called after the Vue instance has been initialized. At this stage, data observation (reactivity), events, computed properties and watchers are yet to be set up. Therefore, we cannot interact with any parts of the component.

    2. **Created**  — This hook is called after the instance is created. At this stage, the instance has finished processing, data observation (reactivity), computed properties, methods, watchers and event callbacks have been set up. You can’t interact with the DOM at this stage because your component has not been mounted. The $el property is not also available yet.

    3. **beforeMount**  — At this stage, the template is compiled, either from the template or render options, or from the outerHTML of the element that Vue was initialized to. The template isn’t rendered yet and the $el method doesn’t exist either. Please note that this hook is not called during sever-side rendering.

    4. **Mounted**  — Called after the instance has been mounted, where el property is replaced by the newly created vm.$el. If the root instance is mounted to an in-document element, vm.$el will also be in-document when mounted is called. The component becomes fully functional after the mounted hook is called and we can fully interact with it.

    5. **beforeUpdate**  — It is called anytime changes are made to our data and the DOM needs to be updated, right before the DOM is patched. This is a good place to access the existing DOM before an update, e.g. to manually remove an added event listeners. This hook is not called during server-side rendering, because only the initial render is performed at server-side.

    6. **Updated**  — Hook is fired after a change has been made. The component’s DOM would have been updated when this hook is called, so you can perform DOM-dependent operations here. However, in most cases you should avoid changing state inside the hook

    7. **beforeDestroy**  — Called right before a Vue instance is destroyed. At this stage the instance is still fully functional. You can perform necessary cleanups here. Please note that this hook is not called during sever-side rendering.

    8. **Destroyed**  — Called after a Vue instance has been destroyed. When this hook is called, all directives of the Vue instance have been unbound, all event listeners have been removed, and all child Vue instances have also been destroyed. Please note that this hook is not called during sever-side rendering.


    **[⬆ Back to Top](#table-of-contents)**

15. ### How to listen to events?

    We can use the v-on directive to listen to DOM events and run some JavaScript when they’re triggered.

    ```
      <div id="example-1">
        <button v-on:click="counter += 1">Add 1</button>
        <p>The button above has been clicked {{ counter }} times.</p>
      </div>
    ```
    ```
      var example1 = new Vue({
        el: '#example-1',
        data: {
          counter: 0
        }
      })
    ```


    **[⬆ Back to Top](#table-of-contents)**

16. ### Which lifecycle hook is most suitable for getting data from API calls?

    Although this depends on the purpose and purpose of the component, the **created** life cycle hook is usually very suitable for placing API calls. You can use the data and responsiveness features of the component, but the component has not yet rendered.


    **[⬆ Back to Top](#table-of-contents)**

17. ### When is the updated lifecycle hook called?

    After the responsive data is updated and the virtual DOM is re rendered, the updated hook is called. It can be used to perform DOM related operations, but (by default) there is no guarantee that subcomponents will be rendered, although it can also be used in update functions **this.$nextTick** To ensure that.


    **[⬆ Back to Top](#table-of-contents)**

18. ### Why not use the arrow function when writing a lifecycle hook or other option or property in a Vue instance?

    Arrow function is not defined by itself **this** Context, but bound to the context of its parent function. When you use arrow function in Vue program（=> When **this** Keyword disease is not bound to a Vue instance, so an error is raised. Therefore, it is strongly recommended to use the standard function declaration instead.


    **[⬆ Back to Top](#table-of-contents)**

19. ### What is asynchronous component?

    When a large program uses a large number of components, it may not make sense to load all components from the server at the same time. In this case, Vue allows us to define components that are loaded asynchronously from the server when needed. When declaring or registering a component, Vue accepts the factory function that provides promise. You can then “parse” the component when it is called.

    By loading only the basic components and delaying the loading of asynchronous components to the future call time, the bandwidth and program loading time can be saved.

    This is a simple example of an asynchronous component.

    ```
      new Vue({
          components: {
              ‘tweet-box’: () => import(‘./components/async/TweetBox’)
          }
      });
    ```
    When used in this way, webpack’s code splitting will be used to provide this functionality.

    **[⬆ Back to Top](#table-of-contents)**

20. ### What are rendering functions? for instance.

    Vue allows us to build templates in a number of ways, the most common of which is to use only HTML with special instructions and mustache tags for response functions. But you can also use JavaScript to build templates using special function classes (called rendering functions). These functions are very close to the compiler, which means they are more efficient and faster than other template types. Because you use JavaScript to write rendering functions, you are free to use the language where you need to add custom functions directly.

    It is very useful for advanced solutions of standard HTML templates.

    **Here is the Vue program using HTML as a template** -

    ```
      new Vue({
        el: '#app',
        data: {
          fruits: ['Apples', 'Oranges', 'Kiwi']
        },
        template:
            `<div>
               <h1>Fruit Basket</h1>
               <ol>
                 <li v-for="fruit in fruits">{{ fruit }}</li>
               </ol>
            </div>`
      });
    ```
    **Here is the same program developed with rendering function** -

    ```
      new Vue({
        el: '#app',
        data: {
          fruits: ['Apples', 'Oranges', 'Kiwi']
        },
        render: function(createElement) {
          return createElement('div', [
            createElement('h1', 'Fruit Basket'),
            createElement('ol', this.fruits.map(function(fruit) {
              return createElement('li', fruit);
            }))
          ]);
        }
      });
    ```

    **Output** -
    ```
      Fruit Basket

      Apples
      Oranges
      Kiwi
    ```

    In the example above, we use a function that returns a series of createElement() Call, each of which is responsible for generating an element. Although the V-for instruction works in HTML based templates, when using rendering functions, you can simply use the standard.map() Function to traverse the fruits data array.


    **[⬆ Back to Top](#table-of-contents)**

21. ### What is mixin?

    Mixins enables us to write pluggable and reusable features for Vue components. If you want to reuse a set of component options between multiple components, such as lifecycle hooks, methods, etc., you can write it as mixins and simply reference it in the component. Then merge the contents of mixin into the component. If you want to define a lifecycle hook in mixin, it will take precedence over the component’s own hook when executed.


    **[⬆ Back to Top](#table-of-contents)**

22. ### How does prop specify its type requirements?

    By implementing the prop verification option, you can specify type requirements for a single prop. This has no impact on production, but warnings are issued during the development phase to help developers identify potential problems with specific types of requirements for incoming data and props.

    To configure three props -

    ```
    props: {
        accountNumber: {
            type: Number,
            required: true
        },
        name: {
            type: String,
            required: true
       },
       favoriteColors: Array
    }
    ```


    **[⬆ Back to Top](#table-of-contents)**

23. ### What is the difference between v-show and v-if directives?

    Below are some of the main differences between between **v-show** and **v-if** directives,

    1. v-if only renders the element to the DOM if the expression passes whereas v-show renders all elements to the DOM and then uses the CSS display property to show/hide elements based on expression.
    2. v-if supports v-else and v-else-if directives whereas v-show doesn't support else directives.
    3. v-if has higher toggle costs while v-show has higher initial render costs. i.e, v-show has a performance advantage if the elements are switched on and off frequently, while the v-if has the advantage when it comes to initial render time.
    4. v-if supports `<template>` tab but v-show doesn't support.


    **[⬆ Back to Top](#table-of-contents)**

24. ### What is Vue Router?

    Vue Router is the official router for Vue.js. It deeply integrates with Vue.js core to make building Single Page Applications with Vue.js easy to implement. Its features include -

    1. Nested route/view mapping
    2. Modular, component-based router configuration
    3. Route params, query, wildcards
    4. View transition effects powered by Vue.js’ transition system
    5. Fine-grained navigation control
    6. Links with automatic active CSS classes
    7. Customizable Scroll Behavior
    8. HTML5 history mode or hash mode, with auto-fallback in IE9


    **[⬆ Back to Top](#table-of-contents)**

25. ### What is parent in Vue?

    Similar to $root, the $parent property can be used to access the parent instance from a child.

    Although it provides direct access, it makes the application hard to test and debug. And we can not easily find out the where the mutation come from.

    Vue also provides $child just like $parent, but it can be used to access the child instance.


    **[⬆ Back to Top](#table-of-contents)**

26. ### What is key in Vue?

    In order to render DOM elements more efficiently, Vue.js reuses the elements instead of creating them from scratch every time. This default mode is efficient, but in some cases it may causes problems. For example, if you try to render the same input element in both v-if and v-else blocks then it holds the previous value as below:

    ```
    <templete v-if="loginType === 'ADMIN'">
      <label>ADMIN</label>
      <input v-for="Enter your ID" :key="admin-id" />
    </templete>
    <templete v-else>
      <label>GUEST</label>
      <input v-for="Enter your Name" :key="user-name" />
    </templete>
    ```


    **[⬆ Back to Top](#table-of-contents)**

27. ### What is the role of ref in Vue?

    Despite the existence of props and events, sometimes if we still need to directly access a child component, we can assign a reference ID to the child component using the ref attribute. For example -

    ```
    <child-component ref="componentId"></child-component>
    ```

    Now in the component where we have defined this ref, we can use -

    ```
    this.$refs.componentId
    ```

    $refs are only populated after the component has been rendered, and they are not reactive. Hence we should avoid accessing $refs from within templates or computed properties.


    **[⬆ Back to Top](#table-of-contents)**

28. ### What are Vue Props?

    Props (or Properties) are defined as the ways in which data is passed from parent component down to its child component.


    **[⬆ Back to Top](#table-of-contents)**

29. ### How do you set up a Webpack in Vue?

    Step#1: Set up Webpack:

    * Install Babel-loader and Webpack module:
    * npm install babel-loader webpack –save-dev
    * Open Webpack package.json and add a webpack script
    * In es6-tutorial, create a new file named webpack.config.js defined as follows -
    ```
    var path = require(‘path’);
    var webpack = require(‘webpack’);

    module.exports = {
      entry: ‘./js/main.js’,
      output: {
        path: path.resolve(__dirname, ‘build’),
        filename: ‘main.bundle.js’
      },
    module: {
      loaders: [{
        test: /\.js$/,
        loader: ‘babel-loader’,
        query: {
          presets: [‘es2015’]
        }
      }]
    },
    stats: {
      colors: true
    },

    devtool: ‘source-map’
    ```
    Step# 2: Building Webpack:

    Run following command: **npm run webpack**

    Open browser, access http://localhost:8080/, and click on the calculate button.


    **[⬆ Back to Top](#table-of-contents)**

30. ### What is slot and slot-scoped in vue?

    Slots are a mechanism for Vue components that allows you to compose your components in a way other than the strict parent-child relationship. Slots give you an outlet to place content in new places or make components more generic.

    **default slot** - when you have a single slot in a component. We create them by adding <slot> in the template where we want to be able to inject our content. This <slot> tag will be replaced with any content passed to the component’s template.

    ```
    <template>
      <div class="frame">
        <slot></slot>
      </div>
    </template>
    ```

    **named slot** - when you have multiple slots in a component and we want to inject different content in different places (slots). We create those by adding <slot> with a name attribute (e.g. <slot name="header"></slot>). Then when we render our component, we provide a slot content for each named slot by adding a slot attribute with the slot name.

    ```
      <base-layout>
        <template slot="header">
          <h1>My awsome header</h1>
        </template>
        <template slot="footer">
          <p>My awsome footer</p>
        </template>
      </base-layout>
    ```
    By doing that, the <slot> tags in the component will be replaced by content passed to the component.

    **scoped slot** - when you want a template inside a slot to access data from the child component that renders the slot content. This is particularly useful when you need freedom in creating custom templates that use the child component’s data properties.

    To create the scope we just need to add a prop in the slot tag with the data needed in the parent <slot :header="header" /> and then in the parent component receive it with slot-scope="{ header }" (see ES6 destructuring) or slot-scope="data" (without ES6).

    ```
      <th slot="header" slot-scope="{ header }">
        {{ header.label }}
      </th>

      or

      <th slot="header" slot-scope="data">
        {{ data.header.label }}
      </th>
    ```


    **[⬆ Back to Top](#table-of-contents)**

31. ### What are the conditional directives in vue?

    VueJS provides set of directives to show or hide elements based on conditions. The available directives are: ** v-if, v-else, v-else-if and v-show**

    1. v-if: The v-if directive adds or removes DOM elements based on the given expression. For example, the below button will not show if isLoggedIn is set to false.

    ```
      <button v-if="isLoggedIn">Logout</button>
    ```
    You can also control multiple elements with a single v-if statement by wrapping all the elements in a element with the condition. For example, you can have both label and button together conditionally applied,

    ```
      <template v-if="isLoggedIn">
        <label> Logout </button>
        <button> Logout </button>
      </template>
    ```
    2. v-else: This directive is used to display content only when the expression adjacent v-if resolves to false. This is similar to else block in any programming language to display alternative content and it is preceded by v-if or v-else-if block. You don't need to pass any value to this. For example, v-else is used to display LogIn button if isLoggedIn(not logged in) is set to false.

    ```
      <button v-if="isLoggedIn"> Logout </button>
      <button v-else> Log In </button>
    ```
    3. v-else-f: This directive is used when we need more than two options to be checked. For example, ifLoginDisabled property is disabled then we need to prevent user to login instead just display the label. This can be achieved through v-else statement.

    ```
      <button v-if="isLoggedIn"> Logout </button>
        <label v-else-if="isLoginDisabled"> User login disabled </label>
      <button v-else> Log In </button>
    ```  
    4. v-show: This directive is similar to v-if but it renders all elements to the DOM and then uses the CSS display property to show/hide elements. This directive is recommended if the elements are switched on and off frequently.

    ```
      <span if-show="user.name">Welcome user,{{user.name}}</span>
    ```


    **[⬆ Back to Top](#table-of-contents)**

32. ###  What is vue instance?

    Every Vue application works by creating a new Vue instance with the Vue function. Generally the variable vm (short for ViewModel) is used to refer Vue instance. You can create vue instance as below,

    ```
    var vm = new Vue({
      // options
    })
    ```


    **[⬆ Back to Top](#table-of-contents)**

33. ### What is Vue CLI tool?

    It is a npm pacakge npm package and allows using the vue command in terminal or command line. It allows to quickly create a Vue project using project scaffolding.

    To create a new project using the CLI use the following below command

    ```
    vue create projectName
    ```

    **[⬆ Back to Top](#table-of-contents)**

34. ### How we can bind HTML classes in Vue JS?

    We can pass an object to v-bind:class to dynamically toggle classes:

    ```
    <div v-bind:class="{ active: isActive }"></div>
    ```
    The above syntax means the presence of the active class will be determined by the truthiness of the data property isActive.


    **[⬆ Back to Top](#table-of-contents)**

35. ### How to create Two-way binding?

    You can use the v-model directive to create two-way data bindings on form input, textarea, and select elements. It automatically picks the correct way to update the element based on the input type

    ```
    <input v-model="message" placeholder="edit me">
    <p>Message is: {{ message }}</p>
    ```


    **[⬆ Back to Top](#table-of-contents)**

36. ### What are filters in Vue js?

    Vue.js allows us to create filters which can be used for applying text formatting.They are used to make the data presentable to the user.

    To use a filter we use the pipe character before the filter name.In the following example we are applying the filter filterName to the Expression expression.

    ```
    {{Expression | filterName}}
    ```
    We register a filter globally or locally.To create filter locally assign the filter method to filter property:

    ```
    filters: {
      boolean: booleanFilter
    },
    ```
    You can create a global filter as:

    ```
    Vue.filter('filterName', function(value) {
      return//data
    });
    ```


    **[⬆ Back to Top](#table-of-contents)**

37. ### When to use keep-alive component?

    To keep the switched-out components in memory, to make that happen, you should use <keep-alive> element:

    The only disadvantage is that these components are kept in memory and therefore their state is saved and not reset.

    ```
    <keep-alive>
          <component :is="currentPage"></component>
    </keep-alive>
    ```
    You also lose lifecycle hooks like created, mounted, etc. since the component is not being rebuilt from scratch anymore. You can replace those lifecycle hooks with hooks that are specific to keep-alive components.


    **[⬆ Back to Top](#table-of-contents)**

38. ### What are the properties of a Vue instance?

    Given an instance of Vue, stored into a variable const vm = new Vue(/*...*/) you can inspect and interact with it.

    * **vm.$data** the data object associated to the instance
    * **vm.$props** the props the instance has received
    * **vm.$el** the DOM element to which the instance is bound
    * **vm.$options** the object used to instantiate the Vue instance
    * **vm.$parent** the parent instance
    * **.$root** the root instance (if this is the root instance, this points to itself)
    * **vm.$children** an array of children instances
    * **vm.$slots** an array of the associated slots contained in the template
    * **vm.$scopedSlots** an array of the associated scoped slots
    * **vm.$refs** an object that contains a property for each element pointed by a ref attribute defined in the template
    * **vm.$isServer** true if the Vue instance is running on the server (useful in server-side rendering)
    * **vm.$attrs** an object of attributes that are provided to the component but not defined as props
    * **vm.$listeners** an object of v-on event listeners assigned to the component


    **[⬆ Back to Top](#table-of-contents)**

39. ### What are built-in components?

    Vue provides 5 built-in components:

    * **<component>**
    * **<transition>**
    * **transition-group>**
    * **<keep-alive>**
    * **<slot>**


    **[⬆ Back to Top](#table-of-contents)**

40. ### What is event key modifiers?

    key modifiers that allow us to listen to a particular key when handling key-related events such as keyup.

    ```
    <input v-on:keyup.13="addToCount" v-model="addValue">
    ```
    In the above example, when the keyup event is fired with the key code of 13 (the enter key), the addToCount method gets called.

    Since it’s difficult to remember all of the key codes, Vue provides a set of pre-defined keys. Some examples are enter, tab, delete, esc, space and left.

    Also, it’s possible to setup your own alias for key codes as follows:
    ```
    Vue.config.keyCodes.a = 65
    ```


    **[⬆ Back to Top](#table-of-contents)**

41. ### How to modify event?

    There are frequently used calls that are made when handling events. Vue has made it easier for us to implement these by using modifiers.
    The following modifiers are available in Vue.

    * **v-on:click.native** trigger a native DOM event instead of a Vue event
    * **v-on:click.stop** stop the click event propagation
    * **v-on:click.passive** makes use of the passive option of addEventListener
    * **v-on:click.capture** use event capturing instead of event bubbling
    * **v-on:click.self** make sure the click event was not bubbled from a child event, but directly happened on that element
    * **v-on:click.once** the event will only be triggered exactly onc
    * **v-on:submit.prevent** : call event.preventDefault() on the triggered submit event, used to avoid a form submit to reload the page

    Example -

    ```
    <a href="test" @click.prevent="addToCount">Add</a>
    ```
    The above code sample would remove the default behavior of the a tag and just call the addToCount  method. If we didn’t add the modifier, the page would try to re-direct to the path defined in the href attribute.


    **[⬆ Back to Top](#table-of-contents)**
