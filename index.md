# Measure Once

a game where you repair holes by cutting wood to the right shapes. works best with a gamepad, can be played on keyboard as well.

![screenshot](screenshot.png)

[download for win32](measure once win32.zip)

[play in browser](./play/index.html)

web version known issues:
- west and north on gamepad seem to be switched. looks like a gilrs issue
- audio causes slowdown on first use. looks like a kira issue

[code](https://github.com/robtfm/bevy_carp)

there are lots of things wrong with this code. it is not exemplary, it is more like gamejam code, but maybe some parts will be useful for some people.
- it is mainly uncommented
- it doesn't use any states
- the wood shader is an abomination
- the code is badly organised with too much in main.rs
- the input system is a bit tangled up with the gameplay logic (for movement)
- it uses ActionEvent with &str keys all over the place - it should use separate events, or at least an action enum instead of &str
- etc

it was mainly done because i got tired of not finishing anything, and to see how much effort it takes to get going with sfx, ui, inputs, deployment, etc.
the whole thing was built in around 10 days, which splits up roughly as:
- 20% actual gameplay code
- 20% input management
- 20% graphics/sfx
- 20% ui
- 20% deployment