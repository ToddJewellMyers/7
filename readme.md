
# Phaser 3 + TypeScript Template


## Template Usage

navigate to to the:

[Generate-Phaser-template](https://github.com/andyroid0/Phaser_template/generate)



## Prerequisites

You'll need [Node.js](https://nodejs.org/en/), [npm](https://www.npmjs.com/), and [Parcel](https://parceljs.org/) installed.



Install Node, then install Parcel:

```bash
npm install -g parcel
```

or 

```bash
yarn add -g parcel
```



## Getting Started

Clone this repository to your local machine:

```bash
git clone https://github.com/andyroid0/Phaser_template.git
```

This will create a folder named `Phaser_template`. You can specify a different folder name like this:

```bash
git clone https://github.com/andyroid0/Phaser_template.git my-folder-name
```

Go into your new project folder and install dependencies:

```bash
cd Phaser_template # or 'my-folder-name'
npm install
```

Start development server:

```
npm run start
```

or 

```
yarn start
```

To create a production build:

```
npm run build
```

or

```
yarn build
```

Production files will be placed in the `dist` folder. Then upload those files to a web server.



## Project Structure

```
    .
    ├── dist
    ├── node_modules
    ├── public
    ├── src
    │   ├── scenes
    │   │   ├── HelloWorldScene.ts
    │   ├── index.html
    │   ├── main.ts
    ├── package.json
```


TypeScript files are intended for the `src` folder. `main.ts` is the entry point referenced by `index.html`.

Other than that there is no opinion on how you should structure your project. There is a `scenes` folder in `src` where the `HelloWorldScene.ts` lives but you can do whatever you want.



## Static Assets

Any static assets like images or audio files should be placed in the `public` folder.

Example `public` structure:

```
    public
    ├── images
    │   ├── my-image.png
    ├── music
    │   ├── ...
    ├── sfx
    │   ├── ...
```

They can then be loaded by Phaser with `this.image.load('my-image', 'my-image.png')`.



## TypeScript ESLint

This template uses a basic `typescript-eslint` set up for code linting.

It does not aim to be opinionated.



## Dev Server Port

You can change the dev server's port number by modifying the `start` script in `package.json`. We use Parcel's `-p` option to specify the port number.

The script looks like this:

```
parcel src/index.html -p 1234
```

Change 1234 to whatever you want.

