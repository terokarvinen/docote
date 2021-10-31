# Docote

Read API docs offline, CLI, supports DevDocs.io compatible JSON files

# Usage

	$ docote sql select|head
	### postgre sql-select ###
	SELECT SELECT, TABLE, WITH — retrieve rows from a table or view   Synopsis [ WITH [ RECURSIVE ] with_query [, ...] ]
	SELECT [ ALL | DISTINCT [ ON ( expression [, ...] ) ] ]
	    [ * | expression [ [ AS ] output_name ] [, ...] ]
	    [ FROM from_item [, ...] ]
	...

# Features

- Supports JSON dictionaries in https://DevDocs.io format. Up to date documentation is available (but not included with docoto) for Python, Go, Postgre, Apache, CSS, DOM, JavaScript, HTML 5, HTTP, Bash, GTK, Godot, jQuery, Leaflet, Lua, MariaDB, nginx, NumPy, Pandas, PHP, PyGame, Qt, Ruby, scikit, SQLite, SVG, TensorFlow, Terraform, Vagrant, Vulkan, Werkzeug and others. 
- Case insensitive AND search

# Use cases

- Search documentation without Internet connection
- Develop your ultra-secret project without revealing your searches to the Internet and search engines
- Quickly search docs without reaching for the mouse

In the future, docoto could be included as plugin to a text editor, such as micro. 

# Install

	$ chmod a+x docote
	$ ./docote

Docote does not include any dictionaries, so feel free to add your own. 

# Limitations

- Not much tested or used in the first release
- HTML tags are stripped from output, but HTML to text parsing is not pretty. E.g. tables are not rendered as ASCII tables
- Search for libraries, but not functions. E.g. can search for "python os.path" but not "python os.path.basename"- Does not automatically invoke $PAGER, but you can pipe output: 'docoto index|less'

# License

Copyright 2021 Tero Karvinen http://TeroKarvinen.com

GNU General Public License, version 3. 

Documentation json dictionaries have their own licences. 
