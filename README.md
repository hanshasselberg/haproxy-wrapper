# HAProxy wrapper

HAProxy doesn't support reloading the configuration, it needs to be restarted in a special way. That doesn't play well when HAProxy is managed by upstart or something like that. Most of the solutions I found were tightly coupled to upstart which I don't like. I created a script which wraps HAProxy and which in turn can be used by upstart like any other executable.

My hope is that this becomes a thing ppl like me find easily and saves them hours of research.
