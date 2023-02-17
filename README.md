![Module Federation](./docs/module_federation_banner.jpg)

# Workshop: Basic Microfrontends in React
A workshop geared to help you create your first microfrontend using react and module federation. This course will give you the basics of the technology that makes it possible and how it all works together. All of the code will be operating in a monorepo for convenience and ease of adoption. 

### Time frame
This course should take 1-3 hours depending on your proficiency.

### Prerequisites 
- Intermediate hands on experience in React.
- Basic knowledge of Http Methods and javascript loading.

## ▪️ What is a Microfrontend Architecture?

Microfrontend architecture is an approach to breaking up your front-end into a set of independently deployable, loosely coupled applications and/or components. These applications are then assembled together to act as a single user experience, once deployed. We do this using a new technology called Module Federation. We have a single Host application which wraps up our single page applications represented as remotes.

### What are hosts and remotes?

When we talk about micro-frontends, we often use words like `HOST` and `REMOTE`. A host is a parent application that ties all remotes together. A remote can be many things, but in the context of what we will be learning, a remote is essentially a single page react application. 

Often time a host can extend configuration, security, types, routing, and many other features to remotes, so that each remote does not have to implement them individually.

## ▪️ What will we be building?
In this workshop we are going to build a simple application which allows you to view a list of movies and then look at additional details about a select movie. The application will use React, javascript, bootstrap css, module federation, and webpack.

### Solution Structure
For now we will keep the structure loose and simple to understand:

```
.
├── 📁 host
│   ├── 📁 public
│   ├── 📁 src
│   │   ├── 📁 components
│   │   ├── 📁 pages
│   │   ├── 📄 routing.jsx
│   │   └── 📄 index.jsx
│   ├── 📄 webpack.config.js
│   └── 📄 package.json
├── 📁 remotes
│   ├── 📁 home
│   │   ├── 📁 public
│   │   ├── 📁 src
│   │   │   ├── 📄 app.jsx
│   │   │   ├── 📄 bootstrap.js
│   │   │   └── 📄 index.js
│   │   ├── 📄 webpack.config.js
│   │   └── 📄 package.json
│   ├── 📁 list-movies
│   │   └── . . .
│   └── 📁 view-movie
│       └── . . .
├── 📄 package.json
└── 📄 pnpm-workspace.yaml
```

## ▪️ Getting started

1) First off we want to branch or fork this repository. 

2) Secondly we want to create a default package to manage the solution using pnpm and setup pnpm to manage our workspaces. Open a terminal in this directory and execute 
    ```
    npm install -g pnpm
    pnpm init
    ``` 

3) Next we want to create a few directories that represents our solution structure. 
    ```
    mkdir host
    mkdir remotes
    mkdir remotes/home
    mkdir remotes/list-movies
    mkdir remotes/view-movie
    ```

4) Now lets setup our host: First we want to copy down the minimal react mfe template from:
    ```
    https://github.com/cfryerdev/mfe-react-template
    ```
    _Put this in the `host` folder and take a moment to explore the directory and see whats inside._

5) Lets configure the project we just copied and make sure it will function as a container for our remotes.

6) Lets copy down the minimal react mfe template again into each of the remote folders. See step #4.

7) tbd

8) tbd

9) tbd

10) tbd

11) tbd

12) tbd

## Common Questions
Here are some common questions I am often asked:

- **How often or under what circumstances would I create a new host?** Coming soon...
- **Can I use other frameworks instead of React?** Coming soon...
- **What if I want to use NextJS or Remix for my host?** Coming soon...