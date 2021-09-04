### Hi there 

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=udhayamoorthi98)](https://github.com/anuraghazra/github-readme-stats)


### Hi there 👋, udhayamoorthi
#### Design and Engineering
I am udhayamoorthi and I do programming and development.

Skills: C / C++ 

- 🔭 I’m currently working on this page. 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/github.svg' alt='github' height='40'>](https://github.com/         udhayamoorthi)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/stackoverflow.svg' alt='stackoverflow' height='40'>](https://stackoverflow.com/users/https://stackexchange.com/users/22656471/udhayamoorthi)  












# udhayamoorthi98.github.io
# Github-Documentation-With-Doxygen

Automatically deploy your documentation of your project without any CI pipelines. This is achieved by using github actions along with github pages.

Doxygen with auto deployment has been setup in this repository. The documentation for this repository is available at https://github.com/Udhayamoorthi98/udhayamoorthi98.github.io/

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
