# C-VIM

This is a "fork" from the c-vim plugin found in:

- `http://lug.fh-swf.de/vim/vim-c/vim-c.html`
- `http://vim.sourceforge.net/scripts/script.php?script_id=213`

Version 6.0, 2012-08-20

I added some modification basing on my abits. The source code is distributed
under GPL2 http://www.gnu.org/licenses/gpl-2.0.html

Official mailing list: http://lug.fh-swf.de/cgi-bin/mailman/listinfo/vim-plugins-list

## Modification

### Documentation
- This README

### Templates

- **c.comments.template**
  * In the file comment, substituted the description CURSOR with a
     placehodler (I don't like to start in insert mode on new files)
- **c.statements.template**
  * Use of *1TBS* ident style for if/else statement.
- **c.preprocessor.template**
  * Shortcut for including the omonimous local header (*BASENAME.h*)
  * Changed the guard shortcut by using the uppercase *BASENAME*.
- **c.idioms.template**
  * K&R indent style for functions
  * Inserted a return type placeholder instead of *void<CURSOR>*
  * Inserted a shortcut for function declaration

### Vim-core
- **c.vim**
  * Fixed a wrong identifier when loading header templates
  * By default header files are created with comment and guard
  * By default source files are created with comment and the include of the
    omonimous header.
