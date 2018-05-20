# DataAnalysis_NOAA

Download	“co2_hawaii.txt”	and	 “co2_alaska.txt”.		These	files	are	from	the	U.S.	National	Oceanic	and	Atmospheric	Administration	
(NOAA).		They	contain	over	40	years	of	measurements	of	carbon	dioxide	levels	(CO2)	in	the	
atmosphere,	taken	from	instruments	at	Barrow,	Alaska	and	Mauna	Loa,	Hawaii.

Write	a	program	to	automatically	perform the	following data	processing steps:

1. Read	the	unmodified	files and	load all	the	data values	into	some	kind	of	appropriate	array,	
matrix, or	similar	data	structure(s).

2. Parse	the	Quality	Control	Flags to	know	which	rows	have	invalid	data	that	must	be	ignored	in	
calculations.	Typically,	you’ll	see	“-999.99”	in	place	of	the	co2	value,	but	there	may	be	other	
kinds	of	invalid	rows,	so	determine	validity	from	the	“qcflag” column	only.

3. Calculate	the	following	items	PER	YEAR,	and	output	a	new	text	file called	“annual_co2.txt”
containing	a table	with	year	down	the	side	and	each	column	heading	indicated,	for	both	
locations.:
a. “MAX_LEVEL”:		The	highest CO2 daily	level	recorded.
b. “MEAN_LEVEL”:		The	mean	(average)	of daily	CO2 levels recorded.
c. “%CHANGE”:	Percentage	change	of	“Mean	level”	compared	to	previous	year.	
Arrange the	output	data	like	this,	and	round	the	mean	CO2	values to	2	decimal	places:
ALASKA HAWAII
YEAR MAX_LEVEL MEAN_LEVEL %CHANGE MAX_LEVEL MEAN_LEVEL %CHANGE
1973
1974
1975
…
2015
2016

4. Then	have	the	program	calculate	the	mean	of	the	annual	“%CHANGE” results	for	each	location,	
and	add	those	results	below	the	table.
