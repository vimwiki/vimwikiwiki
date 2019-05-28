# VimwikiWiki

A [Vimwiki Wiki](https://vimwiki.github.io/vimwikiwiki) about Vimwiki.

- `doc/` folder contains generated html served by GitHub pages.
- `wiki/` folder contains the Vimwiki Wiki (default syntax) source files.

To use configure it as an additional wiki in your vimrc:

```
let g:vimwiki_list = [
      \ {
	  <Config of your existing wikis>
      \ },
      \ {
      \         'path': '<path to this repo>/wiki',
      \         'path_html': '<path to this repo>/docs',
      \         'auto_toc': 1},
      \ ]
```

To generate the HTML output run `:Vimwiki2HTML`. For PR commit both the
wikitext and the rendered HTML.
