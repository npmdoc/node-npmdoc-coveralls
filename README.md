# api documentation for  [coveralls (v2.13.0)](https://github.com/nickmerwin/node-coveralls#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-coveralls.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-coveralls) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-coveralls.svg)](https://travis-ci.org/npmdoc/node-npmdoc-coveralls)
#### takes json-cov output into stdin and POSTs to coveralls.io

[![NPM](https://nodei.co/npm/coveralls.png?downloads=true)](https://www.npmjs.com/package/coveralls)

[![apidoc](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-coveralls_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-coveralls/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-coveralls/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gregg Caines"
    },
    "bin": {
        "coveralls": "./bin/coveralls.js"
    },
    "bugs": {
        "url": "https://github.com/nickmerwin/node-coveralls/issues"
    },
    "contributors": [
        {
            "name": "Gregg Caines",
            "email": "gregg@caines.ca",
            "url": "http://caines.ca"
        },
        {
            "name": "Joshua Ma",
            "email": "github@joshma.com",
            "url": "http://joshma.com"
        },
        {
            "name": "Alan Gutierrez",
            "email": "alan@prettyrobots.com",
            "url": "http://www.prettyrobots.com/"
        },
        {
            "name": "Kir Belevich",
            "url": "https://github.com/svg"
        },
        {
            "name": "elliotcable",
            "email": "github@elliottcable.name",
            "url": "http://elliottcable.name/"
        },
        {
            "name": "Slotos",
            "email": "slotos@gmail.com",
            "url": "http://slotos.net"
        },
        {
            "name": "mattjmorrison",
            "email": "mattjmorrison@mattjmorrison.com",
            "url": "http://mattjmorrison.com"
        },
        {
            "name": "Arpad Borsos",
            "email": "arpad.borsos@googlemail.com",
            "url": "http://swatinem.de/"
        },
        {
            "name": "Adam Moss",
            "url": "https://github.com/adam-moss"
        }
    ],
    "dependencies": {
        "js-yaml": "3.6.1",
        "lcov-parse": "0.0.10",
        "log-driver": "1.2.5",
        "minimist": "1.2.0",
        "request": "2.79.0"
    },
    "description": "takes json-cov output into stdin and POSTs to coveralls.io",
    "devDependencies": {
        "istanbul": "0.4.5",
        "jshint": "2.9.3",
        "mocha": "3.2.0",
        "mocha-lcov-reporter": "1.2.0",
        "should": "9.0.2",
        "sinon-restore": "1.0.1",
        "snyk": "1.23.3"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "df933876e8c6f478efb04f4d3ab70dc96b7e5a8e",
        "tarball": "https://registry.npmjs.org/coveralls/-/coveralls-2.13.0.tgz"
    },
    "engines": {
        "node": ">=0.8.6"
    },
    "gitHead": "28212004077299a871a6216273cce7a502e2ce67",
    "homepage": "https://github.com/nickmerwin/node-coveralls#readme",
    "keywords": [
        "coverage",
        "coveralls"
    ],
    "license": "BSD-2-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "cainus",
            "email": "gregg@caines.ca"
        },
        {
            "name": "nickmerwin",
            "email": "n@mer.fm"
        }
    ],
    "name": "coveralls",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/nickmerwin/node-coveralls.git"
    },
    "scripts": {
        "test": "snyk test && make test"
    },
    "version": "2.13.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module coveralls](#apidoc.module.coveralls)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>convertLcovToCoveralls (input, options, cb)](#apidoc.element.coveralls.convertLcovToCoveralls)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>getBaseOptions (cb)](#apidoc.element.coveralls.getBaseOptions)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>getOptions (cb, _userOptions)](#apidoc.element.coveralls.getOptions)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>handleInput (input, cb, userOptions)](#apidoc.element.coveralls.handleInput)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>logger ()](#apidoc.element.coveralls.logger)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>sendToCoveralls (obj, cb)](#apidoc.element.coveralls.sendToCoveralls)
1.  object <span class="apidocSignatureSpan">coveralls.</span>options

