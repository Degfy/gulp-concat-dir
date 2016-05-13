#按目录合并代码

## install
```sh
npm install gulp-concat-dir
```

## example
```js
var gulp = require('gulp');
var concat = require('gulp-concat-dir');

gulp.task('concat',function(){
	return gulp
		.src('src/js/**/*.js')
		.pipe(concat({ext:'.js'}))
		.pipe(gulp.dest('dest/js'));
});
```