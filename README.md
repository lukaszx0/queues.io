# [Queues.io](http://queues.io)

![screenshot](https://s3.amazonaws.com/f.cl.ly/items/3B1k0I2b120K1O0c1P3C/queues-io-2.png)

There's a lot of libraries in many different languages, using various
technologies, implementing "queuing".

All of them are different and were created out of certain need. The purpose of
this project is to collect them all in one place with resources about them.

# Developing

Right now project is based on one simple `erb` template and `projects.yml` file
with all of the data. Template is rendered and saved to `public/` folder as
static html file using:

```
$ bin/compile
```

# Deployment

```
$ bin/deploy
```

You need to install and configure `s3cmd` utility first:

```
$ brew install s3cmd
```

# Contributing

## Guidelines

I want queues.io to be opinionated page with quality resources about queueing
projects. To achieve this I wrote some bullet points I'd like people stick with
when adding new stuff:

  * Project should consist of `name`, `summary`, `url`, `tags`, `links`
  * There should be at least one tag, which should be language/technology in
    which it was created. Other tags can describe for example database used on
    which solution is based (like redis or postgres)
  * There should be at least one link about the library
  * Links should not point to documentation, client libraries or wiki pages.
    They should be well written, valuable blog posts, articles which are harder
    to find than resources provided by creators.

## Github workflow

I would like this to be a community effort. If there's any lib missing, or you
know cool links to articles/videos/slides about ones that are listed, feel free
to add them. I open for any contribution.

  1. Fork it
  2. Create your feature branch (git checkout -b my-new-feature)
  3. Commit your changes (git commit -am 'Add some feature')
  4. Push to the branch (git push origin my-new-feature)
  5. Create new Pull Request
