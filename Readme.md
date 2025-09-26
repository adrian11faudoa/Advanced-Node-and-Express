Subject:

# Advanced Node and Express

This is the boilerplate for the Advanced Node and Express lessons. Instructions for the lessons start at https://www.freecodecamp.org/learn/quality-assurance/advanced-node-and-express/


A template engine enables you to use static template files (such as those written in Pug) in your app. 

At runtime, the template engine replaces variables in a template file with actual values which can be supplied by your server. 

Then it transforms the template into a static HTML file that is sent to the client. 

This approach makes it easier to design an HTML page and allows for displaying variables on the page without needing to make an API call from the client.

pug@~3.0.0 has already been installed, and is listed as a dependency in your package.json file.

Express needs to know which template engine you are using. Use the set method to assign pug as the view engine property's value:

app.set('view engine', 'pug');
After that, add another set method that sets the views property of your app to point to the ./views/pug directory. This tells Express to render all views relative to that directory.

Finally, use res.render() in the route for your home page, passing index as the first argument. This will render the pug template.

If all went as planned, your app home page will no longer be blank. Instead, it will display a message indicating you've successfully rendered the Pug template!


1. Pug should be a dependency.

2. View engine should be Pug.

3. You should set the views property of the application to ./views/pug.

4. Use the correct ExpressJS method to render the index page from the response.

5. Pug should be working.
















