# State and Props

## React lifecycle
**- What is React lifecycle ?**  
Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence.

**React lifecycle:**  
Mounting, Updating, and Unmounting are the three phases of the component lifecycle. 
![](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

**- What happens first:**   
Mounting --> Updateing --> unmounting  
constructor --> render --> React Updates --> componentDidMount --> componentWillUnmount

- componentDidMount: This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

## React State Vs Props

**What is the different between state and props?**
![](https://i.stack.imgur.com/wqvF2.png)


**- What the use of props and state?** 
- Use state to store the data your current page needs in your controller-view.
- Use props to pass data & event handlers down to your child components.



**- When do we re-render our application?**  
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
