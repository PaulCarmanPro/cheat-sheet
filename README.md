# cheat-sheet

Unfortunately, I use bloated and buggy libreoffice to create cheat sheets. The file takes a long time to load on a Raspberry.

As usual, you may copy my cheat sheets and have them in your posession and do as you please with them . And you may redistribute them in any original or moidifed form where the data is free. I hope that you will creeate another branch and offer edits of any kind you deep appripriate so that the world's best cheat seats can be created and mainttained. It is my intent to keep these cheat sheets in an editable form so that the world may easily improve them.
 
### ToDo

- [ ] Create an emacs mode for cheat sheets . Convert these cheat sheets into raw text containing column formatting inforation unlike markdown or markup because the formmatting data itself not disappar from the text to improve the legibilitty of the content.

emacs proposed columnizer mode: allow column declarations which apply to following lines.
Want to focus upon colors, but emcas does not segregate color from font.

- faces declare colors who parent defines font (allow color declaration)
- single file lacking any hidden data (do not want to retain a secondary buffer).
- column index indicates column (do not want to deal with pixels)
- mono spaced fonts only or misalignment will happen
- tabs cannot be part of data (must be replaced by spaces)
- tab moves cursor to next column
- last column, if left justified, may be varying width
- no line wrap (wrap according to column declarations)
- no line indent

declaration-line = buffer-line whose contents are legally a declaration line
- > begin column here which extends rightward (left justified)
- < end column here which extends leftward (right justified)
- ^ center column here which extends both ways (centered)
- ] force wrapping of previous columns here (inclusive)
- [ force wrapping of next columns here (inclusive)
- | force wrap here and show vertical bar (exclusive)
- : show vertical bar where possible (no force wrap)
- . clear column declaration at this column
- =FACE-NAME declare face to apply to this column 
- (...) declare buffer local face using syntax acceptable to custom-set-faces
data-line = buffer-line whose contents are somehow illegal as declaration line
 
declaration may have a header and a footer which remain visible
- as line declares horizontal separator, end of header or beginning of footer


