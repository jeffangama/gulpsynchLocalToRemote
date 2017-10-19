v1  - MAX / Jeff ANGAMA

# Objective : 
push file to style library using gulp task


# Installation

* npm init
* Copy those dependencies to package.json
```
"gulp": "^3.9.1",
"gulp-clean": "^0.3.2",
"gulp-plumber": "^1.1.0",
"gulp-spsync-creds": "^2.2.6"
```
* npm install --save
* Copy the installation files from InstallationFiles folder to your solution, for info the package contains

```   
src
    style library
        libTest
            example.js
config.json
gulp.js 
settings.js
```

* Configure config.json
        * Inform your site url, credentials (without domain)
        * specify location : style library/libtest (subfolder)
        * publish the file or not ?

# Usage

* A) Push to files to style library immediately. It will create the folder by it self
```
gulp 
```

    or 

* B) Watch changes and push to style library
```
gulp watch
```

* C) if you specified published : false in config.json, it wont get publish until you run
```
gulp publish
```
    
    F5 in browser