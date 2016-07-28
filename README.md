# Extended Live Archive
A modernization of the Extended Live Archive from yesteryear. 

## Original Readme file from version 0.10beta
The Extended Live Archive plugin is one selfcontained bundle called af-extended-live-archive, which should be put into the plugin folder to yield the following structure:

```
wp-content/
		\_...
		\_ plugins/
	   		\_...
	   		\_ af-extended-live-archive/
	   		    \_ elalicenses.txt
				\_ af-extended-live-archive.php
				\_ af-extended-live-archive-include.php
				\_ af-extended-live-archive-options.php
	   			\_ includes/
					\_ af-extended-live-archive.js
					\_ af-ela.php
					\_ af-ela-style.css
				\_ cache/
				    \_ empty directory used to store the cache files
```

The plugin provides a single template function called ```af_ela_super_archive()```. It writes some javascript information in the page it's called in and initializes the whole thing. Some parameter can be passed to the template function.

**However, it is STRONGLY recommended that one uses the option panel the plugin is adding to the admin pages to configure ELA.**

Doing so, all one has to do to display the Extended Live Archive is to add a ```<?php af_ela_super_archive(); ?>``` call wherever one wants the stuff to show up.

Note that if you are using K2, beta one r96 or after, the archives page is already doing that for you.

To install the plugin,

1. upload the af-extended-archive directory and its content to your wp-content/plugins/ directory.
2. make sure the cache directory permission are set to 0777 (refer to your webhost knowledge-base if need be)
3. Then, visit the option->Ext. Live Archive page once to initialize it.

The plugin HomePage can be found somewhere in [SonsOfSkadi.net](http://www.sonsofskadi.net/extended-live-archive/) and the support forum is over at [Flickr](http://www.flickr.com/groups/ela-support/).