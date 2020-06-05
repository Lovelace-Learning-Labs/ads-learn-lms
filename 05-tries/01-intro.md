# Intro

## Learning Goals

By the end of this module, students will be able to...

- **Name** the interface and implementation we'll be studying this week
- **Define** the terms radix, string, prefix and suffix

## Lesson Content

<iframe src="https://adaacademy.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=e043d126-4eae-486e-a0cf-abcf012d3562&autoplay=false&offerviewer=true&showtitle=true&showbrand=false&start=0&interactivity=all" width=720 height=405 style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

### Summary

This week we'll be using the **trie** data structure to implement the **prefix dictionary** interface

Tries are trees optimized for comparing strings

| Term   | Definition                       | Example                                                                                        |
| ------ | -------------------------------- | ---------------------------------------------------------------------------------------------- |
| Radix  | A letter in an alphabet          | 0 and 1 are the radixes of binary, the letters 'a'-'z' are the radixes of the English alphabet |
| String | A sequence of radixes            | 10110 in binary, 'dev' in English                                                              |
| Prefix | Radixes at the front of a string | '', 'd', 'de' and 'dev' are all prefixes of 'dev'                                              |
| Suffix | Radixes at the end of a string   | '', 'v', 'ev' and 'dev' are all suffixes of 'dev'                                              |