Pathogen
========
Pathogen is a simple library for manipulating comma delimited path options.

The full list of functions includes:

*  pathogen#split:

		convert a comma delimited option to an array
*  pathogen#join:

		convert an array to a comma delimited option
*  pathogen#glob:

		wrapper around glob() that returns an array
*  pathogen#runtime_prepend_subdirectories:

		prepend all subdirectories of a path to the runtimepath and append all after subsubdirectories
*  pathogen#runtime_append_all_bundles:

		for each directory in the runtime path, look for a "bundle" entry and add the subdirectories of it to the path, as with runtime_prepend_subdirectories

Install
-------
1. cd ~/.vim/
2. If your .vim is versioned with git:

		git submodule add git://github.com/paulnicholson/vim-pathogen.git autoload

	or

		git clone git://github.com/paulnicholson/vim-pathogen.git autoload

3. Add the following to your vimrc:

		call pathogen#runtime_append_all_bundles()

After adding this, you can take any plugin, unzip/untar/svn-checkout/git-clone it to its own private directory in .vim/bundle, and it will be added to the runtime path.
This makes it easy to remove or update each plugin individually.
