# Lorem Ipsum Mixin

Forked from @Longfilename's [Lorem Ipsum Mixin](https://github.com/Longfilename/Lorem-Ipsum-Mixin)

## What this Jade mixin does

1. Generates a number of sentences, words or characters to use in Jade templates.
2. The content is generated in sequence so that it doesn't change on compilation unless you change the templates themselves.
3. Option to add formatting.

## Usage

`+lipsum(amount, type, formatted)`

**"type" is a string that defines why kind of content to get back:**

the possible values are: characters, words, sentences

**"amount" is a number that defines how many of the "type" to get back:**

- `+lipsum(3, "words")` > "Maecenas accumsan aliquet"
- `+lipsum(32, "characters")` > "Cras pede libero dapibus necp u"
- `+lipsum(2, "sentences")` > "Nam quis nulla. Integer malesuada."

**"formatted" (boolean, default = false) is whether to simulate a sentence when selecting "words" or "character" type:**

- `+lipsum(3, "words", true)` > "Maecenas accumsan, aliquet."
- `+lipsum(32, "characters", true)` > "Cras pede, libero dapibus necp."
