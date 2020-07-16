# Vue JS Interview Questions & Answers

> Click :star:if you like the project. Pull Request are highly appreciated.

---

<div align="center">
    <p>
        <b>Having Tech Interview?</b>
        <br> Tech Interview Questions. <b>Answered</b>.
        <sub><i>Proudly supporting Vue Interview Questions</i></sub>
    </p>
</div>

---

### Table of Contents

| No. | Questions |
| --- | --------- |
|   | **Core Vue JS** |
|1  | [What is Vue?](#what-is-Vue) |
|2  | [What is advantages of Vue?](#What-is-advantages-of-Vue) |
|3  | [Explain Vue.js reactivity and common issues when tracking changes?](#Explain-Vue.js-reactivity-and-common-issues-when-tracking-changes) |
|4  | [What is the virtual DOM and how is it beneficial?](#what-is-the-virtual-DOM-and-how-is-it-beneficial) |
|5  | [What are Components in Vue.js](#what-are-Components-in-Vue.js) |
|6  | [Why do we need local registration?](#Why-do-we-need-local-registration?) |
|7  | [What are list of features in Vue.js](#what-are-list-of-features-in-Vue.js) |



1. ### What is Vue?

    Vue is a **progressive framework** used to building user interfaces. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects.


   **[⬆ Back to Top](#table-of-contents)**

 2. ### What is advantages of Vue?

    **Small in size** — The size of Vue framework is 18 to 21KB and it takes no time for the user to download and use it.
    **Easy to Understand** — One of the reasons for the popularity of this framework is that it is quite easy to understand. The user can easily add Vue.js to his web project because of its simple structure.
    **Simple Integration** — Vue.js can be integrated with the existing applications easily.
    **Flexibility** — This flexibility also makes it easy to understand for the developers of React.js, Angular.js, and any other new JavaScript framework.
    **Virtual DOM** — It uses virtual DOM similar to other existing frameworks such as ReactJS, Ember etc. Virtual DOM is a light-weight in-memory tree representation of the original HTML DOM and updated without affecting the original DOM.
    **Components** — Used to create reusable custom elements in VueJS applications.
    **Two-Way Communication** — Vue.js also facilitates two way communications because of its MVVM architecture which makes it quite easy to handle HTML blocks.


    **[⬆ Back to Top](#table-of-contents)**

  3. ### Explain Vue.js reactivity and common issues when tracking changes?

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


  5. ### What are Components in Vue.js?

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


  7. ### What are list of features in Vue.js?
    Vue js comes with following features

    **Templates**
    **Reactivity**
    **Components**
    **Transitions**
    **Routing**


    **[⬆ Back to Top](#table-of-contents)**
