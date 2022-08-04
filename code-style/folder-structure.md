# Folder structure

### Structure <a href="#structure" id="structure"></a>

The Source files are placed in `src/` and will be built to `build/`. All other files, that don't need to be build, belong in the `assets/` folder.

#### assets <a href="#assets" id="assets"></a>

* fonts: preferable OTF-files
* icons
* images
* locales: ISO code per translation. E.g.: `nl.json`

#### src <a href="#source" id="source"></a>

* components: folder per component, which can include a test and a separate file with styled components
* screens (mobile) or pages (web)
* services
* utils
* hooks
* store: all files related to our redux state
  * actions
  * reducers
  * thunks
  * sagas or action listeners (optional)
* models
* styles

#### Documentation <a href="#documentation" id="documentation"></a>

All information, regarding the documentation will be placed in this folder. It will be automatically generated when the project folder is opened with the lifecycle-tool.
