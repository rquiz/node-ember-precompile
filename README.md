Precompile Handlebars templates for Ember.js

About
-----

Forked from [node-ember-precompile][1] with the intent of making an up-to-date Ember Handlebars compiler available to the Node world.

Install
-------

    npm install -g ember-templates

Usage
-----

This module has a similar interface to the Handlebars precompiler

    ember-templates template... [-f OUTPUT_FILE]

If output file is omitted, the compiled template(s) will be printed to stdout.

The template's name (in the Ember.TEMPLATES object) is created by transforming
the original filename:

 1. the `.handlebars` or `.hbs` file extension is stripped
 2. any remaining `.` characters are replaced by `/` to support
    the [nested templates used by the new Ember Router][2]

[1]: http://github.com/gabrielgrant/node-ember-precompile
[2]: http://emberjs.com/guides/routing/defining-your-routes/#toc_resources
