# tablemaker
A program that takes an input:

```
a | b | c
# With comments as well.
e | f | g
h | i |jk
```

And converts it to a table:

```
┌───┬───┬────┐
│ a │ b │ c  │
│ e │ f │ g  │
│ h │ i │ jk │
└───┴───┴────┘
```

Simply create a new `.txt` file that has the same name as `input_filename` in `main.py`. By default, this is pointing toward `raw.txt` The input for the file is pipe-separated lines of code:

```
a ||| b | c |d
     e |f  |g
# The line below this does blah blah blah.
 hij|klmnop|qr
```
Lines that start with `#` are commented out:

```
┌─────┬────────┬────┬───┬───┬───┐
│  a  │        │    │ b │ c │ d │
├─────┼────────┼────┼───┼───┼───┤
│  e  │   f    │ g  │   │   │   │
├─────┼────────┼────┼───┼───┼───┤
│ hij │ klmnop │ qr │   │   │   │
└─────┴────────┴────┴───┴───┴───┘
```

The program requires a user-input to decide between having "bars" between rows in the table or to not have that. (For now- I have commented out this and made it have no bars by default.)

The output will be showcased in the file in the variable `out_filename`. As of now it is `out.txt`.