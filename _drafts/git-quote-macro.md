CREDIT: https://stackoverflow.com/a/41674859

The macro ways !

press q and q for recording into q register (we use "q" as shortcut to remember "quotes").
press shift + b move cursor to front of current word
press i type ' (a single quotes)
press esc then press e to move to end of word
press a then press ' again to surround the word with quotes.
press esc to get into normal mode.
finally press q to record it into q register.
How to use

Move cursor to desired word.
Press @q to surround a word with quotes.
Press @@ if you want repeat it into another word.
You can alter step 4 with anything you like {a line, a word until found some character, etc}.

Make recorded macro persistent

open .vimrc
go to end of file
change to insert mode. type this to make it persistent:
let @q='ctrl + r ctrl + r q'
save and quit
open your files, go to some words
now press @q
if you do it correctly, magic things should appear in your words.

You can apply this to other macros you loved.
