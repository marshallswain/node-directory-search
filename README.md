node-directory-search
=====================

Recursively search a directory and return a list of matching files.  Currently searches only by matching file extension.

## Usage

	var dirSearch = require('directory-search');

	dirSearch('public', '.css', function(err, results) {
	  if (err) throw err;
	  console.log(results);
	});

Will result in an array that looks something like this:

	[ 'public/styles/app.css',
	  'public/styles/tables.css',
	  'public/styles/home/login.css' ]