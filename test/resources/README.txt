CSV files creation

- utf8.csv
	Created using Gnumeric, by copying strings containing non-ASCII character from a real CSV file provided by our client.

- windows1252.csv
	iconv -f UTF-8 -t WINDOWS-1252 utf8.csv > windows1252.csv

- macintosh.csv
	iconv -f UTF-8 -t MACINTOSH utf8.csv > macintosh.csv

- mixed-utf8-windows1252.csv
	cat utf8.csv windows1252.csv > mixed-utf8-windows1252.csv

- mixed-utf8-macintosh.csv
	cat utf8.csv macintosh.csv > mixed-utf8-macintosh.csv
