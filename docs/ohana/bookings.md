# Page Bookings

Return to: [[Index]]

---

## List View

**Dashboard View**
| Date       | Day        | Time    | Length | City           | State |
| ---------- | ---------- | ------- | ------ | -------------- | ----- |
| `Feb 23`   | tomorrow   | 7:00PM  | 45     | Baltimore      | MD    |
| `Mar 5`    | Friday     | 5:45PM  | 60     | Virginia Beach | VA    |
| `Mar 6`    | Saturday   | 11:30AM | 60     | Gaithersburg   | MD    |
| `Apr 14`   | Saturday   | 9:00PM  | 45     | Manassas       | VA    |
| `May 1`    | Sunday     | 3:30PM  | 30     | Washington     | DC    |

---
**Bookings View**
| Date       | Day        | Time    | Length | City           | State | Dancers   | Client
| ---------- | ---------- | ------- | ------ | -------------- | ----- | --------- | -------
| `Feb 23`   | tomorrow   | 7:00PM  | 45 min | Baltimore      | MD    | 2/2       | Jennifer Johnson
| `Mar 5`    | Friday     | 5:45PM  | 60 min | Virginia Beach | VA    | 5/5       | Christopher Stephens
| `Mar 6`    | Saturday   | 11:30AM | 60 min | Gaithersburg   | MD    | 3/3       | Georgetown University
| `Apr 14`   | Saturday   | 9:00PM  | 45 min | Manassas       | VA    | `2/3`     | Vanessa Valentino
| `May 1`    | Sunday     | 3:30PM  | 30 min | Washington     | DC    | `0/2`     | John Hopkins

---
Sort By: 
- Date
- City
- State
- Dancers
- Client

Filter By:
- Date Range 
- Day (multi-select)
- City (typeahead multi-select)
- State (typeahead multi-select)
- Client Name (typeahead multi-select)

Search By:
- Dates: Abbrev., mm-Month/dd/yy-yyyy
- Day
- City
- State
- Dancer count
- Client Name
## Show Details

```json
{
  "date": new ISODate("2010-09-24"),
  "startTime": new Timestamp(),
  "callTime": new Timestamp(),
  "lengthOfService": 60,
  "location": { 
    "street": "123 street",
    "city": "cityName",
    "state": "stateName",
    "zip": "22123",
  },
  "client": {
    "firstName": "clientFirstName",
    "lastName": "clientLastName"
  },
  "dancers": ["dancer1", "dancer2"],
}
```
