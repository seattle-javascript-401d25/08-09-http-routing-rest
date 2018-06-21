![cf](https://i.imgur.com/7v5ASc8.png) 
# Lab 09: Vanilla REST API w/ Persistence

## Submission Instructions
* Work in a fork of this repository
* Work in a branch on your fork called `lab-09`
* **Please make sure to keep work as separate as possible from `lab-08` so TA's can grade accordingly** 
* Create a PR to your master from your working branch.
* Ensure that your repository/branch is connected to travis-ci.com
* Ensure that your repository/branch is connected to Heroku
* Heroku and Travis should pick you up and deploy
* Submit on canvas:
  * a question and observation
  * how long you spent
  * link to your pull request
  * Heroku Server URL (should be the same as what you submitted for Lab 8)
  
## Feature Tasks
* Continue your work from Lab 8
* Add a `storage` directory in your `lib` directory that contains three modules:
    * Move your `storage.js` module from Lab 8 into this directory and rename it `memory.js` (or whatever naming convention you want)
    * Create a new module called `file-system.js` (or whatever you want) where you will write new storage methods that will save and persist your resources to your local file system instead of in memory. Those storage methods should be the same as the MVP requirements for Lab 8: `GET, POST, and DELETE (PUT is extra credit)`
    * Export those modules into an entry point module of your `storage` directory that will rely on an `env` variable to determine which database system you use for your API

## Stretch Goals
* Automatically delete your test files that get created when you run tests if you are using file system storage
* In your `file-system` module, write code that dynamically creates a new resource directory if one is not found, i.e. if there is no **data/Notes** folder, use the `fs` module to create those directories.
* Research and utilize other modules and third party libraries that can automatically promisify your `fs` methods for you without having to manually wrap your code in Promises






