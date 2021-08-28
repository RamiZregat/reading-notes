# Introduction to React and Components

## Component
**- What is a component ?**  
A component architecture is a type of application architecture composed of independent, modular, and reusable building blocks called components.


The value proposition of a component-based architecture is that it boosts application development time and reduces.

**- What are the charactistics of a component ?**  
- **Reusability:** Components are usually designed to be reused in different situations in different applications. However, some *components* may be designed for a specific task.
- **Replaceable:** Components may be freely substituted with other similar *components*.
- **Not context specific:** Components are designed to operate in different environments and contexts.
- **Extensible:** A component can be extended from existing *components* to provide new behavior.
- **Encapsulated:** A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
- **Independent:** Components are designed to have minimal dependencies on other *components*.

**- What are the advantages of using component based architecture ?**  
- **Ease of deployment:** As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

- **Reduced cost:** The use of third-party components allows you to spread the cost of development and maintenance.

- **Ease of development:** Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

- **Reusable :** The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

- **Modification of technical complexity:** A component modifies the complexity through the use of a component container and its services.

- **Reliability :** The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

- **System maintenance and evolution:** Easy to change and update the implementation without affecting the rest of the system.

- **Independent :** Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.


## Props

**- What is props short for ?**  
React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.

**- How are props used in React ?**  
1. Firstly, define an attribute and its value(data).
2. Then pass it to child component(s) by using Props.
3. Finally, render the Props Data.

**- What is the flow of props?**  
There are basically two ways that data gets handled in React: props and state (available through `this.state` ). A third is context, not discussed here, which is more advanced and not currently guaranteed stable.

While a component can’t change its own props, it can change its state…Props and state are used as input for the `render()` method to determine its output. The `render()` method also calls the diff algorithm which recognizes any changes in the component and logs them for batching to the “real” DOM.