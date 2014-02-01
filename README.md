#TimelineSetter
- Full docs for ProPublica TimelineSetter can be found <a href="https://github.com/propublica/timeline-setter/" target="_blank">here</a>

###Setup
- Create a spreadsheet using <a href="https://docs.google.com/spreadsheet/ccc?key=0AowdnjGpuk-idElHNlozZERCNVY4dnhSUlNQa2p0SUE&usp=sharing" target="_blank">this template</a>
- Download spreadsheet as csv (Google will automatically append filename with " - sheetName" but the gem doesn't like spaces in the filename so make sure to fix that before running the script)

- Install TimelineSetter: `gem install timeline_setter`
- Run `timeline-setter -c /path/to/data.csv -o /path/to/output/directory`(if you omit `-o` it will assume current directory)

###ToDo
- Increase min-width of cards on desktop screens
- Set min-width of Twitter card width for mobile
- Add photos
- Fix issue with embedded Tweets wiping out other data
- Add chart above timeline
- <a href="http://propublica.github.io/timeline-setter/#interval_notch_options" target="_blank">Change interval notch defaults</a> so that timeline starts at 7 a.m. Tuesday to match up with the traffic data
- Add marker to chart to show corresponding timestamp to active timeline card
- Cross-browser testing (I've only looked at it in Firefox on Mac)
- If someone can incorporate the stills from the timelaps somehow that could be cool

