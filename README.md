# Peter Jacobson's solution
## Approach
Use plain React. With just two hours I'll pull in react from a CDN and focus on implementing clean, readable validations.
I prefer writing easily readable code over comments, so will endeavour to make my code self-documenting.

## Technology
React reasonably handles live updating.
In a real project for a form I'd likely use a well supported form library like https://www.npmjs.com/package/informed or https://www.npmjs.com/package/react-redux-form.
React can be slow with unnecessary updating without performance checks via flamegraphs - I'd check these and remove unnecessary component re-renders.
I'd also consider using Redux for state mananagement instead of local react component state depending on other UI & app context.
React took a little while to setup, but makes adding functionality easy when implemented well.

## Tooling
 - Serving: (npm) live-server to hot-reload the code for quicker dev.
 - Editor: Atom-Beta, which has excellent syntax highlighting. I have a number of custom snippets to speed my coding.
 - Debugging: Using the Google Chrome React Extension

## Documentation
 - Mostly through writing well named & readable code
 - Also through succinct and descriptive git commits

## Testing
 - If this was in context of a full react app, I'd TDD the form validations in Jest a separate file and import them.

# End of Peter's solution


# [Form validation problem](https://springload.github.io/form-validation-problem/)

We've created this problem to evaluate how developers tackle a real-world problem. If you've been assigned this problem you should spend around **2 hours** working on it. The last thing we want you to do is toil away for days on end!

If you've stumbled across this and want to work at [Springload](https://www.springload.co.nz/) feel free to submit it too. We're always on the lookout for skilled developers.

## Problem definition

Included in this repository is an [index.html](index.html) file that contains a form. You must ensure all of the following rules are met before the form is posted to the (in this case imaginary) server:

* `Email` must be a valid email address.
* `Password` must be longer than 8 characters.
* `Colour` must be selected.
* At least two `Animal`s must be chosen.
* If `Tiger` is one of the chosen `Animal`s then `Type of tiger` is required to be a non-empty string.

## Other requirements

If the form is submitted and an error occurs, the error element's parent should have a CSS `error` class added to it.

```html
<p class="error">
    <label for="field"></label>
    <input id="field" type="text" value="foo">
</p>
```

Please write a little bit about the technology you chose and why, including any limitations or possibilities of this approach.

## The cherry on the cake

Beyond the problem statement, show us the consideration you have given to some or all of the following:

- Documentation
- Accessibility
- Progressive enhancement
- Browser support
- Testing
- Tooling

## Submission

Please email us a link to your fork of this repository, or a zip of your solution to `1337h4x0r@springload.co.nz`.
