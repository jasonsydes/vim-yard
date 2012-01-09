# YARD-vim

A [VIM](http://www.vim.org/) plugin which:

* adds syntax highlighting to your [YARD](http://yardoc.org/) tags.
* adds [snipmate](https://github.com/garbas/vim-snipmate) style YARD snippets
  (ported from textmate).

## Install
                                                                                        
If you don't have a preferred installation method, I recommend installing
[pathogen.vim](https://github.com/tpope/vim-pathogen), and then simply copy and
paste:

    cd ~/.vim/bundle
    git clone git://github.com/jasonsydes/vim-yard.git

To get the YARD snippets working with Ruby (without stepping on existing
snippets), I have something like the following in my `.vimrc`:
    
    let g:snipMate = {}
    let g:snipMate.scope_aliases = {}
    let g:snipMate.scope_aliases['ruby'] = 'ruby,ruby-yard'

There's definitely a slicker way to do add the `ruby-yard` stanza to
`scope_aliases` within the plugin itself without overwriting any existing
settings, but I'm relatively new to vim for the moment.  Please feel free to
contact me with suggestions (via email or forks).

### Thanks 

Thanks to [Postmodern](https://github.com/postmodern) for their [YARD syntax
highlighting](https://github.com/postmodern/vim-yard) from which this fork is
derived.
