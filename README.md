# ImageTweak ![ImageTweak icon](http://github.com/CAFxX/ImageTweak/raw/master/skin/imagetweak32.png)
Mozilla Firefox add-on for improving the image viewing UX 

[Homepage](http://cafxx.strayorange.com/ImageTweak) - 
[Downloads](https://addons.mozilla.org/en-US/firefox/addon/3683) - 
[GitHub repository](http://github.com/CAFxX/ImageTweak) - 
[Contact me](mailto:imagetweak@cafxx.strayorange.com)

ImageTweak is an add-on for Firefox, Iceweasel and SeaMonkey that enhances the vision of images in the browser by allowing zooming, rotating and viewing them against a custom/neutral/dark/black background.

## Contribute
You can contribute code to ImageTweak by sending patches or pull requests, a [list of planned features](http://github.com/CAFxX/ImageTweak/wiki) is available. Alternatively you can make donations to support the development of ImageTweak on [addons.mozilla.org](https://addons.mozilla.org/en-US/firefox/addon/3683). 

You can also help by [reporting bugs](http://github.com/CAFxX/ImageTweak/issues) (please, try to be as acccurate as possible by including your OS, browser version, extensions installed, plugins and exact steps to reproduce the bug: if I can't reproduce it, most likely I won't be able to fix it!), [suggesting new features](http://github.com/CAFxX/ImageTweak/wiki) or by [translating ImageTweak in your language](http://www.babelzilla.org/).

## Extension compatibility
Other extensions can use the following function to test if ImageTweak is installed and enabled:

	function isImageTweakEnabled() {
		try {
			return ImageTweakHelper.enabled();
		} catch (e) {
			return false;
		}
	}

The following snippet can be used to test if the document doc is being displayed using ImageTweak

	function isImageTweakDocument(doc) {
		try {
			return ImageTweakHelper.enabledForDocument(doc);
		} catch (e) {
			return false;
		}
	}
    