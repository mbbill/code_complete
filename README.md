Created by:
Ming Bai

Script type:
Utility

### Description
![Demo](https://web.archive.org/web/20131110125157/http://files.myopera.com/mbbill/files/code_complete.gif)

It shows what this script can do.

In insert mode, when you type `<tab>` (default value of g:completekey) after function name with a `(` , function parameters will be append behind, use `<tab>` key again to switch between parameters.

This key is also used to complete code snippets.

#### Example:
press `<tab>` after function name and `(`

    foo ( <tab>
  
becomes:

    foo ( `<first param>`,`<second param>` )
  
press `<tab>` after code template

    if <tab>
  
becomes:

    if( `<...>` )
    {
        `<...>`
    }

### Code Snippets

Custom snippet files can be used. The default file is
[my_snippets.vim](plugin/my_snippets.vim) and is loaded by default. To add
more custom snippet files (see [my_snippets.vim](plugin/my_snippets.vim) for
the structure), use one of the following variables in your vimrc:

``` viml
let g:user_defined_snippets = "snippets/custom_snippets.vim"
let g:user_defined_snippets = ["snippets/c_snippets.vim", "snippets/js_snippets.vim"]
```
