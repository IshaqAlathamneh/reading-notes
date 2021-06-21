# Custom Hooks

## Questions
1. What does a component’s lifecycle refer to?
    It's refer to the component's rendering and updating or deleting.

1. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
   useCallback will help in avoiding regeneration of functions when the functional component re-renders. However there isn't much of a performance difference caused by recreation of functions. You are specifying a function as a dependency to useEffect .
1. Why are functional components preferred over class components?
    Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices.
1. What is wrong with the following code?
    The render items array should be spreaded.


## Vocabulary Terms
* state hook: It's a hook allow you to change the state of anything rathar than the this.state object from class.
* effect hook: Hook to follow what's happen for specific component or the whole page.
* reducer hook: useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke.
 


## Notes
* Which 3 things had you heard about previously and now have better clarity on?
    1. react
    1. hooks
    1. bootstrap
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. react
    1. hooks
    1. bootstrap
* What are you most excited about trying to implement or see how it works?
To make a perfect website