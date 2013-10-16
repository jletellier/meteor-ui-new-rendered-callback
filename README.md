The new templating engine, part of Meteor UI, changes the way
[template `rendered` callbacks are
fired](https://github.com/meteor/meteor/wiki/New-Template-Engine-Preview#rendered-callback-only-fires-once).

Here's an example of how to achieve the same behavior as the old
`rendered` callback in a simple app. The important issue is that in
the new system you have to be explicit about which modifications
should fire callbacks.

`old/` - An app running against Meteor 0.6.6.1 (with the old `rendered`
behavior)

`new1/` - Resolution #1 (adding a new helper)

`new2/` - Resolution #2 (wrapping the contents of `#each` in a
template)
