# Timetable Extractor for VU Rooster

This bookmarklet allows you to extract the course schedule information from VU Amsterdam's legacy Rooster web app and export them in iCal format, appropriate for importing in ordinary calendar applications.

Please note that the code is under _beta test_, so use it at your risk.

Also note that due to a deficiency in the way [RFC 5545](https://icalendar.org/RFC-Specifications/iCalendar-RFC-5545/) and [RFC 7986](https://icalendar.org/RFC-Specifications/New-Properties-for-iCalendar-RFC-7986/) have been implemented in Microsoft Outlook, the current solution won't work properly on that platform. Subsequent developments will fix this issue.

## Installation
- Drag the following link into your bookmark bar: [VU🐓](javascript:(function()%7Bfunction%20callback()%7BparseTT()%7Dvar%20s%3Ddocument.createElement(%22script%22)%3Bs.src%3D%22https%3A%2F%2Fretrography.github.io%2FVUTt%2Fvutt.js%22%3Bif(s.addEventListener)%7Bs.addEventListener(%22load%22%2Ccallback%2Cfalse)%7Delse%20if(s.readyState)%7Bs.onreadystatechange%3Dcallback%7Ddocument.body.appendChild(s)%3B%7D)())

## Usage
- Go to [VU Rooster website](https://rooster.vu.nl/sws17181en) and find the schedule you would like to import
- Click the `VU🐓` bookmarklet in your bookmark bar

## Development
- Do not hesitate to [fork and improve](https://github.com/retrography/vurooster)
- Report bugs [here](https://github.com/retrography/vurooster/issues)

## Credits
- This work is inspired by [the great work of Anne Jon Schoonhoven](https://vurooster.nl/)
- The main idea of this bookmarklet came from [Georgios Andreadis](https://github.com/gandreadis/vu-timetable)

## Legal
- [MIT](https://spdx.org/licenses/MIT)-licensed

&copy; 2017 Mahmood S. Zargar  
