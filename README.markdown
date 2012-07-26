Redmine Redcarpet Markdown formatter
================================

This is a redmine plugin for supporting Markdown as a wiki format. This plugin use Redcarpet which is GitHub's markdown wiki formatter.
Redcarpet is extreme fast and compatible GitHub's Wiki. They are advantage from Redmine Markdown Formatter and Redmine Markdown Extra Formatter.
This code is originally Redmine Markdown Formatter and Redmine reStructuredtext Formatter. I appreciate these guys.

Additions in the joerocklin fork include:
 * Installation via Bundler
 * no intra-word emphasis on strings_like_this
 * [SmartyPants](http://daringfireball.net/projects/smartypants/) support

What is redmine?
----------------

Redmine is a flexible project management web application.
See [the official site](http://www.redmine.org/) for more details.


What is Markdown?
-----------------------

(from http://daringfireball.net/projects/markdown/)
Markdown is a text-to-HTML conversion tool for web writers. Markdown allows
you to write using an easy-to-read, easy-to-write plain text format, then
convert it to structurally valid XHTML (or HTML).

Prerequisites
-------------

*  Redmine 1.x, Remine 2.x (**Note**: This repo is not being tested with Redmine 1.x)
*  Redcarpetr >= 2.0.0 - see https://github.com/tanoku/redcarpet


Installation
------------

1. Clone and checkout plugin into the appropriate plugins directory

``` 
    cd plugins
    git clone https://github.com/joerocklin/redmine_redcarpet_formatter.git


2.  Install Redcarpet gem. Redcarpet version should be 2.0.0 or later.
```
    bundle install
```
or if you aren't using bundler
```
    sudo gem install --version 2.0.0 redcarpet
```

3.  Run rake at Redmine installed directory.

```
    RAILS_ENV=production rake redmine:plugins:migrate
```

4.  Restart Redmine.
5.  Installed plugins are listed on 'Admin -> Information' screen.
6.  Config Wiki engine for 'markdown' on 'Admin -> Settings -> Text formatting' screen.


Credits
-------
*  ALMinium as the primary maintainers of the plugin (https://github.com/alminium/redmine_redcarpet_formatter)
*  Hiroyuki MORITA (Thanks for multi section edit)
*  mikoto20000 (http://github.com/mikoto20000) develop redmine_redcarpet_formatter
*  Yuki Sonoda (http://github.com/yugui) did the real work by creating the redmine_rd_formatter
*  Larry Baltz (https://github.com/bitherder/) did develop redmine_markdown_formatter
*  william melody(https://github.com/alphabetum) develop redmine_restrucutedtext_formatter

Suggestions, Bugs, Refactoring?
-------------------------------

Fork away and create a Github Issue. Pull requests are welcome.
https://github.com/alminium/redmine_redcarpet_formatter

