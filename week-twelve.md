# Week Twelve

### Redux and Other Dirty Words
In today's session we worked on a Redux tutorial over on freecodecamp. It started of relatively simple with a few basic concepts but had a few difficult ones near the end which required a few hints to get the syntax. Redux is all about managing the state of an application. There are several places in my project where things get really messy passing around data between components so Redux is hopefully how I'm going to solve that issue.

There are several main elements involved in Redux:
* Store: This almost seems a bit magical. It is simply an object with a few methods but is used as a container for the applications state data.
* Reducer: A reducer is a javascript function that takes two parameters, the current state and an action. They then return the appropriate state.
* Actions: Basically a javascript object with two properties, a type and a payload. 

We then have the subscribe and dispatch functions. these are store methods although I need to gain a little more understanding as to how these work.

The trick part for now is probably going to be working out who is meant to do what and how to connect it with react. This will likely be determined by some of the redux rules such as abstracting control away from components and ensuring the we change copies of the state rather than the state itself. react-redux appears to have a 'connect' method which seems to allow us to connect react components with the store. 

... And then theres async actions on the horizon. 

### Project
Even though we've only been introduced to redux at this stage I can see a couple of places where this is going to be handy in the project. I feel like my project is all over the place at the moment. There's components passing data around and it can be difficult to follow what's going where and sometimes even harder just to find what I'm looking for! Although redux is adding another level of abstraction, I'm envisioning an easier structure to follow and I can possibly remove some of the nested component complexity, especially where I am retrieving a list of vehicles from the database and then trying to display them on a dynamic number of cards. Will be interesting to see how the project develops from here. I did agree to get some additional functionality in my project within the next four weeks but I'm not really sure how long this redux is going to take to pick up and that is going to be my goal for now, because if I manage to comprehend it, then the additional functionality should be easier to implement.