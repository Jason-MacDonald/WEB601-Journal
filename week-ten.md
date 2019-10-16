# WEB601 Journal: Week Ten

### MySQL
For the first session this week we started working with a test database which included tables for Employees and Departments. After looking at MySQL briefly last week, all that DAT602 knowledge came flooding back and this was a pretty simple task, although it can be one of those simple but time consuming tasks trying to put together enough records for testing.

After getting the bare minimum done :D I was able to start generating the Data Definition Language required for the simple database I had planned for Milestone Two of the project. I didn't quite get to adding the test data during class as we moved on with the next adventure but should have it up and running soon.

### Knex <-> MySQL
We also had a look at Knex and MySQL, and more specifically how to communicate between them. We were given an example which allowed us to perform calls such as GET, POST, UPDATE, and DELETE from the Employee table and then created similar calls for the departments table. It was a little confusing at first but after getting one or two done it became a bit easier.
I had a little time left after the exercise so I even managed to create a GET request in my own project before leaving class.

### Class Project Work
I managed to get the a variety of calls completed between the first and second class of the week. These were able to function using Insomnia as I was having a few issues with the original Postman app we were using for testing our requests. I'm a little confused about how a search request would work but will look into achieving this over the holidays.

### Project
This is just a little update on some of the things I achieved over the holidays:
* GET (single), GET (all), POST, PATCH, and DELETE requests created and working for Accounts table.
* GET (single), GET (all), POST, PATCH, and DELETE requests created and working for Vehicles table.
* GET request which returns a filtered list of vehicles based on form inputs.
* Added administration page for login, adding vehicles, updating vehicles and deleting vehicles from the database.
* Added some code which allowed requests to be performed on the database. Another option would have been to install Cors but the first way worked so...
* GET request which returns list of vehicles that are tagged as 'featured' vehicles.
* Displays featured vehicles on the front page.
* Displays unfiltered vehicles on vehicle page if no parameters provided.
* Created data sources for search form drop down boxes.
* Displays filtered vehicles on vehicle page when parameters are provided.
* Tidied up an issue with the reset css which was breaking on occasion. This required an additional forward slash and only took about three hours to solve............
* Several study session with a classmate. This was helpful to me as I had to try an explain what I had done and I feel it has given me a better understanding of the code.

I was having a little difficulty working out how to get data returned from the database to be displayed on screen when the request needed to be provided information from a form. I've used to different ways to accomplish this, one is  in the components componentDidMount life cycle method which required passing variables from here to there to over there and took a while to get working. The other way was to call it directly from the search from component, which I found in a fellow classmates project. This was far simpler but I'm not sure I fully understand how it works yet.

### Kill Me Now
So there are many things in my project which I feel I could improve upon but the ever closing in deadlines mean I am having to choose which things I need to accomplish and which things I'm just not going to get to in time. Some of these include:
*
Hopefully some of these thing will get done, but I'm also finding that every step I make forward reveals 10 other issues that I need to deal with. Happy Times.
