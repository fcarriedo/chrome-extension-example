# Chrome Extensions Example

Simple Chrome Extension Example that shows
simple ineraction between the background.html, badge
and popup view.

*Best implementation*

Handle all the model in background.html

On update, if popup is visible, push the model to the popup view
and use `backbone.js`, `jQuery` and `jquery-templ` for rendering the model.

### Idea for storing credentials in a shitty secure way

Sate `time to live` in the localStorage, encode the creds with that
number and save them.

For retrieval, use the saved `time to live` number to decode the
credentials and use them. If somebody modifies the `time to live`,
the credentials won't be correctly decoded.
