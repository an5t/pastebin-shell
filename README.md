# pastebin-shell

Bash pastebin.com client. Bash Script to post text from `stdin` to [pastebin.com](http://pastebin.com).

## Installation

Download:

	curl -f https://raw.githubusercontent.com/mefuckin/pastebin-shell/master/pbin -o pbin
	chmod +x pbin

Run:

	./pbin -h

## Usage

	Usage: pbin [options]
	Post text from stdin to pastebin.com.

	Options:
		-l				Log into pastebin.com
		-u				Your pastebin.com username
		-p				Your pastebin.com password
		-n name				Paste title
		-f format			Syntax highlightig format (you can find list 
						of formats at http://pastebin.com/api#5)
		-e expire			Paste expire time:
						  n (or never) - never
						  10M          - 10 minutes
						  1H           - 1 hour
						  1D           - 1 day
						  1M           - 1 month
		-r private			Private settings: public (or 0), unlisted (or 1)
						or private (or 2, need to login)
		-h				Show this message
		-o				Print sample config
		-c /path/to/pastebin.conf	Set path to config file

Examples:

`pbin < /proc/cpuinfo`


`echo -e "foo\nbar" | bash pbin -n "foobar.txt" -l 1`

## Requirements

Only `bash` and `curl`.
