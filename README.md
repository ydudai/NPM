# NPM Node Package Manager Modules | 
NPM Tutorial for Beginners 
by: Dave Gray
-----------------------------------------------------------.     
Youtube lecture: https://www.youtube.com/watch?v=oGO_-DWTmKA  
Site:              https://www.npmjs.com/  
CLI documentation: https://docs.npmjs.com/cli/v10/

1) Install a node package named: **nodemon**  globaly.  
    >**npm i nodemon -g**
    
2) Execute file name **index.js** (the default for nodemon).  
    >**nodemon**   
    
3) Initialize NPM for a project.  
   >cd *[project directory]* .  
   **npm init** 

    - a file *package.json* is created in project directory.
    
4) Install a Package from NPM.  
   >npm i date-fns
    
   - In package.json a field named: *dependencies* is added.  
   - A file *package-lock.json* is created in the project directory.
   - A folder named *node-modules* is added in the project directory.

5) Ignore the folder *node-modules* from git.  
   - Create file .gitignore and write *node-modules* in it. 
   
6) **npm install**.  
   - install a module from node-modules package.json
            
7) Add a development dependency module (modules which is running only in development time not in production).  
    >**npm i nodemon -D**.   
    - A *devDependencies* field is added in package.json
 
8) Create scripts for running in the scripts field in *package.json*
    >**npm start**.  
     Run the start script.  
    >**npm run dev**.  
    run all other scripts which are not named "start"
      
9) Add another Package
    >**npm i uuid  - "uuid"**.    
    - A field was added to dependency
    
10) Version numbers in NPM.  
    **"uuid": "^3.1.9**.  
        ^3.1.9
        ^ - Allow update to the minor version and the patch if needed but do not update              the major version.        
        3 - Major Version.  
        1 - minor Version.  
        9 - a patch.  
        
        3.1.9 (without ^carrot).  
        only this specific version can work.   
        ~ - Allow update the patch version but not the minor version.  
        * - Update everything all the time. Use the absolute latest version every time.
        
11) Install only a specific version.  
    >**npm i uuid@3.1.9**
    
12) Install update of the major Version.  
    **npm update**
    
13) Uninstall a Package.  
    >**npm rm nodemon -D** (D for dev dependencies).  
    **Note:** if a Package is used in script it is not removed automatically.
    
    
