## Version 1.2.0 (2012-02-06)

Minor:

  * The `Md2Man::Document` module now handles paragraph() nodes and dispatches
    their content accordingly to hook methods for indented, tagged, and normal
    paragraphs.  A Redcarpet markdown parser need only include that module and
    implement those hook methods in order to benefit from md2man's extensions
    to markdown syntax programmatically.

Other:

  * README: mention features; revise markdown; cleanup.

  * LICENSE: @tanoku created initial Manpage renderer.

## Version 1.1.0 (2012-02-02)

Minor:

  * Add `Md2Man::Document` module for programmatic processing of
    cross-references to other UNIX manual pages within Redcarpet.

Other:

  * README: not all systems support `man -l` option.

  * gemspec: upgrade to redcarpet 2.1.0.

  * bundler suggests moving all dev deps into gemspec.

  * README: fix installation commands for development.

  * README: simplify project slogan to be more memorable.

## Version 1.0.2 (2012-01-09)

Patch:

  * Blockquote's leading paragraph regexp was not anchored.

  * Freezing internal constants prevents monkey patching.

Other:

  * Upgraded to Binman 3 for better interoperability with Bundler.

  * Added example input file from the Linux Man Page Howto.

  * Forgot to change project slogan in the gem package.

## Version 1.0.1 (2011-12-06)

Major:

  * Renamed the project from "redcarpet-manpage" to "md2man".

    * `RedcarpetManpage::Renderer` is now `Md2Man::Engine`.

    * `RedcarpetManpage::RENDERER` is now `Md2Man::ENGINE`.

  * Tagged paragraphs no longer require the first line to begin with italic or
    bold styling.  All that matters is that the subsequent lines are indented.

Minor:

  * Added md2man(1) executable for command-line usage.

  * Added support for all HTML 4.0 and XHTML 1.0 entities.

  * Added support for tables, horizontal rules, and more.

  * Added `Md2Man::Roff` mixin for advanced Redcarpet2 usage.

  * Improved README with some new and revised documentation.

Other:

  * Rewrote entire Markdown to Roff conversion from scratch while doing TDD.

## Version 0.0.1 (2011-10-13)

First release! Happy birthday! Woohoo! :-)
