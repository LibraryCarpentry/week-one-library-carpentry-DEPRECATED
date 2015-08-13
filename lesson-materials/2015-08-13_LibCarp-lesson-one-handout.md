# Library Carpentry Week One: Some Basics

_____
### Regular Expressions

- `[]` define a list or range of characters to be found
- `.` matches any character at all.
- `\d` matches any single digit
- `\w` matches and part of word character (equivalent to [A-Za-z0-9_] )
- `\s` matches any space, tab, or newline
- `^` defines the start of the string
- `$` defines the end of the string
- `*` matches when the proceeding character appears any number of times including zero
- `+` matches when the proceeding character appears any number of times excluding zero
- `?` matches when the proceeding character appears one or zero times
- `{VALUE}` matches the proceeding character the number of times define by VALUE; ranges can be specified with the syntax `{VALUE,VALUE}`
- `|` means or.

Check you regex with regex101: https://regex101.com/

#### Exercise

What does `Fr[ea]nc[eh]` match?

What does `Fr[ea]nc[eh]$` match?

What would match strings that begin with `French` and `France` only? {France|French}

How do you match the words 'colour' and 'color' (case insensitive)? {`colou?r`}

How would you find 'headrest' and 'head rest' but not 'head  rest'? {head\s?rest}

How would you find a 4 letter word that begins a string and is preceded by at least one zero? {0+[a-z]{4}$}

How do you match any 4 digit string? {`\d{4}`}

How would you match the date format 'dd-MM-yyyy'? {`\d{2}-\d{2}-\d{4}`}

How would you match the date format 'dd-MM-yyyy' or 'dd-MM-yy' at the end of a string only? {`\d{2}-\d{2}-\d{2,4}$`}

How would you match a thirteen digital ISBN? {^\d{13}$}

How would you match publication formats such as 'British Library : London, 2015' and 'Manchester University Press : Manchester, 1999'?  {`.* : .*, \d{4}`}

_____
### References

James Baker , "Preserving Your Research Data," *Programming Historian* (30 April 2014), [http://programminghistorian.org/lessons/preserving-your-research-data.html](http://melbourne.resbaz.edu.au/post/95320810834/why-code). The sub-sections 'Plain text formats are your friend' and  'Naming files sensible things is good for you and for your computers' are reworked from this lesson.

Owen Stephens, "Working with Data using OpenRefine", *Overdue Ideas" (19 November 2014), [http://www.meanboyfriend.com/overdue_ideas/2014/11/working-with-data-using-openrefine/](http://www.meanboyfriend.com/overdue_ideas/2014/11/working-with-data-using-openrefine/). The section on 'Regular Expressions' is reworked from this lesson developed by Owen Stephens on behalf of the British Library

Andromeda Yelton, "Coding for Librarians: Learning by Example", *Library Technology Reports* 51:3 (April 2015), doi: [10.5860/ltr.51n3](http://dx.doi.org/10.5860/ltr.51n3)

Fiona Tweedie, "Why Code?", *The Research Bazaar* (October 2014), [http://melbourne.resbaz.edu.au/post/95320810834/why-code](http://melbourne.resbaz.edu.au/post/95320810834/why-code)
