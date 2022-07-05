# Data entry info

This is some info for the data entry job. It doesn't explain everything, just ask any doubts.
Honestly there is a lot of work to do and I'm doing everything 😂

Inside every entry in a json file are some types, this is a short and to the point list.

| word | option         | meaning                                                                    |
| ---- | -------------- | -------------------------------------------------------------------------- |
| type | section        | chapter of the book                                                        |
| type | pf-h1          | chapter title                                                              |
| type | pf-h1-flavour  | cursive text just below the chapter title                                  |
| type | pf-h2          | Title inside the chapter, blue, all caps with bigger capitalized letters   |
| type | pf-h3          | Title inside the chapter, tight, red, all caps, no bigger letter           |
| type | pf-h4          | Title inside the chapter, tight, light-red, all caps, no bigger letter     |
| type | pf-h5          | Title inside the chapter, tight, blue background, all caps, yellow letters |
| type | hr             | Horizontal breakline. It doesn't take any other arguments beside the type  |
| type | list           | List of bullets                                                            |
| type | pf-options     | chapter title                                                              |
| type | table          | table, it takes "rows": [["title 1"]]                                      |
| type | pf2-sidebar    | red sidebar                                                                |
| type | pf2-sample-box | grey box                                                                   |
| type | pf2-brown-box  | brown (bigger) box                                                         |

| at                       | option | description                                       |
| ------------------------ | ------ | ------------------------------------------------- |
| {@b my_text}             | none   | `my_text` will be displayed **bold**              |
| {@i my_text}             | none   | `my_text` will be displayed _italics_             |
| {@note}                  | none   | tiny line in dark gray, to leave notes, you know? |
| {@skill Acrobatics}      | none   | It will hyperlink the Acrobatics Skill            |
| {@actions Sneak}         | none   | It will hyperlink the Sneak action                |
| {@ability darkvision}    | none   | It will hyperlink the action                      |
| {@condition flat-footed} | none   | It will hyperlink the flat-footed condition       |
| {@trait concentrate}     | none   | It will hyperlink the concentrate trait           |
| {@table Skills}          | none   | I have no idea                                    |

Filters also work kinda mysteriously
`{@filter companion's type|companionsfamiliars||Type=Companion}`
idk man, I don't understand this

## Tables

```json
{
  "type": "table",
  "page": 234,
  "colStyles": ["text-center", "text-center", "text-center"],
  "rows": [
    ["General Skill Action", "Proficiency", "Page"],
    ["{@action Decipher Writing}", "Trained", "234"],
    ["{@action Earn Income}", "Trained", "236"]
  ]
}
```
