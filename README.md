# illaCloud with AppWrite

In this tutorial, you'll learn how to connect illaCloud with the AppWrite database and use the powerful features of the AppWrite database within the illaCloud Builder.

## illaCloud - [link](https://cloud.illacloud.com)

#### What is illaCloud Builder and why do we need it?

illaCloud Builder is a product of illaCloud which is a robust open source low-code platform for developers to build internal tools. By using ILLA's library of Components and Actions, developers can save massive amounts of time on building tools.

## Features

1. **Real-time Collaboration:** We can create everything in real-time together.
2. **Custom Plugin:** Build any custom plugin to do what you want.
3. **Automate Support:** Connect everything and automate them in 5 seconds.
4. **Self-hosted:** supports Docker & k8s
5. **Page Support:** The base of creating a content-rich and UI-friendly tool.
6. **Powered by [ILLA Design](https://github.com/illacloud/illa-design):** Components should not constrain your imagination.

## Appwrite

#### What is Appwrite and why do we need it?

Appwrite is an open-source backend server infrastructure that simplifies the development of web applications by providing a wide range of pre-built APIs. We need Appwrite because it provides a NoSQL database and API endpoints, allowing developers to easily store and retrieve data.

#### How to configure Appwrite with illaCloud?

To configure Appwrite, follow these steps:

1. Open [Appwrite Cloud](https://cloud.appwrite.io/) and create a new project.
2. Choose the "Web App" platform and provide a name for your app.
3. In the hostname field, enter your domain name without any protocol or port (e.g., "\*"). Be cautious as incorrect configuration can lead to CORS errors.
4. Proceed with the next steps and save the connection URL (End Point) and then navigate to the dashboard.
5. Create a new database and within the database, create a new collection.
6. Define the necessary attributes for the collection. In our case, we will create four attributes:
    - `name`: A string type attribute to store the name of the student.
    - `email`: A email type attribute to store the email id of the student.
    - `phone`: A number type attribute to store phone number of the student.
    - `state`: A string type attribute to store state of the student.
    - `team_name`: A string type attribute to store team name of the student.
    - `github`: A URL type attribute to store github link of the student.
7. Navigate to the "Overview" tab. Look for the "API KEY" options and create a new API key. This key will be necessary for connecting with illaCloud.

## Getting Started With illaCloud

To try ILLA, the most convenient way is to sign up and log in to [ILLA Cloud](https://cloud.illacloud.com/).

1. Begin by setting up your workspace and choosing "ILLA Builder".
2. Within the ILLA Builder interface, you'll find two tabs: "App" and "Resources." Go to the "Resources" tab, create a new resource, and select "appwrite." Fill out the form with the necessary appwrite configuration details.
3. Once you've completed the resource setup, proceed to create a new app. Upon doing so, you will be directed to the editor page where you can begin working on your app.
4. At the bottom of the page, you'll find an action list. From there, you can create a new action. Choose "appwrite" as the action type, and select the appwrite resource that was previously created.
5. Within the method, you will find a list of available methods provided by appwrite. These methods include options such as retrieving documents, creating new documents, and more.
6. Choose a specific method from the list that best describes the functionality of your action and save that action.
7. On the right side of the page, you'll notice a variety of components offered by illa Builder. Simply click and drag the desired components from the sidebar and drop them onto the workspace to utilize them in your app.
8. To modify the configuration of a component, simply click on that component, and you will be able to access and make changes to its configuration settings.
9. By binding events with the actions you've created, you can enable specific actions to be triggered in response to certain events. For example, you can set up an action to be performed when a form is submitted or when a button is clicked to fetch data and display it in a table.
10. To deploy your app, locate the deploy button located at the top right corner of the page and simply click on it. This will initiate the deployment process for your app.

---

\
Congratulations! You have successfully created your first web app using illaCloud, leveraging appwrite as a backend-as-a-service (BaaS) solution.
