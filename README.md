# tipsy

Facebook-style tooltip plugin for jQuery

(c) 2008-2010 Jason Frame (jason@onehackoranother.com)

Released under The MIT License.

## Description:

tipsy is a simple jQuery plugin for generating Facebook-style tooltips.

It's used by Twitter, Github, Slideshare and Bitbucket, amongst others.

## Homepage:

http://onehackoranother.com/projects/jquery/tipsy

## Source:

Hosted at GitHub; browse at:

  http://github.com/jaz303/tipsy/tree/master

Or clone from:

    git://github.com/jaz303/tipsy.git

## Usage:

1. Copy the contents of src/{javascripts,stylesheets} to the corresponding asset directories in your project.

2. Insert the neccesary elements in your document's `<head>` section, e.g.:

        <script type='text/javascript' src='/javascripts/jquery.tipsy.js'></script>
        <link rel="stylesheet" href="/stylesheets/tipsy.css" type="text/css" />

 Remember to include jquery.tipsy.js *after* including the main jQuery library.

3. Initialise Tipsy in your document.onload, e.g.:

        <script type='text/javascript'>
         $(function() {
	       $('a[rel=tipsy]').tipsy({fade: true, gravity: 'n'});
	     });
        </script>

Since jQuery 1.9, 'live' tipsy expects selector as live option, e.g:

        $(document).tipsy({
            live: '.live-tooltip'
        });

## Shadow:

You can add shadow to Tipsy like this :

    <script type='text/javascript'>
         $(function() {
         $('a[rel=tipsy]').tipsy({fade: true, gravity: 'n', shadow: true, shadowBlur: 10, shadowOpacity: 1, shadowSpread: 1});
       });
    </script>
  


Please refer to the docs directory for more examples and documentation.

