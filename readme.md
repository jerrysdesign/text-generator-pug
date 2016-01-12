# Lorem Ipsum Mixin

I got tired of going to content generation websites, so I made this mixin. lipsum() is an easy-to-use mixin that will insert as much (random) content as you ask for into the page. No HTML, just content.

It takes three parameters - amount of content, and type ("words", "characters", or "sentences"), and should it add a period (boolean).

## Usage:

lipsum(3, "words", false) > "Maecenas accumsan aliquet"; Capitalises first letter to mimic real world scenario, adds no punctuation;
lipsum(32, "characters", true) > "Cras pede libero, dapibus necp u.";
lipsum(2, "sentences") > "Nam quis nulla. Integer malesuada.";
lipsum(2, "sentences") > "Aenean vel massa quis mauris vehicula lacinia tincidunt scelerisque libero. Maecenas dictum tincidunt diam.";

Each time lipsum() is called the content is randomized again.