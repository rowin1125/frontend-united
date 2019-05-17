# Una Kravets

## CSS

We still have issues in the CSS and have a hard time with write good CSS

- forms are hard
- Comic gradiant aren't available
- The list is still huge

## We now have Houdini

What does it mean and what is the problem?

- if we want to do things which arent supported... we need to polyfill wioth JS

What does houdini

- Polyfill your missing pieces in the web
- Check for coverage houdinireadyyet.com

## CSS variables

what is this:

- `--color: yellow` => this is how the variable is defined
- can also make a variable defined in the code which uses the variable: `--color: newcolor` => `--newcolor: black`

We can make use of the type object modal:

- `element.computedstyleMap().set('height') || element.computedstyleMap().get('height)`
- This will generate direct css without parsing the strings first, which means .. FASTER

Make use of the service workers to register worklet definitions.

- Use the CSS paint API
- this means you can use this inside your css
- This is JS in css.. pretty cooool

## Houdini does:

- Make custom layout
- Make Animations + available API
- Polyfill everything
- https://github.com/GoogleChromeLabs
