A character is some sort of symbol. Then, we might define a string to be a sequence of characters in math and computation. We might take particular interest in different kinds of strings, but first: a language is just a set of strings. A set is just an unordered collection of stuff.

Now, we might be interested in useful things of programming called regular expressions. Regular expressions are formally defined with respect to an alphabet (a set containing all valid characters to use), but for the sake of it, we won't look at a formal definition. A regular expression is useful for programming when you need to see whether a string matches a particular pattern.

For example, consider the regular expression "entries/(x+y+w+z)*entry(0+1+2+...)*" where we use the mathematical notation instead of the programming notation (here, our alphabet contains a-z, 0-9, and slash). This regular expression describes a typical file path for certain types of files; here, we use x, y, w, z as placeholders for characters I actually want to list but won't, for the sake of brevity.

Here, note some ideas of interest. We use brackets to denote sub-expressions for a regular expression. We use + to mean logical OR in the sense of us taking any of the possible characters that are being "added up", so to speak. Lastly, * refers to the Kleene star, which denotes the repetition of the expression to which it applies. You might call the Kleene star a unary operation, but you would need to know what operations are for that explanation to make any sense.

Another note: we say a language is regular if there exists a regular expression which represents every element of the language and nothing else. The pumping lemma is sometimes used to show whether a language is regular. Be on the lookout for more examples!

### Answer

gain access to voidentry(1-7)