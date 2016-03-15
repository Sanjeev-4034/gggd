This is a tool in Python that can fetch the entirety of a Google Group as raw mbox files for easy import into other systems.

Since there is no native way offered by Google to do that, we have to spider the web interface and extract all the messages manually.

# Features

* Fetches all messages in all topics as individual mbox files (one directory per group, one subdirectory per topic, one file per message)
* Can operate on private groups by using lynx' cookie store
* Incremental update mode using RSS
* Postprocessing tool `demangle.py` that fixes two sorts of message munging that google applies (probably a bug on their side).

# Added Feature

* Modified in such a way that it downloades limited topics from a group.

# Usage

 ````
 python gggd.py "group-name" -r "limit"
````

* The changes were made only to the "gggd.py" file.

* In the above instruction "-r" indicates the range that specifies number of topics from which the messages are to be            downloaded.

* you specify the limit in place of "limit".
