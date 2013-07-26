# Queues.io

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

You need to install and configure `s3cmd` utilty first:

```
$ brew install s3cmd
```

# Contributing

I would like this to be a community effort. If there's any lib missing, or you
know cool links to articles/videos/slides about ones that are listed, feel free
to add them. I open for any contribution.

  1. Fork it
  2. Create your feature branch (git checkout -b my-new-feature)
  3. Commit your changes (git commit -am 'Add some feature')
  4. Push to the branch (git push origin my-new-feature)
  5. Create new Pull Request
