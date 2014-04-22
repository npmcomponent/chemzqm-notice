*This repository is a mirror of the [component](http://component.io) module [chemzqm/notice](http://github.com/chemzqm/notice). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/chemzqm-notice`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# notice

A notification message component.

A fork with API rework from [yuehu/notice](https://github.com/yuehu/notice).

Showcase at <http://chemzqm.github.io/notice/>.

## Installation

Install with [component(1)](http://component.io):

    $ component install chemzqm/notice

## API

```js
var Notice = require('notice');
var notice = new Notice('show a notice', {
  type: 'success',
  duration: 4000
})
```

### notice(msg, [option])

Show notice with `msg` (String or HTML) and optional option.

* `option.type` could be `success` (implies duration to be 2000) `warning` `error`.
* `option.duration` could be the millisecond to auto hide, no close button when set.
* `option.closable` whether the notice should be closable.

### .hide([ms])

Hide the message in `ms` millisecond, success notice implies auto hide.

### .remove()

Remove the message without animation.

## License

  MIT
