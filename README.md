# __Skript StyleGuide__
Skript is a great way to add scripts to your Minecraft server, it's simple syntax makes it pretty powerful, but also leads to it being really frustrating to organize in to a format that is easily understandable, and that makes it easy for editing later on. This is where I am think that I can help, this is a Skript StyleGuide that lists a variey of best practices to use while writing your scripts, so that they can be easily deciphered in the future if ever neccesary. Lets's begin!
****
## Introductory Comments
Comments in Skript make adding additional information or notes to your script super simple, while also easily making it to 'comment' out some code while testing new code, or if you want to keep it as a reference. Introductory comments are comments that you have in the very begining of the script that describe what it's for, how to use it, and any other information about fair use, or additional arbitrary information. This is only really neccesary in production scripts, or scripts that you will be making publically available.

### _Introduction_
The first part that you should include is the introduction about what the script is for, and what it's used for, this should follow proper grammar and syntax of the given language that's being used. Skript does not offer multiple line comments like some other languages do, meaning we have to use multiple single-line comments so that we can understand the content.

**Spacing** You should leave one space after ever comment character (\#) so that it makes it easier to read, in addition to this if you are making a paragraph you should indent the first sentence of the paragraph so that it follows the english language's standards.

**Line Length** Since not everyone uses word wrap in their editors, often long command continue past the visible window, and require scrolling to see the end, so that the scripts created are more universily formatted, decide on a length which you want the sentences to span, and then make a new line once you hit the end of the allocated line length.

```
#   This is the first sentence of the pargaraph, consisting of a space after the comment character (#) and then
# a tab because it is the first sentence of this paragraph. You may have noticed that this paragraph now spans over
# multiple lines, and this is why every line has a space after the comment character (#), so that you can easily
# read the comments, without issue.
```
****
## Options
Options in Skript are great for if you want to define information that cannot be changed, and can only be called within that specific script, this also comes with the bonus of the value not being stored in which ever system you have decided to use to store your variables. 

#### _Location_
All options should be defined at the top of the script under any information given in comments about the script
