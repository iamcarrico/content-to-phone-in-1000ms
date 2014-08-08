## Gulpfiles

Your gulpfile.js holds all your tasks within it.

```js
var gulp = require('gulp');
var paths = require('compass-options').dirs();
var compass = require('gulp-compass');
var minifyCSS = require('gulp-minify-css');
var prefix = require('gulp-autoprefixer');

// Compile our Sass, and save the output.
gulp.task('sass', function() {
  return gulp.src(paths.sass + '/**/*.scss')
    .pipe(compass({
      config_file: './config.rb',
      css: paths.css,
      sass: paths.sass,
      bundle_exec: true
    }))
    .pipe(prefix(["last 1 version", "> 1%", "ie 8"]))
    .pipe(minifyCSS())
    .pipe(gulp.dest(paths.css));
});
```

Note: Gulp can do so much, and has the power of Node.js behind it. It is very simple to do a lot of really complex work. For a sample Gulpfile--- check out https://github.com/una/ATXSass/blob/master/gulpfile.js
