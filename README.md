Universal Résumé Template
---------

This is my universal resume repository, copied from https://github.com/WebPraktikos/universal-resume/

How to run it
---------

Navigate to the base directory:

```
cd universal-resume
```

Install the dependencies:

```
npm install
```

Start the development server:

```
npm run serve
```

Only generate CSS that is used on the page which results in a much smaller file size:

```
npm run build
```

Starting Point
---------

`docs/index.html` is the main content file. By copying HTML: add pages, sec­tions, subsection, and other parts.

`npm run build` will make **docs** directory ready for drag-n-drop to, for example, https://app.netlify.com/drop (free registration required beforehand). Also, with additionally running `git add docs/styles.css -f` and committing changes, it’s ready for the push to GitHub and integration with GitHub Pages. It may take some time for changes to occur. GitHub Pages are set by configuring `Settings → Options → GitHub Pages → Source → /docs` (free for public repos).


A4 Size Variant
---------

Change the default (letter) size to A4:

**1.** Inside `docs/index.html`, replace every `-letter` with `-a4`.

**2.** Inside `tailwind.config.js`, uncomment code block below `/* For A4 size */` and then comment code block below `/* For Letter size */`

**3.** Inside `tailwind.css`, comment code below `/* For Letter size */` and uncomment code below `/* For A4 size */`

**Important:** Too much content on one page will break the page in the form of additional columns.

Printing
---------

### Chrome

Right-click → Print.  
Also, choose the **Save as PDF** option if needed.

By expanding **More Settings**, change **Page Size** to A4 or Letter.

### Firefox

File → Print.

Choose A4 or Letter size by navigating to **Properties → Advanced → Paper Size**.

### Adobe Acrobat Reader

File → Print.

By clicking on the **Page Setup** button, you are taken to the window with A4 and Letter options.

Blocking Search Engines
---------

Disable search engine indexing by adding the following code to the `<head>`:

```html
<meta name="robots" content="noindex">
```

License
---------

NonCommercial-ShareAlike 1.0 Generic (CC NC-SA 1.0)  
https://creativecommons.org/licenses/nc-sa/1.0/

### You are free to:

Share — copy and redistribute the material in any medium or format  

Adapt — remix, transform, and build upon the material

### Under the following terms:

NonCommercial — You may not use the material for commercial purposes.

ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
