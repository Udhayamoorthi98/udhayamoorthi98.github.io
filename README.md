# udhayamoorthi98.github.io
# Github-Documentation-With-Doxygen

Automatically deploy your documentation of your project without any CI pipelines. This is achieved by using github actions along with github pages.

Doxygen with auto deployment has been setup in this repository. The documentation for this repository is available at https://github.com/Udhayamoorthi98/eXAMPLE/blob/gh-pages/doc/html/main1_8c.html/

## Doxygen - Documentation Setup
Skip this if you already have doxygen configured 
* Install `doxygen`
    * macOS - `brew install doxygen`
    * Ubuntu - `sudo apt-get install -y doxygen`
* Create doxygen config file (Doxyfile). Run `doxygen -g`
* Configure `Doxyfile`
    * Set `RECURSIVE` to `YES`
    * Set `EXCLUDE` and `EXCLUDE_PATTERNS` to exclude directories you don't want documented. Typically library code and plugins come here. 
    * Set `PROJECT_NAME` to the name of your project
* Optionally add `html` and `latex` to `.gitignore` file
* Document your code according to Doxygen guidlines
    * Check `src/main.c` for C style documentation. Output can be seen [here](https://udhayamoorthi98.github.io/).
   
## Configuring automatic publishing using github actions
* Copy the action file `main.yml` to `.github/workflows/main.yml`
* Commit and Push to github
* Github action should automatically start running
* Confirm that github is set to deploy `gh-pages` branch in settings page

## Notes
* Ensure that `publish_dir` in `main.yml` is set correctly
