# Login & Auth

## Questions
1. Why is the Context API useful?
    Because it allows you to share data with other components.
1. Can a component outside of a provider get its context?
   No it can't.
1. What are some common use cases for using the Context API?
    Theming — Pass down app theme. Authentication — Pass down current authenticated user.
1. Describe “Context Hell”
    Context hell is the nasty code you get taking advantage of the React Context API.To clean up the nasty code you get from taking advantage of React Context API we need a way to nest multiple Context.Provider without passing them as children of each other. To achieve that we can use the React.cloneElement API.


## Vocabulary Terms

* global state: State that all component can use it.
* global context: context at the top level of your app.
* provider: allows consuming components to subscribe to context changes.
* consumer: A React component that subscribes to context changes.
 


## Notes
* Which 3 things had you heard about previously and now have better clarity on?
    1. react
    1. context
    1. auth
* Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. react
    1. context
    1. auth
* What are you most excited about trying to implement or see how it works?
To make a perfect website