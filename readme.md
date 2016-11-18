# Generate Dummy Text for Pug

Forked from @Longfilename's [Lorem Ipsum Mixin](https://github.com/Longfilename/Lorem-Ipsum-Mixin)

## What this Pug mixin does

1. Generates a number of sentences, words or characters to use in Pug templates using lorem ipsum.
2. The content is generated in sequence so that it doesn't change on compilation unless you change the templates themselves.
3. Option to add formatting.

## Usage

`+text-gen(amount, format, sentence)`

@mixin text-gen
@param {number} amount - number of 'types'
@param {string} format - possible values: "characters", "words", "sentences"
@param {boolean} sentence - format as a sentence when using "words" or "character" type

### Examples

- `+text-gen(3, "words")` > "Maecenas accumsan aliquet"
- `+text-gen(32, "characters")` > "Cras pede libero dapibus necp u"
- `+text-gen(2, "sentences")` > "Nam quis nulla. Integer malesuada."

- `+text-gen(3, "words", true)` > "Maecenas accumsan, aliquet."
- `+text-gen(32, "characters", true)` > "Cras pede, libero dapibus necp."
