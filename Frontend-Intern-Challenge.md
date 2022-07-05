## Frontend Developer Intern Challenge

### Spacegram: Image-sharing from the final frontier.

For the purposes of this project, Outpost is building a serverless cloud platform. Please build us an app to help share photos from one of NASA’s image APIs.

### The Challenge

We need a webpage that can pull images, and allow the user to “like” and “unlike” their favourite images.

We'd like a simple to use interface that makes it easy to:
- Fetch data from one of NASA’s APIs and display the resulting images (more details under Technical Requirements)
- Display descriptive data for each image (for example: title, date, description, etc.)
- Like an image
- Unlike an image

### Technical requirements

1. Search results should come from NASA’s free APIs, for which you’ll need a free API key from https://api.nasa.gov - 
- you do not need to enter anything more than your first name, last name, and email address (i.e. application url is not required)
- We’ve provided screenshots below of demo apps we built using the Astronomy Picture of the Day or Mars Rover Photos APIs (along with Outpost’s open source React component library: Jenga-UI). 
- You are free to use any NASA API you like
- You are free to use any front end framework/component library you like (or none at all!)
2. Each image result should list at least a title, date of capture (ideally in earth_date) and a button to “like” that image.
3. Each image can be “liked”, and a user should be able to undo their “like”
4. The HTML that ends up being served client-side should be accessible and semantic (MDN reference)

### Example screenshots

### Extras

There is a lot to be improved on here, you can polish the required features by crafting a nicer design, or improve the app by adding new features! Choose something that you feel best showcases your passion and skills.

If you need inspiration, here are examples of what you can work on. If you work on these ideas, we recommend choosing only one or two.


- Save likes if the user leaves or reloads the page
- Animate the “like” action (might we suggest a heart?)
- Add a loading state while we wait for NASA’s API to return data
- Create shareable links for each image
- Add a date-picker to be able to browse photos starting from a specific date

### Submission

Please submit your application via “Apply Now” and make sure you include:
- A link to your hosted code so we can test it (Free hosting available via: CodeSandbox, Github pages, Netlify and Heroku)
- A link to your Github repository containing the code
- Any other notes you'd like us to consider alongside the page
