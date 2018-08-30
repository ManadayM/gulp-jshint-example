## Setup
Install dependencies using `npm install`. That's it.

## Run
Execute only `gulp` from the root project directory.

The file at `src/js/frame-mngr.js` contains error and hence should log an error message as `JSHint has caught error` and immediately stop the gulp tasks' execution.

Remove/delete all code from the same file `src/js/frame-mngr.js` to check if everything works when there's no error. If you empty out the file content or delete the file itself. Things should work normally.

![Gulp JSHint in Action](https://raw.githubusercontent.com/ManadayM/gulp-jshint-example/master/gulp-jshint-inaction.gif)

## Useful resources:
- http://dev.topheman.com/gulp-fail-run-sequence-with-a-correct-exit-code/
- https://github.com/spalger/gulp-jshint#custom-reporters
- https://github.com/spalger/gulp-jshint/blob/master/src/reporters/fail.js
- https://github.com/sindresorhus/jshint-stylish/blob/master/index.js
- http://jshint.com/docs/reporters/
- In cases when map-stream (here JSHint Fail Reporter) was being called more than once then I was getting `Error: map stream is not writable` error. This thread was helpful https://github.com/spalger/gulp-jshint/issues/50#issue-35343385
