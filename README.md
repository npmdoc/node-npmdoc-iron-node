# api documentation for  [iron-node (v3.0.18)](https://github.com/s-a/iron-node#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-iron-node.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-iron-node) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-iron-node.svg)](https://travis-ci.org/npmdoc/node-npmdoc-iron-node)
#### Debug Node.js code on the fly with Chrome Developer Tools on Linux, Windows and OS X.

[![NPM](https://nodei.co/npm/iron-node.png?downloads=true)](https://www.npmjs.com/package/iron-node)

[![apidoc](https://npmdoc.github.io/node-npmdoc-iron-node/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-iron-node_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-iron-node/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-iron-node/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-iron-node/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stephan Ahlf",
        "email": "stephan.ahlf@gmail.com",
        "url": "https://github.com/s-a"
    },
    "bin": {
        "iron-node": "./bin/run.js"
    },
    "bugs": {
        "url": "https://github.com/s-a/iron-node/issues"
    },
    "dependencies": {
        "commander": "^2.9.0",
        "deep-extend": "^0.4.1",
        "electron": "^1.4.15",
        "electron-recompile": "^1.0.16",
        "markdown": "^0.5.0",
        "nmp": "^1.0.3",
        "package.js": "^1.1.3",
        "pretty-error": "^2.0.2",
        "syntax-error": "^1.1.6"
    },
    "description": "Debug Node.js code on the fly with Chrome Developer Tools on Linux, Windows and OS X.",
    "devDependencies": {
        "changelog": "^1.0.7",
        "eslint": "^3.14.1",
        "eslint-config-xo-space": "^0.14.0",
        "jshint": "^2.9.4",
        "mdlint": "^0.1.0",
        "mocha": "^2.5.3",
        "pre-commit": "^1.2.2",
        "should": "^8.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "76d050773f16e66566bcd4ba857c73c1edd27d08",
        "tarball": "https://registry.npmjs.org/iron-node/-/iron-node-3.0.18.tgz"
    },
    "gitHead": "ab6a5aeaab6eb89ad6875176aeadca711471fc0f",
    "homepage": "https://github.com/s-a/iron-node#readme",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "s-a",
            "email": "stephan.ahlf@gmail.com"
        }
    ],
    "name": "iron-node",
    "optionalDependencies": {},
    "pre-commit": [
        "test",
        "mdlint"
    ],
    "preferGlobal": true,
    "productName": "ironNode",
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/s-a/iron-node.git"
    },
    "scripts": {
        "bump": "npm version patch && git push && git push --tags && npm publish",
        "changelog": "node node_modules/changelog/bin/changelog.js all --markdown  > ./CHANGELOG.md",
        "compiler": "electron ./app --compile=c:\\git\\require\\",
        "dev": "node bin/run.js",
        "edge-test": "node bin/run.js ..\\require\\edge.js",
        "err": "node bin/run.js ..\\require\\error.js",
        "mdlint": "rem node_modules/.bin/mdlint glob \"docs/*.md\"",
        "mocha-debug": "electron ./app node_modules/mocha/bin/_mocha",
        "mocha-t": "iron-node node_modules/mocha/bin/_mocha",
        "mocha-test": "node bin/run.js node_modules/mocha/bin/_mocha",
        "node-sass-test": "electron ./app ..\\require\\node-sass.js",
        "pipe-test": "echo var i = 0;debugger; | node bin/run.js",
        "pipe-test-coffee": "coffee -p ./../require/app.coffee | node bin/run.js",
        "start": "node bin/run.js",
        "test": "node node_modules/mocha/bin/_mocha",
        "test-notify": "electron ./app ..\\require\\notify.js",
        "test2": "node bin/run.js ./../test.js"
    },
    "version": "3.0.18"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module iron-node](#apidoc.module.iron-node)
1.  [function <span class="apidocSignatureSpan">iron-node.</span>menu ()](#apidoc.element.iron-node.menu)
1.  [function <span class="apidocSignatureSpan">iron-node.</span>update ()](#apidoc.element.iron-node.update)
1.  object <span class="apidocSignatureSpan">iron-node.</span>_iron_node
1.  object <span class="apidocSignatureSpan">iron-node.</span>menu.prototype
1.  object <span class="apidocSignatureSpan">iron-node.</span>update.prototype

#### [module iron-node._iron_node](#apidoc.module.iron-node._iron_node)
1.  [function <span class="apidocSignatureSpan">iron-node._iron_node.</span>workSpaceDirectory (argv)](#apidoc.element.iron-node._iron_node.workSpaceDirectory)
1.  object <span class="apidocSignatureSpan">iron-node._iron_node.</span>app
1.  object <span class="apidocSignatureSpan">iron-node._iron_node.</span>nodeModule
1.  object <span class="apidocSignatureSpan">iron-node._iron_node.</span>v8

#### [module iron-node.menu](#apidoc.module.iron-node.menu)
1.  [function <span class="apidocSignatureSpan">iron-node.</span>menu ()](#apidoc.element.iron-node.menu.menu)

#### [module iron-node.menu.prototype](#apidoc.module.iron-node.menu.prototype)
1.  [function <span class="apidocSignatureSpan">iron-node.menu.prototype.</span>init (mainWindow)](#apidoc.element.iron-node.menu.prototype.init)

#### [module iron-node.update](#apidoc.module.iron-node.update)
1.  [function <span class="apidocSignatureSpan">iron-node.</span>update ()](#apidoc.element.iron-node.update.update)

#### [module iron-node.update.prototype](#apidoc.module.iron-node.update.prototype)
1.  [function <span class="apidocSignatureSpan">iron-node.update.prototype.</span>check (window)](#apidoc.element.iron-node.update.prototype.check)



# <a name="apidoc.module.iron-node"></a>[module iron-node](#apidoc.module.iron-node)

#### <a name="apidoc.element.iron-node.menu"></a>[function <span class="apidocSignatureSpan">iron-node.</span>menu ()](#apidoc.element.iron-node.menu)
- description and source-code
```javascript
menu = function () {
	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iron-node.update"></a>[function <span class="apidocSignatureSpan">iron-node.</span>update ()](#apidoc.element.iron-node.update)
- description and source-code
```javascript
update = function () {
	return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iron-node._iron_node"></a>[module iron-node._iron_node](#apidoc.module.iron-node._iron_node)

#### <a name="apidoc.element.iron-node._iron_node.workSpaceDirectory"></a>[function <span class="apidocSignatureSpan">iron-node._iron_node.</span>workSpaceDirectory (argv)](#apidoc.element.iron-node._iron_node.workSpaceDirectory)
- description and source-code
```javascript
workSpaceDirectory = function (argv) {  // determines the workspace directory for specific commandline applications.
  var result = "";
  if (argv[2]){
    result = path.dirname(argv[2]);
    var startupScriptName = path.basename(argv[2]).toLowerCase();

    switch(startupScriptName) {
        case "_mocha":
          result = process.cwd();
          break;
        default:
          result = path.resolve(result);
          break;
    }
  }

  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iron-node.menu"></a>[module iron-node.menu](#apidoc.module.iron-node.menu)

#### <a name="apidoc.element.iron-node.menu.menu"></a>[function <span class="apidocSignatureSpan">iron-node.</span>menu ()](#apidoc.element.iron-node.menu.menu)
- description and source-code
```javascript
menu = function () {
	return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iron-node.menu.prototype"></a>[module iron-node.menu.prototype](#apidoc.module.iron-node.menu.prototype)

#### <a name="apidoc.element.iron-node.menu.prototype.init"></a>[function <span class="apidocSignatureSpan">iron-node.menu.prototype.</span>init (mainWindow)](#apidoc.element.iron-node.menu.prototype.init)
- description and source-code
```javascript
init = function (mainWindow) {
	var mnuFile = {
		label: "Project",
		submenu: [
			{
				label: "Exit",
				click: function() {
					mainWindow.close();
				},
				accelerator: "Control+w"
			}
		]
	};

  if (os.platform() === "darwin") {
    mnuFile.submenu.push({
      type: "separator"
    });
    mnuFile.submenu.push({
      label: "Quit ironNode",
      click: function () {
        app.quit();
      },
      accelerator: "Cmd+Q"
    });
  }
	template.push(mnuFile);

	if (os.platform() === "darwin"){
		var mnuEdit = {
			label : "Edit",
			submenu:[
				{
					label: "Cut",
					accelerator: "Cmd+X",
					selector: "cut:"
				},
				{
					label: "Copy",
					accelerator: "Cmd+C",
					selector: "copy:"
				},
				{
					label: "Paste",
					accelerator: "Cmd+V",
					selector: "paste:"
				},
				{
					label: "Select All",
					accelerator: "Cmd+A",
					selector: "selectAll:"
				}
			]
		};

		template.push(mnuEdit);
	}

	var mnuView =   {
		label: "View",
		submenu: [
			{
				label: "Show developer tools",
				click: function() {
					mainWindow.openDevTools();
				},
				accelerator: "F12"
			},
			{
				label: "Show global config folder",
				click: function() {
					var shell = require("electron").shell;
					var f = path.join(app.getPath("appData"), "iron-node");
					if (!fs.existsSync(f)){
						console.warn("No packages folder found. You can install some at " +  path.join( app.getPath("appData"), "iron-node", "node_modules
" ) + " from ", "https://www.npmjs.com/search?q=iron-node", ":O)");
					}
					shell.openItem( f );
				}
			}
		]
	};
	template.push(mnuView);

	var mnuHelp =   {
		label: "Help",
		submenu: [
			{
				label: "Documentation",
				click: function() {
					shell.openExternal("https://developer.chrome.com/devtools/docs/javascript-debugging");
				}
			},
			{
				label: "Report a bug",
				click: function() {
					shell.openExternal("https://github.com/s-a/iron-node/issues");
				}
			},
			{
				type: "separator"
			},
			{
				label: "Source Code",
				click: function() {
					shell.openExternal("https://github.com/s-a/iron-node");
				}
			},
			{
				type: "separator"
			},
			{
				label: "Check for Updates",
				click: function() {
					var upd = new SoftwareUpdate();
					upd.check(mainWindow);
				}
			},
			{
				type: "separator"
			},
			{
				label: "Donate",
				click: function() {
					shell.openExternal("http://s-a.github.io/donate/");
				}
			}
		]
	};
	template.push(mnuHelp);

	var menu = Menu.buildFromTemplate(template);
	Menu.setApplicationMenu(menu);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iron-node.update"></a>[module iron-node.update](#apidoc.module.iron-node.update)

#### <a name="apidoc.element.iron-node.update.update"></a>[function <span class="apidocSignatureSpan">iron-node.</span>update ()](#apidoc.element.iron-node.update.update)
- description and source-code
```javascript
update = function () {
	return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iron-node.update.prototype"></a>[module iron-node.update.prototype](#apidoc.module.iron-node.update.prototype)

#### <a name="apidoc.element.iron-node.update.prototype.check"></a>[function <span class="apidocSignatureSpan">iron-node.update.prototype.</span>check (window)](#apidoc.element.iron-node.update.prototype.check)
- description and source-code
```javascript
check = function (window) {
	dialog.showMessageBox(window, {type:"info", title:"ironNode Update check", message:"Stay tuned. This may take a few seconds.",
detail:"", buttons: ["ok"]});
	execute("npm outdated -g --depth=0 iron-node", function(str){
		dialog.showMessageBox(window, {type:"info", title:"ironNode Update check done", message:str, detail:"", buttons: ["ok"]});
	});
}
```
- example usage
```shell
...
			{
				type: "separator"
			},
			{
				label: "Check for Updates",
				click: function() {
					var upd = new SoftwareUpdate();
					upd.check(mainWindow);
				}
			},
			{
				type: "separator"
			},
			{
				label: "Donate",
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
