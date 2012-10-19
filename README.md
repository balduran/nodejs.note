nodejs.note
===========

## install homebrew

```
ruby -e "$(curl -fsSkL raw.github.com/mxcl/homebrew/go)"

==> This script will install:
/usr/local/bin/brew
/usr/local/Library/...
/usr/local/share/man/man1/brew.1
==> The following directories will be made group writable:
/usr/local/.
/usr/local/bin
==> The following directories will have their group set to admin:
/usr/local/.
/usr/local/bin
```

## install NVM

```
git clone git://github.com/creationix/nvm.git ~/.nvm
echo ". ~/.nvm/nvm.sh" >> ~/.bashrc
source ~/.bashrc 
nvm install v0.6.6
nvm alias default v0.6.6
```
##install jslint

### locally install

```
amountsort-lm:~ balduran$ npm install jslint
npm http GET https://registry.npmjs.org/jslint
npm http 200 https://registry.npmjs.org/jslint
npm http GET https://registry.npmjs.org/jslint/-/jslint-0.1.9.tgz
npm http 200 https://registry.npmjs.org/jslint/-/jslint-0.1.9.tgz
npm http GET https://registry.npmjs.org/nopt
npm http 200 https://registry.npmjs.org/nopt
npm http GET https://registry.npmjs.org/nopt/-/nopt-1.0.10.tgz
npm http 200 https://registry.npmjs.org/nopt/-/nopt-1.0.10.tgz
npm http GET https://registry.npmjs.org/abbrev
npm http 200 https://registry.npmjs.org/abbrev
npm http GET https://registry.npmjs.org/abbrev/-/abbrev-1.0.3.tgz
npm http 200 https://registry.npmjs.org/abbrev/-/abbrev-1.0.3.tgz
jslint@0.1.9 ./node_modules/jslint 
└── nopt@1.0.10
amountsort-lm:~ balduran$ cd node_modules/jslint/
amountsort-lm:jslint balduran$ make lint
find bin lib -name "*.js" -print0 | xargs -0 node ./bin/jslint.js --stupid

bin/jslint.js is OK.

lib/color.js is OK.

lib/linter.js is OK.

lib/nodelint.js is OK.

lib/reporter.js is OK.

lib/jslint.js is OK.
```
### globally install

```
amountsort-lm:jslint balduran$ npm install -g jslint
npm http GET https://registry.npmjs.org/jslint
npm http 304 https://registry.npmjs.org/jslint
npm http GET https://registry.npmjs.org/nopt
npm http 304 https://registry.npmjs.org/nopt
npm http GET https://registry.npmjs.org/abbrev
npm http 304 https://registry.npmjs.org/abbrev
/Users/balduran/.nvm/v0.6.6/bin/jslint -> /Users/balduran/.nvm/v0.6.6/lib/node_modules/jslint/bin/jslint.js
abbrev@1.0.3 /Users/balduran/.nvm/v0.6.6/lib/node_modules/jslint/node_modules/nopt/node_modules/abbrev 
nopt@1.0.10 /Users/balduran/.nvm/v0.6.6/lib/node_modules/jslint/node_modules/nopt 
jslint@0.1.9 /Users/balduran/.nvm/v0.6.6/lib/node_modules/jslint
```

reference <https://github.com/SublimeLinter/SublimeLinter>