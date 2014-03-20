coversheet
====

### Purpose

coversheet is used to start a build monitor that
waits for notifications to run tests.

### Usage

1. Create virtualenv via `virtualenv cov`
2. Use the virtualenv with `source cov/bin/activate`
3. Run `python setup.py install`
4. Call coversheet with `coversheet --pulsefile=pulse.json`

An example pulse.json file for Mac OSX:

    {"buildtype": "opt", 
     "buildid": "20110818083549",
     "timestamp": "20110818130551",
     "testsurl": "http://stage.mozilla.org/pub/mozilla.org/firefox/tinderbox-builds/mozilla-central-macosx64/1392339197/firefox-30.0a1.en-US.mac.tests.zip",
     "key": "build.mozilla-central-linux.20.step.maybe_rebooting.finished",
     "builddate": 1392085663,
     "tree": "mozilla-central", 
     "platform": "macosx64", 
     "buildurl": "http://stage.mozilla.org/pub/mozilla.org/firefox/tinderbox-builds/mozilla-central-macosx64/1392339197/firefox-30.0a1.en-US.mac.dmg", 
     "branch": "mozilla-central"}

See [cli.py](https://github.com/jonallengriffin/coversheet/blob/master/coversheet/cli.py#L55) for other command line options.

### Builds

[OSX 64 builds](https://ftp.mozilla.org/pub/mozilla.org/firefox/tinderbox-builds/mozilla-central-macosx64/)

[Win 64 builds](https://ftp.mozilla.org/pub/mozilla.org/firefox/tinderbox-builds/mozilla-central-win64/)

[Linux 64 builds](https://ftp.mozilla.org/pub/mozilla.org/firefox/tinderbox-builds/mozilla-central-win64/)


### Notes

See https://bugzilla.mozilla.org/show_bug.cgi?id=740228
