In this project we're going to:
Create a local git repository
Create a gulp build process
Add a README.md document
Push a branch with latest code up to Github

Read the following instruction to create a similar project.

1. Initialize the app.
    - Open your project folder
    - git init
    - npm install
2. Review the project files.
    - look over the files provided in this project and familiarize yourself with the contents.
3. Create a gulp script -- build:js
    - add the following steps to th gulpfile.js
    Add the following code to define your first task:
    gulp.task('build:js', function() {
        return gulp.src('src/js/*.js')
            .pipe(uglify())
            .pipe(concat('bundle.min.js'))
            .pipe(gulp.dest('dist'))
    });
4. Create a gulp script -- build:css
    - Repeat the code above but with css  contents.
5. Check that your app works.
    - Reload the website and see if it works.
6. Add README.md -- add description on how to recreate the project.