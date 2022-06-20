Deployed on Netlify: https://doctor-booking-assignment.netlify.app
1. Choice of Package: Please specify the key packages you use (except for React) and explain why you choose the particular package.

a. What's the purpose/importance of the package?

I used Next.js framework for the whole project.
Generally such booking platforms require high Google SEO for user attractive and Next.js provides good effects regarding google SEO.
That's the most important point that I selected this Next.js


b. What are the benefits & drawbacks associated with that choice?

Next.js provides server side rendering and it improves the application performance as well as SEO.
It also makes developer easier to construct application full-fledged.
There are also more benefits using Next.js such as fast refresh, TypeScript support and so on.
By the way, it doesn't provide many built-in front pages, so you have to create the whole front-end layer from the ground up.
And it doesn't support many plugins


c. What are the assumptions underlying that choice?

I've worked on React.js and Next.js projects for several years and have deep understanding about it's features and much experienced to use it.


2. Potential Improvement: Please elaborate on what kind of improvements you would like to implement if you have given more time.

- cancel schedule
Now, there are no account info so we can't match the user and his/her scheduled data.
So I wanan implement auth feature to register user info in backend so they can see their scheduled info as well as cancel function

- booking database restructure
For now, the datastructure of booking is not so clear and perfect so I wanna change it on my mind.

- detailed schedule option
According to less time, I couldn't implement the details about schedule options.
For example, users should choose time range (15min, 30min, 1hr, etc) for scheduling the booking and each time range will change the available time slot on the calendar or table.
So we can add option for time range on scheduling page.

- get nearby doctors from my side.
The doctors have their info which is also containing their addresses.
We can get the users' location using api once they come to our platform.
With comparing two loactions, we can get the nearest doctors that users can prefer.

- view doctors shedule and my booking lists weekly, monthly and daily.

3. Production consideration: Any extra steps should be taken with caution when deploying your app to a production environment?
- Use caching wherever possible.
- Ensure the database and backend are deployed in the same region.
- Aim to ship the least amount of JavaScript possible.
- Ensure logging is set up.
- Ensure error handling is set up.
- Configure the 404 (Not Found) and 500 (Error) pages.

4. Assumptions

a. Any assumptions you have made when you designed the data model and API schema?

Regarding the data model, I will create a user table and save the booking table with userid instead of name and doctorid.
In terms of API schema, I will update the get booking api with params.
We only have api that gets all booking lists at the moment, but it's not convenient because all data has to be retrieved whenever a user wants to book. We can include doctorId, date, and userId in the params, so that backend filters the data and retrieve the matching data.
It will reduce the time.

b. Any other assumptions and opinions you have taken throughout the assessments?

I think almost of my opinions regarding the assesments are mentioned on the above questions.
Thanks
