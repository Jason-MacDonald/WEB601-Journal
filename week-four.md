# WEB601 Journal: Week Four

### Technical Jargon
Our first discussion for week four focused on a high level view of the communications between front end and backend. The topic was covered in simplistic terms removing the technical jargon 'We request something from the sever, the server evaluates and returns the requested data etc". We also discussed the importance of being able to communicate technical details in a simplistic way as jargon can be a major barrier to effective communication. I find on occassion that someone will use an acronym or call something by a name I can't remember or haven't heard before and become immediately lost. It really comes to evaluating who you're talking to and adjusting the explaination to an appropriate level of detail. 

### Evaluating Node Packages
When deciding on Node packages to use in our projects, there are a range of things we should do to ensure it is appropriate on has a reasonable longevity. Simply by going to it's git repo can reveal alot of information like; 
* is the package being updated regularly,
* are package issues being resolved,
* is the package well documented etc.
I have a general understanding of what node is although I definately need some practice in implimenting packages in a few projects, and codecademy is coming the the rescue with a couple of node courses. 

### express.js
From my current understanding, express is built upon the node.js framework with a heavy focus on web applications. I remember taking a few php tutorials a quite a few years back so I am quite interested in how express will allow us to communicate between the network and its clients. Routing is another aspect of Express we discussed, specifically the routing for a member site where a user needs to be logged on and be able to provide credentials before they can access certain information. This is one aspect I am interested in seeing how it is handled.

### Require Statements
Express is downloaded using NPM. We can use Nodes Require() function to add the express package to our project. We then assign express to an alternate variable.

<pre>const express = Require('express');</pre> 
<pre>const app = express;</pre>

### Middleware
Middleware is our interaction with express. This process will call actions which will be run within express and return results. The following is a general example of expresses 'use' function (without route);

<pre>
 app.use(function(request, result, next)){
   let booking = request.booking;
   let age = request.age;
   if(booking && age >= 18){
       next();
   }
 }</pre>

 ['request' is an http request]

 Flow: request > use > get > send

### Routes
Below is an example of the use function including a route using the class example.

<pre>
 app.use('/route', (request, result, next)) => {
   let booking = request.booking;
   let age = request.age;
   if(booking && age >= 18){
       next();
   }
 }</pre>

 <pre>
 app.get('/route':amount, (request, result, next)) => {
     let dinner = request.params.amount;
     result.send('Looking for table for ' + dinner);
   }
 }</pre>

<pre>
request = {
    p:{
         amount : 4
    }
}
</pre>

Class example of Bar:
<pre>
const express = Require('express');

const tableRoute = express.Router();

tableRoute.use(function (req, res, next)){
    let booking = req.booking; 
    let age = req.age;
    if(booking && age){
        next();
    }
}

tableRoute.use(/bar, function (req, res, next)){
    let age = req.age;
    if(age >= 18){
        next();
    }
}

tableRoute.use(/kids, function (req, res, next)){
    let age = req.age;
    if(age <= 10){
        next();
    }
}</pre>

<pre>
app.listen(3000){
    console.log('Running on :3000');
}</pre>

### Application

### Codecademy
Unfortunately I've been a lttle slack on the codecademy front as of late. It's not that I don't enjoy it, it's actually the opposite, where I spend far more time in it then I probably should be at the moment. Now that the PRO account has been downgraded there are significantly less sections to cover, but I am continuously finding new courses that I want to take. If only I could get a job as a codecademy learner... I'm currently working through the javascript course and I'm hoping to start working on the node and express courses soon.

### Homework
Nothing to difficult in the homework we had set for the week. What I found really interesting was turning the code into arrow functions. This was the first time I have really seen alot of the ES6 shorthands like string literals ${'foo'}, ternary statements foo ? true : false, and arrow functions => and I'm always looking for ways to shorten the code. At first I found it a little difficult to read but after a while it becomes second nature.

### Next Steps
There is quite a bit to be done at the moment but my main focuses will be:
* Finish wireframes and storyboards,
* Draft report documentation,
* Create project repository,
* Create GitHub project.
