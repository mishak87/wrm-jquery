jQuery for Nette projects using Web Resource Management
==========================================================

This is still experimental and I am working on way to circumvent composer definition and need for manual including of config.

## Instalation

### Composer

Add to `composer.json` requirement `"mishak/wrm-jquery": "1.8.3"` and add `jquery/jquery` to repositories:

	"repositories": [
		{
			"type": "package",
			"package": {
				"version": "1.8.3",
				"name": "jquery/jquery",
				"dist": {
					"url": "http://code.jquery.com/jquery-1.8.3.js",
					"type": "file"
				}
			}
		}
	]

### App config

	includes:
		- ../../libs/mishak/wrm-jquery/config.neon

	parameters:
		libsDir: %appDir%/../..
