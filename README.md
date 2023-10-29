# Frontend multipage builder

## Environment requirements

- node v18.18.0
- yarn
- git

## Setup

### 1. Installing project dependencies

To install project dependencies, enter the following commands in the command line:

```bash
yarn
```

If additional packages are required, then to install them, run the command:

- The installation of the package, while the information about it, is automatically registered in the "devDependencies" section of the "
package.json"

```bash
yarn add package_name -D 
```

- The installation of the package, while the information about it is automatically registered in the "dependencies" section of the "package.json"

```bash
yarn add package_name
```

## How to use the environment

- `yarn dev` - start live-server
- `yarn build` - building a project

## Project file structure

```bash
├── dist/                      # compiled project code ready to be hosted on the server
├── public/                    # static project files (images, videos, etc.)
├── src/                       # sources
│   ├── assets/                # resources used in the project (images, fonts, etc.)
│   │   ├── fonts/             # fonts
│   │   └── img/               # images
│   ├── data/                  # arrays of data for output of values in twig files
│   │   └── site.js            # file for data output
│   ├── scripts/               # js filse
│   │   ├── helpers/           # auxiliary js files
│   │   ├── index.js           # the entry point of js files
│   │   └── main/              # js project files
│   ├── styles/                # scss filse
│   │   ├── common/            # basic style files for the project
│   │   ├── components/        # styles for reused parts of the application
│   │   ├── helpers/           # auxiliary css files
│   │   ├── partials/          # styles for logical parts of the application
│   │   └── index.scss         # the entry point of css files
│   ├── templates/             # templates and pieces of code
│   │   ├── layouts/           # page templates
│   │   └── partials/          # pluggable pieces of code
│   └── views/                 # twig files of project pages (converted to html)
│       ├── index.twig         # main page
│       └── ui.twig            # list of site pages
└── vite.config.js             # configuration file vite
```
