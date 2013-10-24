vim-taskwarrior
===============

vim interface for [taskwarrior](http://taskwarrior.org)

*note:* this fork also includes vim ftdetect and syntax files for task edit, taskrc and data files

Should add this line to .taskrc

    defaultwidth=999

Or lines may be awfully wrapped.

And **uuid** field is recommanded in **report.all.columns** to get the exact filter for current task.

Default map:

```vim
nnoremap <buffer> A ... " add annotation
nnoremap <buffer> D ... " delete task
nnoremap <buffer> a ... " create new task.
nnoremap <buffer> d ... " set the task in current line done.
nnoremap <buffer> <CR>. " show task info.
nnoremap <buffer> m ... " modify current task.
nnoremap <buffer> q ... " quit buffer.
nnoremap <buffer> r ... " clear all completed task.
nnoremap <buffer> u ... " undo last change.
nnoremap <buffer> x ... " delete annotation.
nnoremap <buffer> s ... " task summary.
```

Commands:
```vim
:TW            " task list
:TWEditTaskrc  " edit ~/.taskrc
:TWEditVimrc   " edit ~/.vimrc
:TWEditVitrc   " edit ~/.vitrc
:TWSync        " Synchronise with taskd server

```