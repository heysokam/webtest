# id-Tech3 Mapping Website

## Local development
1. Install Node. [(recommended: `nvm`)](https://github.com/nvm-sh/nvm)  
2. Run `npm start` from the `src/docusaurus` folder.  
   The command will launch a development version of the website that can be accessed from `localhost`.  

## Project Structure
```md
ROOT
 ├─ 🗀 docs
 ├─ 🗀 src
 │   ├─ 🗀 blog
 │   ├─ 🗀 css
 │   ├─ 🗀 docusaurus
 │   ├─ 🗀 pages
 │   ├─ 🗀 static
 │   │   └─ 🗀 img
 │   └─ 🗎 website.config.ts
 └─ 🗀 public
```
### `./docs`
Stores all of the files that will become part of the documentation website.  
### `src/website.config.ts`
Stores all of the site's configuration options in one place for easier/simpler access.  
### `src/docusaurus`
Holds the files required by the framework to work.  
No need to modify anything, so the technical stuff is stored away into this folder.  
Run `npm start` from this folder to launch a development version of the website from `localhost`.
### `src/pages`
Root folder of the pages plugin.  
Every `js,jsx,ts,tsx,md,mdx` file that doesn't start with `_` will be interpreted as a standalone website page.
### `src/css`
Folder where global css files should be stored.  
_note: Not mandatory. Pages could also store their css right next to them as `PAGE.module.css`_
### `src/blog`
_(disabled)_
Holds the content that will show up in the blog section.  
### `./public`
Folder where build files are stored locally when creating a release build.  
Ignored by git. Only for development/testing. The website is deployed into a separate branch.