#### [module coveralls.getOptions](#apidoc.module.coveralls.getOptions)
1.  [function <span class="apidocSignatureSpan">coveralls.</span>getOptions (cb, _userOptions)](#apidoc.element.coveralls.getOptions.getOptions)
1.  [function <span class="apidocSignatureSpan">coveralls.getOptions.</span>getBaseOptions (cb)](#apidoc.element.coveralls.getOptions.getBaseOptions)



# <a name="apidoc.module.coveralls"></a>[module coveralls](#apidoc.module.coveralls)

#### <a name="apidoc.element.coveralls.convertLcovToCoveralls"></a>[function <span class="apidocSignatureSpan">coveralls.</span>convertLcovToCoveralls (input, options, cb)](#apidoc.element.coveralls.convertLcovToCoveralls)
- description and source-code
```javascript
convertLcovToCoveralls = function (input, options, cb){
  var filepath = options.filepath || '';
  logger.debug("in: ", filepath);
  filepath = path.resolve(process.cwd(), filepath);
  lcovParse(input, function(err, parsed){
    if (err){
      logger.error("error from lcovParse: ", err);
      logger.error("input: ", input);
      return cb(err);
    }
    var postJson = {
      source_files : []
    };
    if (options.git){
      postJson.git = options.git;
    }
    if (options.run_at){
      postJson.run_at = options.run_at;
    }
    if (options.service_name){
      postJson.service_name = options.service_name;
    }
    if (options.service_job_id){
      postJson.service_job_id = options.service_job_id;
    }
    if (options.service_pull_request) {
      postJson.service_pull_request = options.service_pull_request;
    }
    if (options.repo_token) {
      postJson.repo_token = options.repo_token;
    }
    if (options.parallel) {
      postJson.parallel = options.parallel;
    }
    if (options.service_pull_request) {
      postJson.service_pull_request = options.service_pull_request;
    }
    parsed.forEach(function(file){
      file.file = cleanFilePath(file.file);
      var currentFilePath = path.resolve(filepath, file.file);
      if (fs.existsSync(currentFilePath)) {
        postJson.source_files.push(convertLcovFileObject(file, filepath));
      }
    });
    return cb(null, postJson);
  });
}
```
- example usage
```shell
...
if (err){
  logger.error("error from getOptions");
  cb(err);
  return;
}
logger.debug(options);

index.convertLcovToCoveralls(input, options, function(err, postData){
  if (err){
    logger.error("error from convertLcovToCoveralls");
    cb(err);
    return;
  }
  logger.info("sending this to coveralls.io: ", JSON.stringify(postData));
  index.sendToCoveralls(postData, function(err, response, body){
...
```

#### <a name="apidoc.element.coveralls.getBaseOptions"></a>[function <span class="apidocSignatureSpan">coveralls.</span>getBaseOptions (cb)](#apidoc.element.coveralls.getBaseOptions)
- description and source-code
```javascript
getBaseOptions = function (cb){
  var options = {};
  var git_commit = process.env.COVERALLS_GIT_COMMIT;
  var git_branch = process.env.COVERALLS_GIT_BRANCH;
  var git_committer_name, git_committer_email, git_message;

  var match = (process.env.CI_PULL_REQUEST || "").match(/(\d+)$/);

  if (match) {
    options.service_pull_request = match[1];
  }

  if (process.env.TRAVIS){
    options.service_name = 'travis-ci';
    options.service_job_id = process.env.TRAVIS_JOB_ID;
    options.service_pull_request = process.env.TRAVIS_PULL_REQUEST;
    git_commit = 'HEAD';
    git_branch = process.env.TRAVIS_BRANCH;
  }


  if (process.env.DRONE){
    options.service_name = 'drone';
    options.service_job_id = process.env.DRONE_BUILD_NUMBER;
    options.service_pull_request = process.env.DRONE_PULL_REQUEST;
    git_committer_name = process.env.DRONE_COMMIT_AUTHOR;
    git_committer_email = process.env.DRONE_COMMIT_AUTHOR_EMAIL;
    git_commit = process.env.DRONE_COMMIT;
    git_branch = process.env.DRONE_BRANCH;
    git_message = process.env.DRONE_COMMIT_MESSAGE;
  }

  if (process.env.JENKINS_URL){
    options.service_name = 'jenkins';
    options.service_job_id = process.env.BUILD_ID;
    options.service_pull_request = process.env.ghprbPullId;
    git_commit = process.env.GIT_COMMIT;
    git_branch = process.env.GIT_BRANCH;
  }

  if (process.env.CIRCLECI){
    options.service_name = 'circleci';
    options.service_job_id = process.env.CIRCLE_BUILD_NUM;

    if (process.env.CI_PULL_REQUEST) {
      var pr = process.env.CI_PULL_REQUEST.split('/pull/');
      options.service_pull_request = pr[1];
    }
    git_commit = process.env.CIRCLE_SHA1;
    git_branch = process.env.CIRCLE_BRANCH;
  }

  if (process.env.CI_NAME && process.env.CI_NAME === 'codeship'){
    options.service_name = 'codeship';
    options.service_job_id = process.env.CI_BUILD_NUMBER;
    git_commit = process.env.CI_COMMIT_ID;
    git_branch = process.env.CI_BRANCH;
    git_committer_name = process.env.CI_COMMITTER_NAME;
    git_committer_email = process.env.CI_COMMITTER_EMAIL;
    git_message = process.env.CI_COMMIT_MESSAGE;
  }

  if (process.env.WERCKER){
    options.service_name = 'wercker';
    options.service_job_id = process.env.WERCKER_BUILD_ID;
    git_commit = process.env.WERCKER_GIT_COMMIT;
    git_branch = process.env.WERCKER_GIT_BRANCH;
  }

  if (process.env.GITLAB_CI){
    options.service_name = 'gitlab-ci';
    options.service_job_number = process.env.CI_BUILD_NAME;
    options.service_job_id = process.env.CI_BUILD_ID;
    git_commit = process.env.CI_BUILD_REF;
    git_branch = process.env.CI_BUILD_REF_NAME;
  }
  if(process.env.APPVEYOR){
    options.service_name = 'appveyor';
    options.service_job_number = process.env.APPVEYOR_BUILD_NUMBER;
    options.service_job_id = process.env.APPVEYOR_BUILD_ID;
    git_commit = process.env.APPVEYOR_REPO_COMMIT;
    git_branch = process.env.APPVEYOR_REPO_BRANCH;
  }
  if(process.env.SURF_SHA1){
    options.service_name = 'surf';
    git_commit = process.env.SURF_SHA1;
    git_branch = process.env.SURF_REF;
  }
  options.run_at = process.env.COVERALLS_RUN_AT || JSON.stringify(new Date()).slice(1, -1);
  if (process.env.COVERALLS_SERVICE_NAME){
    options.service_name = process.env.COVERALLS_SERVICE_NAME;
  }
  if (process.env.COVERALLS_SERVICE_JOB_ID){
    options.service_job_id = process.env.COVERALLS_SERVICE_JOB_ID;
  }

  if (!git_commit || !git_branch) {
    var data = require('./detectLocalGit')();
    if (data) {
      git_commit = git_commit || data.git_commit;
      git_branch = git_branch || data.git_branch;
    }
  }

  if (process.env.COVERALLS_PARALLEL) {
    options.parallel = true;
  }

  // try to get the repo token as an environment variable
  if (process.env.COVERALLS_REPO_TOKEN) {
    options.repo_token = process.env.COVERALLS_REPO_TOKEN;
  } else {
    // try to get the repo token from a .coveralls.yml file
    var yml = path.join(process.cwd(), '.coveralls.yml');
    try {
      if (fs.statSync(yml).isFile()) {
        var coveralls_yaml_conf = yaml.safeLoad(fs.readFileSync(yml, 'utf8'));
        options. ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coveralls.getOptions"></a>[function <span class="apidocSignatureSpan">coveralls.</span>getOptions (cb, _userOptions)](#apidoc.element.coveralls.getOptions)
- description and source-code
```javascript
getOptions = function (cb, _userOptions){
  if (!cb){
    throw new Error('getOptions requires a callback');
  }

  var userOptions = _userOptions || {};

  getBaseOptions(function(err, options){
    // minimist populates options._ with non-option command line arguments
    var firstNonOptionArgument = index.options._[0];

    if (firstNonOptionArgument)
      options.filepath = firstNonOptionArgument;

    // lodash or else would be better, but no need for the extra dependency
    for (var option in userOptions) {
      options[option] = userOptions[option];
    }
    cb(err, options);
  });
}
```
- example usage
```shell
...

var index = require('../index');
var logger = require('./logger')();

function handleInput(input, cb, userOptions) {
  logger.debug(input);
  logger.debug('user options ' + userOptions);
	index.getOptions(function(err, options){

if (err){
  logger.error("error from getOptions");
  cb(err);
  return;
}
logger.debug(options);
...
```

#### <a name="apidoc.element.coveralls.handleInput"></a>[function <span class="apidocSignatureSpan">coveralls.</span>handleInput (input, cb, userOptions)](#apidoc.element.coveralls.handleInput)
- description and source-code
```javascript
function handleInput(input, cb, userOptions) {
  logger.debug(input);
  logger.debug('user options ' + userOptions);
	index.getOptions(function(err, options){

    if (err){
      logger.error("error from getOptions");
      cb(err);
      return;
    }
    logger.debug(options);

    index.convertLcovToCoveralls(input, options, function(err, postData){
      if (err){
        logger.error("error from convertLcovToCoveralls");
        cb(err);
        return;
      }
      logger.info("sending this to coveralls.io: ", JSON.stringify(postData));
      index.sendToCoveralls(postData, function(err, response, body){
        if (err){
          cb(err);
          return;
        }
        if (response.statusCode >= 400){
          cb("Bad response: " + response.statusCode + " " + body);
          return;
        }
        logger.debug(response.statusCode);
        logger.debug(body);
        cb(null);
      });
    });
  }, userOptions);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coveralls.logger"></a>[function <span class="apidocSignatureSpan">coveralls.</span>logger ()](#apidoc.element.coveralls.logger)
- description and source-code
```javascript
logger = function (){
  return require('log-driver')({level : getLogLevel()});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.coveralls.sendToCoveralls"></a>[function <span class="apidocSignatureSpan">coveralls.</span>sendToCoveralls (obj, cb)](#apidoc.element.coveralls.sendToCoveralls)
- description and source-code
```javascript
sendToCoveralls = function (obj, cb){
  var urlBase = 'https://coveralls.io';
  if (process.env.COVERALLS_ENDPOINT) {
    urlBase = process.env.COVERALLS_ENDPOINT;
  }

  var str = JSON.stringify(obj);
  var url = urlBase + '/api/v1/jobs';

  if (index.options.stdout) {
    process.stdout.write(str);
    cb(null, { statusCode: 200 }, '');
  } else {
    request.post({url : url, form : { json : str}}, function(err, response, body){
      cb(err, response, body);
    });
  }
}
```
- example usage
```shell
...
    index.convertLcovToCoveralls(input, options, function(err, postData){
if (err){
  logger.error("error from convertLcovToCoveralls");
  cb(err);
  return;
}
logger.info("sending this to coveralls.io: ", JSON.stringify(postData));
index.sendToCoveralls(postData, function(err, response, body){
  if (err){
    cb(err);
    return;
  }
  if (response.statusCode >= 400){
    cb("Bad response: " + response.statusCode + " " + body);
    return;
...
```



# <a name="apidoc.module.coveralls.getOptions"></a>[module coveralls.getOptions](#apidoc.module.coveralls.getOptions)

#### <a name="apidoc.element.coveralls.getOptions.getOptions"></a>[function <span class="apidocSignatureSpan">coveralls.</span>getOptions (cb, _userOptions)](#apidoc.element.coveralls.getOptions.getOptions)
- description and source-code
```javascript
getOptions = function (cb, _userOptions){
  if (!cb){
    throw new Error('getOptions requires a callback');
  }

  var userOptions = _userOptions || {};

  getBaseOptions(function(err, options){
    // minimist populates options._ with non-option command line arguments
    var firstNonOptionArgument = index.options._[0];

    if (firstNonOptionArgument)
      options.filepath = firstNonOptionArgument;

    // lodash or else would be better, but no need for the extra dependency
    for (var option in userOptions) {
      options[option] = userOptions[option];
    }
    cb(err, options);
  });
}
```
- example usage
```shell
...

var index = require('../index');
var logger = require('./logger')();

function handleInput(input, cb, userOptions) {
  logger.debug(input);
  logger.debug('user options ' + userOptions);
	index.getOptions(function(err, options){

if (err){
  logger.error("error from getOptions");
  cb(err);
  return;
}
logger.debug(options);
...
```

#### <a name="apidoc.element.coveralls.getOptions.getBaseOptions"></a>[function <span class="apidocSignatureSpan">coveralls.getOptions.</span>getBaseOptions (cb)](#apidoc.element.coveralls.getOptions.getBaseOptions)
- description and source-code
```javascript
getBaseOptions = function (cb){
  var options = {};
  var git_commit = process.env.COVERALLS_GIT_COMMIT;
  var git_branch = process.env.COVERALLS_GIT_BRANCH;
  var git_committer_name, git_committer_email, git_message;

  var match = (process.env.CI_PULL_REQUEST || "").match(/(\d+)$/);

  if (match) {
    options.service_pull_request = match[1];
  }

  if (process.env.TRAVIS){
    options.service_name = 'travis-ci';
    options.service_job_id = process.env.TRAVIS_JOB_ID;
    options.service_pull_request = process.env.TRAVIS_PULL_REQUEST;
    git_commit = 'HEAD';
    git_branch = process.env.TRAVIS_BRANCH;
  }


  if (process.env.DRONE){
    options.service_name = 'drone';
    options.service_job_id = process.env.DRONE_BUILD_NUMBER;
    options.service_pull_request = process.env.DRONE_PULL_REQUEST;
    git_committer_name = process.env.DRONE_COMMIT_AUTHOR;
    git_committer_email = process.env.DRONE_COMMIT_AUTHOR_EMAIL;
    git_commit = process.env.DRONE_COMMIT;
    git_branch = process.env.DRONE_BRANCH;
    git_message = process.env.DRONE_COMMIT_MESSAGE;
  }

  if (process.env.JENKINS_URL){
    options.service_name = 'jenkins';
    options.service_job_id = process.env.BUILD_ID;
    options.service_pull_request = process.env.ghprbPullId;
    git_commit = process.env.GIT_COMMIT;
    git_branch = process.env.GIT_BRANCH;
  }

  if (process.env.CIRCLECI){
    options.service_name = 'circleci';
    options.service_job_id = process.env.CIRCLE_BUILD_NUM;

    if (process.env.CI_PULL_REQUEST) {
      var pr = process.env.CI_PULL_REQUEST.split('/pull/');
      options.service_pull_request = pr[1];
    }
    git_commit = process.env.CIRCLE_SHA1;
    git_branch = process.env.CIRCLE_BRANCH;
  }

  if (process.env.CI_NAME && process.env.CI_NAME === 'codeship'){
    options.service_name = 'codeship';
    options.service_job_id = process.env.CI_BUILD_NUMBER;
    git_commit = process.env.CI_COMMIT_ID;
    git_branch = process.env.CI_BRANCH;
    git_committer_name = process.env.CI_COMMITTER_NAME;
    git_committer_email = process.env.CI_COMMITTER_EMAIL;
    git_message = process.env.CI_COMMIT_MESSAGE;
  }

  if (process.env.WERCKER){
    options.service_name = 'wercker';
    options.service_job_id = process.env.WERCKER_BUILD_ID;
    git_commit = process.env.WERCKER_GIT_COMMIT;
    git_branch = process.env.WERCKER_GIT_BRANCH;
  }

  if (process.env.GITLAB_CI){
    options.service_name = 'gitlab-ci';
    options.service_job_number = process.env.CI_BUILD_NAME;
    options.service_job_id = process.env.CI_BUILD_ID;
    git_commit = process.env.CI_BUILD_REF;
    git_branch = process.env.CI_BUILD_REF_NAME;
  }
  if(process.env.APPVEYOR){
    options.service_name = 'appveyor';
    options.service_job_number = process.env.APPVEYOR_BUILD_NUMBER;
    options.service_job_id = process.env.APPVEYOR_BUILD_ID;
    git_commit = process.env.APPVEYOR_REPO_COMMIT;
    git_branch = process.env.APPVEYOR_REPO_BRANCH;
  }
  if(process.env.SURF_SHA1){
    options.service_name = 'surf';
    git_commit = process.env.SURF_SHA1;
    git_branch = process.env.SURF_REF;
  }
  options.run_at = process.env.COVERALLS_RUN_AT || JSON.stringify(new Date()).slice(1, -1);
  if (process.env.COVERALLS_SERVICE_NAME){
    options.service_name = process.env.COVERALLS_SERVICE_NAME;
  }
  if (process.env.COVERALLS_SERVICE_JOB_ID){
    options.service_job_id = process.env.COVERALLS_SERVICE_JOB_ID;
  }

  if (!git_commit || !git_branch) {
    var data = require('./detectLocalGit')();
    if (data) {
      git_commit = git_commit || data.git_commit;
      git_branch = git_branch || data.git_branch;
    }
  }

  if (process.env.COVERALLS_PARALLEL) {
    options.parallel = true;
  }

  // try to get the repo token as an environment variable
  if (process.env.COVERALLS_REPO_TOKEN) {
    options.repo_token = process.env.COVERALLS_REPO_TOKEN;
  } else {
    // try to get the repo token from a .coveralls.yml file
    var yml = path.join(process.cwd(), '.coveralls.yml');
    try {
      if (fs.statSync(yml).isFile()) {
        var coveralls_yaml_conf = yaml.safeLoad(fs.readFileSync(yml, 'utf8'));
        options. ...
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
