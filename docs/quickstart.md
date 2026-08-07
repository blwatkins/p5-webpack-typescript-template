---
title: "Quickstart Guide"
layout: post
author:
  - Brittni Watkins
date: 2026-07-30
modified_date: 2026-08-06
toc: true
---

## System Requirements

To use this template, you will first need to have the following software installed on your system:

- Node.js - Current version compatibility is specified in `package.json` under the `engines` field
- npm - Bundled with Node.js installation
- Text editor or IDE of your choice - Visual Studio Code and WebStorm are two popular options for TypeScript development. For a pared down developer experience, you can use a text editor like Sublime Text.
- Web browser of your choice for testing and running your sketches

## Getting Started

### Creating a New Project

To create a new project from this template, you can use the GitHub "Use this template" feature to create a new repository based on this template.
Once your new repository is created, you can clone it to your local machine.

Alternatively, you can download the template source code as a ZIP file and extract it to your desired location.

### Installing Dependencies

Once you have created your new project, navigate to the project directory in your terminal and run the following command:

```shell
npm install
```

`npm install` will install all the dependencies required to test and run this project.

### Project Structure

Source code for your sketches should be placed in the `src/` directory.
The `src/sketch.ts` file provided contains a simple p5.js program with a black background and a white circle.
This file will be used as the entry point for webpack.
The webpack build configuration lives in `webpack.config.mjs`.

Production and development builds are written to the `_dist/` directory, which is generated and not committed.

### Running the Sketch on a localhost Development Server

To test your sketch, navigate to the project directory in your terminal and run the following command:

```shell
npm run dev
```

`npm run dev` will bundle the sketch in development mode, start a localhost development server (`127.0.0.1:8080`), and open a new browser window for the `index.html` file bundled with the compiled sketch.
Development server settings live alongside the build configuration in `webpack.config.mjs`, under the `devServer` object.

### Available npm Scripts

- `npm run lint:js` - lint repository files with `eslint.config.js.mjs`
- `npm run lint:ts` - lint repository files with `eslint.config.ts.mjs`
- `npm run lint:all` - run both lint configurations in sequence
- `npm run build` - bundle the sketch source code and dependencies with `webpack` in production mode
- `npm run build:dev` - bundle the sketch source code and dependencies with `webpack` in development mode
- `npm run build:check` - run both build scripts in sequence
- `npm run serve` - bundle the sketch in production mode, start a localhost development server, and open a new browser window for the `index.html` file bundled with the compiled sketch
- `npm run dev` - bundle the sketch in development mode, start a localhost development server, and open a new browser window for the `index.html` file bundled with the compiled sketch
- `npm run test` - placeholder for a future test runner; the template ships none, and the script exits with an error until one is added
- `npm run validate` - run lint and build checks in sequence

## Resources and References

For additional information about the software and tools discussed in this guide, the following resources may be helpful:

### Node.js and npm Resources

- [Node.js](https://nodejs.org/en/)
- [npm](https://docs.npmjs.com/cli)

### Text Editor and IDE Resources

- [Visual Studio Code](https://code.visualstudio.com/)
- [WebStorm](https://www.jetbrains.com/webstorm/)
- [Sublime Text](https://www.sublimetext.com/)

### Git and GitHub Resources

- [GitHub Docs - Creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
- [Learn to Code, with Brittni Watkins - Create and Clone a GitHub Repository](https://blwatkins.github.io/learn-to-code/git/github/create-and-clone-repo.html)

### Unix Shell

- [Learn to Code, with Brittni Watkins - How to Execute a Unix Shell Command](https://blwatkins.github.io/learn-to-code/unix/commands.html#how-to-execute-a-unix-shell-command)
