<img style="" src="http://nwjs.io/images/nw.png">

# [NW.js](http://nwjs.io) playground


Project to learn and experiment with [NW.js](http://nwjs.io)

## Installing NW.js

Download and unpack nwjs app for your platform from <http://nwjs.io>

> On OSX you'll end up with `/Applications/nwjs.app`

## Developing Your App

create `index.html` and `package.json` files

> see [nw.js quick-start](https://github.com/nwjs/nw.js#quick-start) for details

## Running

Create alias in `~/.bash_profile`to ease the use from terminal
```bash
# alias to nw
alias nw="/Applications/nwjs.app/Contents/MacOS/nwjs"
```

Run

```bash
cd ~/projects/nwjs-playground
nw .
```

## Packaging as app on OSX

1. Create `.nw` file

	```bash
	cd ~/projects/nwjs-playground
	zip -r ../${PWD##*/}.nw *
	```

	>`.nw` file will be created along side the project directory

2. make copy of `nwjs.app`

	```bash
	cp -r /Applications/nwjs.app /Applications/myapp.app
	```

3. Copy `.nw` file into myapp.app bundle

	```bash
	cp ../nwjs-playground.nw /Applications/myapp.app/Contents/Resources/app.nw
	```