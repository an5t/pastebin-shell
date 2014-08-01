pastebin-shell
==============

bash pastebin.com client
Posts text from stdin to pastebin.com.

Usage: pbin [options]

Options:
   -n name	Paste title
   -f format	Syntax highlightig format (you can find list 
		   of formats at http://pastebin.com/api#5)
   -e expire	Paste expire time:
		  n (or never) - never
		  10M - 10 minutes
		   1H - 1 hour
		   1D - 1 day
		   1M - 1 month
   -r private	Private settings: public (or 0), unlisted (or 1)
		   or private (or 2, need to login)
   -l		Log into pastebin.com
   -u		Your pastebin.com username
   -p		Your pastebin.com password
   -h		Show this message
   -o		Print sample config
   -c /path/to/pastebin.conf	Set path to config file
