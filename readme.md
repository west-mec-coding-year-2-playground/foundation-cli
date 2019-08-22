# About (IN PROGRESS)
A student led forked version of Zurb's command line installer for Foundation 6 customized for fullstack rapid development and extreame programming.

# Branches
1. Master - This is maintained by the instructor(s) to communicate instructions / goals of the project. 
2. Demo - This is used to show students how to customize the CLI.
3. Alpha- Students will teach this like the master branch and only students with the role of "Project Manager" may approve pull requests.
4. QA - This branch is managed by students with the role of "QA". They will be required to write unit-tests, etc for code before it is "released" to Alpha. Students with the role of "Designer" will work to ensure that "user tests" with puppeteer, etc pass. All "**Feature Branches**" must go through this branch before it is merged into Alpha.
5. Various Feature Branches - Students will create issues and related features branches and work as a team to complete the desired feature.

# Minimium Goals (Subject to Change)
  ## Maintainer
  You've picked the most difficult capstone and proven yourself more than capable to work for any company to maintains open source project.
    
    1. Students will create a map/diagram of the decision tree involved with the CLI.
   
    2. Students will use the above to create a map/diagram of the current software architecture and plan out a strategy to meet the deadline (graduation).
    
    3. Student will fix some issues related
   
    4. Students will change the output of all CLI commands.
   
    5. `Foundation new site` will provide users the following options:
      A. West-Mec Template: Everything needed in Extreame Programming.
      B). Theme: Everything needed to build a "modern" static html, css, JS/ES/TS and deploy it to github pages and heroku in under an hour.

  ## Extreame Team
  You've done the "impossible". People said high school students could never accomplish this and you proved them wrong.

    `Foundation new site` will provide users the following options:

    1. Express: A lean fullstack app that uses docker, mongoDB, handlebars, etc and hosted on heroku.  

  ## Innovator
  The highest possible award for C201-C202. You're team is the best of the best and will undoubtedly put so called "10x developers", "rock star developer", etc to shame. Every member has far exceeded any expectation of the instructor, of Wec Mec, the advisory counsel, etc. Recruiter's will absolutely fight over you.

 1. Students have **completely** refactored the CLI to ES6+ in such a way it is completely independant of the original and published on a seperate repo.

 2. The CLI should meet the following standards:
   A). `foundation new client` CLI should be able to create a standalone  boilerplate for used for analyzing a potential client's website, creating a **styleguide** for the client, creating a **proposal** for the client and help provide **documentation** for a project.

      B). `Foundation new site` will provide users the following options:
     1. Theme: Everything needed to build a "modern" static html, css, JS/ES/TS and deploy it to github pages and heroku in under an hour.
     2. West-Mec Template: Everything needed in Extreame Programming.
     3. Express: A lean fullstack app that uses docker, mongoDB, handlebars, etc and hosted on heroku.
     4. React: A boilerplate that uses react-foundation.
     5. MarkoJS: A boilerplate thats uses MarkoJS. Atleast 10 **functional** "blocks" have been converted to markoJS and atleast 20 have been converted to **design** components.
     6. WordPress: Creates a WordPress boilerplate that works with docker in local development, able to be staged with Heroku for free and then integrates with cloud platforms in "production" (D.O. , AWS, AZURE, ETC).

      C). `Foundation new App` will create a boilerplate for a react-ionic mobile app.

      D). `Foundation new email` will provide users the following options:
     1. West-Mec: An email boilerplate used to send west-mec branded email templates.
   
      E). `Foundation block and kits` has been completely rebuilt in a way that html, scss and js are abstracted into the desired framework, ex: converted to react/jsx, marko.js.



# OLD Foundation CLI

This is the command-line interface for [Foundation](https://foundation.zurb.com) family of frameworks.. It downloads and installs blank templates in any of the three Foundation frameworks:

- [Foundation for Sites](https://foundation.zurb.com/sites), a framework for responsive websites.
- [Foundation for Apps](https://foundation.zurb.com/apps), a framework for responsive web apps.
- [Foundation for Emails](https://foundation.zurb.com/emails), a framework for responsive email.


## Requirements

You'll need the following software installed to get started.

  * [Node.js](http://nodejs.org) 0.12+: Use the installer provided on the NodeJS website.
    * With Node installed, run `[sudo] npm install -g gulp bower`.
  * [Git](http://git-scm.com/downloads): Use the installer for your OS.
    * Windows users can also try [Git for Windows](http://git-for-windows.github.io/).

## Installing
**Requres** node version 10.

The Foundation CLI is installed through npm.

```bash
npm install -g foundation-cli
```

This will add the `foundation` command to your system.

### Updating

The CLI periodically gets updates that add features or fix bugs. Use npm to upgrade the CLI to the newest version.

```bash
npm update -g foundation-cli
```

To check what version you currently have, use `-v`.

```bash
foundation -v
```

## Commands

### New

Starts the setup process for a new Foundation project. The CLI will ask you which framework you want to use and a folder name for the project.

```bash
foundation new
```

### Watch

While inside of your app's folder, use the `watch` command to assemble your app and run a test server.

```bash
cd appName
foundation watch
```

While this process is running, you can view the assembled app in your browser, at this URL:

```
http://localhost:8080
```

While the server is running, any changes you make to your HTML, Sass, or JavaScript will automatically be processed and added to your live app.

### Build

To build your app for production, use `foundation build`.

```bash
foundation build
```

### Update

Updates your Bower packages, which includes Foundation. Run this command when you want to update an existing project to the newest version of Foundation.

```bash
foundation update
```

### Help

Lists all available commands in the CLI.

```bash
foundation help
```

Add a command name at the end to learn how a specific command works.

```bash
foundation help new
```
