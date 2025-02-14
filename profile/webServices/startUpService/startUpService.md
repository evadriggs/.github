# Start up deliverable - Service

Now that you have learned how to use and create services, it is time to add significant functionality to your start up application. The main things you should focus on in this deliverable include calling third party services, providing your own service endpoints, persistently storing data using MongoDB as a data service, securely authenticating a user and storing their credentials, and enabling peer to peer communication using webSockets. This is a big upgrade to your previous deliverable and it will take a significant amount of time to provide all of this functionality.

You must use the same start up GitHub repository that you created in the earlier instruction. Update the README.md file with things that you learn as you work on your start up. As you make changes to your HTML, CSS, and JavaScript commit those changes and push them to GitHub. You will need at least four commits to get full credit, but in reality you should have many more than that. If you are using pair programming then your commit history should reflect contributions from all contributing peers.

Remember to use the `Live Server VS Code extension` to see what your code looks like in the browser. Also use the browser's debugger window to debug your CSS and JavaScript. You can also debug your service JavaScript running on Node.js using the built in VS Code debugger.

Once you have developed your application to where you want it, you need to release it to your production environment. **Replace** your previous start up deployment script with a copy of the `deployService.sh` script from the [Simon Service repository](https://github.com/webprogramming260/simon-service/blob/main/deployService.sh) and use `startup` for the service parameter (`-s`).

```sh
./deployService.sh -k <yourpemkey> -h <yourdomain> -s startup
```

For example,

```sh
./deployService.sh -k ~/keys/production.pem -h yourdomain.click -s startup
```

Doing this will make this deliverable of your start up available from `https://startup.yourdomainname`.

### Update your website's home page

You should also update your website's home page with a link to your project so that you can access everything you have done for this class from the home page. This will make a great portfolio of all your work in this class. You can easily do this by modifying the index.html file that is part of the website-html repository, that you created in the earlier instruction, and deploying it using the script found in that repository. Make sure you run this script from a console in the website-html repository and not your start up repository.

```sh
./deployWebsite.sh  -k <yourpemkey> -h <yourdomain>
```

## ☑ Assignment

1. Convert your start up application into a web service.
1. Provide endpoints for your service.
1. Call third party endpoints from your service.
1. Persist data in MongoDB.
1. Authenticate users.
1. Use WebSockets.
1. Make sure all authors of the code are attributed in the application and that there is a link to your GitHub repository.
1. Periodically commit and push your code to GitHub.
1. Periodically update your start up repository's README.md file to reflect what you have learned and want to remember.
1. Push your final version of your project to GitHub.
1. Deploy your start up application to your production environment (your server).
1. Make sure your application is available from your production environment.
1. Upload the URL to your start up application to the Canvas assignment.

## Grading Rubric

- 10% - Calls third party service endpoints
- 20% - Provides service endpoints running under Node.js
- 10% - Stores data in MongoDB
- 10% - Provides authenticated login with securely stored credentials in MongoDB
- 10% - Peer communication using webSockets
- 20% - Your start up application is hosted on your web server and is accessible using a subdomain of your domain name using HTTPS.
- 10% - Multiple Git commits with meaningful comments.
- 10% - Notes in your start up Git repository README.md file documenting what you have learned using services, node.js, mongodb, authentication, and webSockets.

## Go celebrate

You did it! This is a significant milestone. Time to grab some friends, show them what you did, and celebrate by watching a movie with popcorn.
