#TimelineSetter
- Full docs for ProPublica TimelineSetter can be found <a href="https://github.com/propublica/timeline-setter/" target="_blank">here</a>

###Setup
- Create a spreadsheet using <a href="https://docs.google.com/spreadsheet/ccc?key=0AowdnjGpuk-idElHNlozZERCNVY4dnhSUlNQa2p0SUE&usp=sharing" target="_blank">this template</a>
	- Make sure to use single instead of double quotes in HTML column
- Download spreadsheet as csv (Google will automatically append filename with " - sheetName" but the gem doesn't like spaces in the filename so make sure to fix that before running)

- Install TimelineSetter: `gem install timeline_setter`
- Run `timeline-setter -c /path/to/data.csv -o /path/to/output/directory`(if you omit `-o` it will assume current directory)
	- if you already have the a version of the template files use `-a` to prevent overwriting any customizations (maybe I'm doing it wrong but couldn't make that work - just make a copy of the altered CSS and keep that one on the server)

###ToDo
- Top priorities:
	1. Add chart above timeline
	2. Delete Monday dates from spreadsheet (and re-run script)
	2. <a href="http://propublica.github.io/timeline-setter/#interval_notch_options" target="_blank">Change interval notch defaults</a> so that timeline starts at 7 a.m. Tuesday to match up with the traffic data, if you can't figure it out ask John for traffic data starting at midnight Tuesday morning
	3. Add marker to chart to show corresponding timestamp to active timeline card
	4. Fix issue with embedded Tweets wiping out other data - or add the info to the html column, that seems to work for some reason

- Secondary:
	- mobile testing/optimizations
	- Cross-browser testing (I've only looked at it in Firefox on Mac)
	- If someone can incorporate the stills from the timelaps somehow that could be cool

##Notes
- Right now some of the photos are loading on the wrong side (when 960px or smaller), but if we start the timeline Tuesday morning instead of Monday that should fix the problem (for now)
