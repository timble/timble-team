# Timble - Team

JSON stream & avatars of our team members.

Built to be used in [Jekyll](http://jekyllrb.com/) with [Grunt](http://gruntjs.com/) and [Bower](http://bower.io/).

## Used on

- http://www.timble.net/about/
- https://www.joomlatools.com/about/ & https://www.joomlatools.com/enterprise/

## Install

Add the following dependency to your bower.json file:

```"timble-team": "timble/timble-team"```

Run `bower install`

## Grunt contrib copy example (place in your gruntfile)

```
copy: {
    main: {
        files: [
            {
                expand: true,
                src: ['bower_components/timble-team/images/*.*'],
                dest: 'images/team',
                flatten: true
            },
            {
                expand: true,
                src: ['bower_components/timble-team/team.json'],
                dest: '_data/vendor/timble-team',
                flatten: true
            }
        ]
    }
}
```