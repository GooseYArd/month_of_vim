A Month With Vim

Before ever opening a shell, I ordered a paper copy of "Practical Vim", second
edition, after a bit of googling turned up several endorsements for it. I am
starting this journal a few days after having started the project, but I am very
satisfied by the decision to start with a paper book, away from the computer. I
am also happy about this particular book, as it avoids the tedious patterns that
I encounter in most software books. Drew Neil has a concept about what matters
when learning this software, and he goes straight into it with a minimum of
fluff.

Although there must be ten thousand different vi/vim cheat sheets on the web, I
haplessly landed on this one:

https://hea-www.harvard.edu/~fine/Tech/vi.html

and then spent several days trying to find it again. I like this one in
particular although I am unsure why.

I spent a couple of hours over the first weekend trying some of the examples in
the book, which was enjoyable. I then experimented a little, editing a couple of
files that I needed to change for work.

My method so far has been to avoid creating a vimrc file. I've been through the
process of creating a pathologically enormous editor configuration file that
must be schlepped from machine to machine, carefully curated and organized and
so on. My goal with vim is to adapt to the editor, rather than trying to adapt
it to me. The reason for this is that I have not made any conclusions about
whether, at the end of this month, I will switch from emacs to vim. Instead, I
look at this as a short term assignment to a remote office abroad; I am there to
absorb as much of the culture as possible. Perhaps I will stay, probably not.

Other resources include a graph-ruled steno book. The steno book is a liability,
because I have to remember to take it with me if I want to use it as a resource.
Because there are so many commands to remember, I initially thought I'd use the
steno book to record things I felt were juicy, but possibly difficult enough, to
remember

One concession I made to the minimal-vimrc policy was to add:

    noremap <Up> <NOP>
    noremap <Down> <NOP>
    noremap <Left> <NOP>
    noremap <Right> <NOP>

to try to prevent repeating the mistake I made with emacs, which was to prefer
the arrow keys for most movement, especially now that I don't have to hold a
modifier to use the non-arrow movement keys.

I did notice today that unmapping the arrows that way doesn't stop them working
in insert mode, which makes sense, although I wonder whether I should get into
the habit of switching modes (maybe using the one-shot-normal-mode thing, ctrl-o
or whatever it is) when I find myself arrowing around. Haven't decided yet.

Things which I've had trouble with.

In emacs I usually edit text in text-mode; prior to switching to the XMonad
window manager, I usually left xterms in an 80 column width and I had never
gotten around to setting the paragraph fill width to 80 columns. The result of
this was that I developed the tic of hitting fill-paragraph compulsively to
reflow paragraphs.

Having no .vimrc, I had no default textwidth, and because with the tiler, I get
xterms having all manner of column widths, I elected to add:

    set textwidth=80

I struggle to remember "gqG" or "gqq" to reflow column width after inserting
something; I kept accidentally entering "qqg", which got me into record mode,
which I couldn't figure out how to get out of.



