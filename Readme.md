*This repository is a mirror of the [component](http://component.io) module [yields/atkinson](http://github.com/yields/atkinson). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-atkinson`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# Atkinson

  Atkinson can remember form input data across requests, [demo](http://yields.github.io/atkinson/index.html).

## Installation

    $ component install yields/atkinson

## API

### Atkinson.selector

  default selector for `form.querySelectorAll()`.

### Atkinson.store

  localStorage with fallback to an empty object.

### new Atkinson([prefix], form)

  initialize new `Atkinson` instance with the given optional
  `prefix` and `form`.

### atkinson.save()

  use `Atkinson.selector` to find `input, textarea, select` and save
  their values.

### atkinson.restore()

  restore saved data, Atkinson will fill out the form.

### atkinson.clean()

  clean all stored data.

### atkinson.prefix

  the prefix that was passed to `Atkinson` constructor,
  this is defaulted to `form.id`.

### atkinson.el

  the `form` that was passed to `Atkinson` constructor.

### atkinson.selector

  instance selector string, defaulted to `Atkinson.selector`

### atkinson.store

  instance store, defaulted to `Atkinson.store`

## License

  MIT
