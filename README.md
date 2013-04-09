# tdbwriter
=========

Write a pseudo-random number (`random.random() * 50.0`) to a TempoDB database every second.

## Instructions:

You should use `virtualenv` to run this project.

```batch
$ virtualenv tdbwriter
$ cd tdbwriter/
$ git clone git://github.com/krallja/tdbwriter.git app/
$ source bin/activate
$ cd app/
$ pip install -r requirements.txt
$ # Set API_KEY and API_SECRET before running:
$ python tdbwriter.py
```

The program uses environment variables to set up its connection to the database:

`API_KEY`, `API_SECRET` - these are required. They can be found on your Database Management page at https://tempo-db.com/manage/

`SERIES_KEY` - defaults to `prng` if not specified.
