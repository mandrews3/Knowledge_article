# Knowledge_article                          # Written By: Matthew Landon Andrews

#Personal Experience

  Throughout setting up my node.js app, I realized there are muiltiple different parts that make the app itself work, as you build the app you have to commute back and forth to seperate folders and files to ensure that the system is working properly. Node.js is a type of open source and cross-platform Javascript runtime enviorment that is used for a muiltiude of project. It works by creating a single process without creating a new thread for each and every request, making it simple to travel back and forth to make updates to your code. My personal experince when setting up my first node.js app, I found that starting small and building to get to a bigger picture works best. Throughout writting your code, I found that testing certain ideas before moving on to a different task allows you to ensure that the system is running smoothly, this ensures that you don't move on to a new step if the system isn't working properly. Node.js is a test driven development, which means that you must test the system as you creating it to ensure that it runs properly without any error. You are able to code both the front in and back in of the programming language in a single languge rather than being like a web browser, were you are not able to choose what browsers your visitors will use, when you can with node.js. The Node.js performs using a I/O operation that reads from a network and accesses its database or filesystem, instead of having to block the thread and wasting many CPU cycles, keeping them waiting. With node.js you are able to resume your normal operations as soon as you pull the app back up. Theres less bugs and errors when creating a node.js app because its all located within a single server. The Node.js allows you to commit changes and then save your document and return the next day to complete more changes without keeping the server waiting. You are able to make notes and add information to your readme file you can come back and pick up where you left off in the code.

# Benefits of Using Node.js

-It gives you a production boost.

-Ensures you code works properly.

-It is easy to maintain your code, while allowing you to provide correct maintance.

-Improves development of your code.

-Less room for debugging your code (reducing errors).

#Different API functions that were used in my Node.js app

-app.use(express.json())

This simple function is considered middleware that parses JSON request bodies, so when someone sends JSON data such as a name ({"name": "Landon"}) in a POST request, it makes it available in the 'req.body'.

-app.get('/api/barry', (req, res) => { ... })

This function handles the GET request that is pulled from /api/barry, and it returns a JSON object, or in simple text its a smaller API that says hello in the JSON format.

-app.listen(PORT, () => { ... })

This simple function is what starts the server on whatever given port is enter into it, with the default being port '3000', which is what makes your app listen for incoming request at http://localhost:3000, if we were using the default port. 

-There are many different functions that you are able to use for a Node.js app and many can be found through this links. There are many different soruces out there to find different API but to share a few here are two links to descirbe some APIs for a Node.js.

Link: https://jsschools.com/javascript/essential-nodejs-apis-a-complete-backend-develop/

Link: https://www.sitepoint.com/useful-built-in-node-js-apis/

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Handoffs

Handsoffs are used whe writting a node.js app because it allows you transfer tasks or responsibilities to ether someone else in group or to yourself for a furture date. It allows you to write a snipit of text that explains where you left off in the code, or write a simple message to someone else to complete the next part of the code to ensure you are directly where you left off in the code. This allows the creation of the node.js app to have continuity and efficiency in many different settings. In simple terms, handoffs are where you can write a note for yourself, then leave the coding platform, and return on a later date and see the note you left yourself and start right back where you ended off. 

#Example of a Handoff

In my node.js app I have written staright in the code, in this case the App.mjs file, comments that tell me what task I need to complete next. 

-app.get('/api/url/:iaddasfsd', (req, res) => {
  console.log("client request with URL param:", req.params.iaddasfsd); 
  // const name = req.query.name; 
  // res.json({"message": `Hi, ${name}. How are you?`});
});

Note that the items I commented-out told my future self that I shouldn't forget that this route should eventually send JSON back to the client. That way when I came back to the code I wouldn't be puzzled or confused on what the /api/url/:id was supposed to be doing, instad I left a commit to ensure I knew what it was supposed to do.


-app.get('/', (req, res) => {
  res.send('Hello Express from Render 😍😍😍. <a href="barry">barry</a>')
})

// endpoints...middlewares...apis? 

// send an html file
app.get('/barry', (req, res) => {
 
  res.sendFile(join(__dirname, 'public', 'barry.html')) 

})

#Git Commands

-"git commit -m "message"

This git command commits staged changes with a message. 

-git clone

This clones a remote repository to your local machine.

-git add

This stages all changes in the working directory.

-git status

This displays the current state of the repository.

-git pull

Fetches and merges changes from a remote repository.

-git push

Pushes local commits to a remote repository.

There are a muiltitude of git commands you can uses, heres a link to show you a large portion of them: https://www.geeksforgeeks.org/git/git-cheat-sheet/



Another example of me using a "handoff" in mode code so that I wasn't confused when returning to the code or forgetting what to add is above. The comments "//endpoints...middlewares...apis?" told me when returning to the codes that I needed to add enpoints such as /api/query. The middlewares section explained that I need to add a "express.json()", so I needed to define my API endpoints first then add the middleware section later.

#Simple Idea of a Handoff

 -Example:
  // TODO: connect this route to the database later
app.get('/users', (req, res) => {
  res.json({ message: "Users route not finished yet" });
});

-To simplify it in the eyes of someone who is unable to process the tech language this is a simple snipit of code that I created to show how these comments can help. By adding the "//TODO:...." you simple adding a sticky note to be specific to your code so that you are able to come back on a later date to complete it. So, in this case you can see that where the TODO comment is, that you need to connect the database to this system so it can run properly. This way you are able to pickup where you left off, or if you were to be handing this code to another individual, they can read this stick note and understand what to add to the code to make to run properly. 

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#Agile Handoff

Definition: In Agile methodology, handoff refers to the process of transfering work, information, or responsibilities between team memebers or individuals during different phases of works. It gives guidlines to ensure smooth transitions while mainting the quality of the app and communicaiton if you were working with multiple people. These handoffs allow you to communicate smoothly throughout the development process. Adding this simple notes throughout my code helped me stay on track with what I was trying to complete whenever I would stop working on the app. I found that the more handoffs you add to your code, even if you had already completed what you need, it explains exactly what the code is doing or needs to be doing. This ensure that each and ever process of your code is working properly. As I was working on my Node.js, the handoffs gave me clarity while maintaining momentum, to help prevent me from having any delays with my code. Everytime you I stopped coding in my Node.js app and returned later, I realized that you are just handing off your work to your future self, and if I didn't leave myself any notes/context then I just confused myself.

#Resources

1: https://www.w3schools.com/nodejs/

2: https://nodejs.org/en/learn/getting-started/fetch

3: https://thisvsthat.io/handoff-vs-handover

4: https://www.geeksforgeeks.org/git/git-cheat-sheet/

5: https://code.visualstudio.com/docs/nodejs/nodejs-tutorial


#Video Links

1: https://www.youtube.com/watch?v=gyQyk80_upM

2: https://www.youtube.com/watch?v=32M1al-Y6Ag

