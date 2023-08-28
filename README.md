# Sample app for deployment to AKS cluster

To use this sample app for deployment:

1. Ensure Git is installed in your machine.
2. Clone this repository to your local machine.
3. (OPTIONAL) If you want to run this code locally, ensure you have Node and NPM installed. Once you have done so, you can run npm install and npm start. Visit localhost:3000 on your browser and verify that you can see the message "Hello world".

To make changes and commit this app to be built and deployed:
1. Checkout a new branch to your local machine (sample branch name "welcome-message-feature")
2. Open app.js in a text editor.
3. Change the message on line 5 from "Hello world" to "Hello Collectius!".
4. Commit changes and push to the upstream branch.
5. Visit https://github.com/rvind92/express-app/pulls and approve the PR to kick the build and push process. You can view the workflox execution at https://github.com/rvind92/express-app/actions.
6. Once completed, visit https://github.com/rvind92/express-app/pulls again and approve for merging the code.
7. Visit the ArgoCD UI at localhost:80 or https://20.14.29.149 and click on express-app application in the application list.
8. Observe the ArgoCD agent in updating the state of the application. If it is not updating, then manually sync the application by click on the Sync Apps button.
9. Once the state is healthy, open your browser and visit localhost:3000 or https://20.14.29.149:3000.
