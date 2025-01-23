:linux:ls:
to list files by creation/birth date/time, you can use:
ls -t --time=birth
add -r to reverse the order
Source: https://unix.stackexchange.com/questions/20460/how-do-i-do-a-ls-and-then-sort-the-results-by-date-created

:vim:vimwiki:shortcuts:
<leader> ww - open wiki index file
<leader> wt - open wiki index file in a new tab
<leader> ws - list and select available wikis
<leader> wd - delete wiki page
<leader> wr - rename wiki page

<leader> wi - open diary index file for wiki
<leader> w <leader> i - update current diary index
<leader> w <leader> w - open today's diary file for wiki
<leader> w <leader> t - open today's diary file for wiki in new tab
<C-Up> - open previous day's diary
<C-Down> - open next day's diary

:apt:autoremove:
source: https://www.cyberciti.biz/faq/debian-ubuntu-linux-delete-old-kernel-images-command/
On newer system all obsolete kernels and headers should automatically be 
flagged as no more needed, and thus can be purged with the following single 
command: sudo apt --purge autoremove
