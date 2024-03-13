# LaunchBar-smart-title-case

A LaunchBar action to convert text to title case ignoring "small words".

As a writer based in Europe I dislike and fear US-style "title case" headlines, which capitalise the first letter of most words. Most word processors and text editors offer a function to convert text to title case, but in my experience this is always a "dumb" process. Small words such as "A" and "The" always end up capitalised, whereas most style guides agree that they should remain lowercase. Remembering which words to capitalise is a challenge for those who deal with title case only infrequently.

John Gruber and many other skilled programmers (I am not one) have created title case converters that are more or less smart in their handling of small words. The basic functionality is not so hard, but the edge cases involving punctuation, acronyms in all caps, and so on can be complicated. Plus, of course, different style guides have different ideas about what constitutes a "small word".

Here is my attempt at a LaunchBar Action to convert selected text to title case. It's based on JavaScript by David Gouch ([https://github.com/gouch/to-title-case]()), derived ultimately I think from John Gruber's original idea. In handling edge cases it's not the best implementation I've seen, but it's the only one I could get to work with LaunchBar and it's good enough for my purposes.

Because the script doesn't touch words in all caps, it has no effect on all-caps headlines. A significant improvement would be to detect and process headlines that are entirely in caps, as opposed to those containing one or more all-caps words. 
