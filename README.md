# index-js
gulp pipe for creating index.js files from directories

# Usage: 

in a gulp file

````javascript
var indexJS = require('index-js');

gulp.task('make-indecies', () => {

  var dirs = [ 
      './app/components',
      './app/mixins'
    ];
  return gulp.src(dirs, { base: './' })
          .pipe(indexJS())
          .pipe(gulp.dest('./dist'));
});
````
