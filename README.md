# ZFVimFormater

vim script to format some file types


# how to use

1. use [Vundle](https://github.com/VundleVim/Vundle.vim) or any other plugin manager you like to install

    ```
    Plugin 'ZSaberLv0/ZFVimFormater'
    Plugin 'ZSaberLv0/ZFVimCmdMenu' " only required if you want the util method ZF_Formater()
    Plugin 'ZSaberLv0/ZFVimBeautifier'
    Plugin 'ZSaberLv0/ZFVimBeautifierTemplate'
    ```

    optional plugin settings for `ZF_FormaterAuto()`:

    ```
    Plugin 'sbdchd/neoformat'
    ```

    recommended external tools for 'sbdchd/neoformat'

    ```
    'apt-get install' : astyle clang-format shfmt swiftformat tidy uncrustify
    'pip install' : cmake_format jsbeautifier sqlparse yapf
    'npm install -g' : eslint lua-fmt prettier typescript typescript-formatter
    ```

1. use the util function to popup a menu to choose

    ```
    call ZF_Formater()
    ```


# functions

* `ZF_Formater()` : popup a menu and choose format function
* `ZF_FormaterAuto()` : format automatically accorrding to filetype (syntax aware)
* `ZF_FormaterXml()` : format xml files (plain regexp replace)
* `ZF_FormaterHtml()` : format html files (plain regexp replace)
* `ZF_FormaterJson()` : format json files (plain regexp replace)

    recommended to install this plugin for better result

    ```
    Plugin 'elzr/vim-json'
    let g:vim_json_syntax_conceal=0
    ```

* `ZF_FormaterMarkdownToHtmlWithWPCodeHighlight()` : format markdown to html that wordpress supported with WP Code Highlight

    require [pandoc](http://pandoc.org/)

* `ZF_FormaterMarkdownToHtml()` : format markdown to html

    require [pandoc](http://pandoc.org/)

* `ZF_FormaterMarkdownToHtmlFile()` : format markdown to html file and save to the same folder

    require [pandoc](http://pandoc.org/)

* `ZF_FormaterMarkdownPreview()` : preview markdown file on your system browser, only for Windows

    require [pandoc](http://pandoc.org/)

* `ZF_FormaterMarkdownInsertTocStyle()` : insert predefined TOC style for markdown
* `ZF_FormaterMarkdownPreviewWithToc()` : preview markdown file on your system browser with a nice TOC style template, only for Windows

    require [pandoc](http://pandoc.org/)

* `ZF_FormaterHtmlPreview()` : preview html file on your system browser, only for Windows

* `ZF_FormaterUnicodePunctuation()` : format unicode punctuation to ansi punctuation

