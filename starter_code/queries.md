![Ironhack Logo](https://i.imgur.com/1QgrNNw.png)

# Answers

### 1. All the companies whose name match 'Babelgum'. Retrieve only their `name` field.

_id:52cdef7c4bab8bd675297da0
name:"Babelgum"

### 2. All the companies that have more than 5000 employees. Limit the search to 20 companies and sort them by **number of employees**.

_id:52cdef7c4bab8bd675297d8e
name:"Facebook"
_id:52cdef7c4bab8bd675297d9b
name:"eBay"
_id:52cdef7c4bab8bd675297da2
name:"Cisco"
_id:52cdef7c4bab8bd675297dc4
name:"Intel"
_id:52cdef7c4bab8bd675297da3
name:"Yahoo!"
_id:52cdef7c4bab8bd675297e49
name:"Nintendo"
_id:52cdef7c4bab8bd675297dba
name:"Google"
_id:52cdef7c4bab8bd675297e6f
name:"Sony"
_id:52cdef7c4bab8bd675297e5d
name:"Adobe Systems"
_id:52cdef7c4bab8bd675297e89
name:"PayPal"
_id:52cdef7c4bab8bd675297e8e
name:"The Walt Disney Company"
_id:52cdef7c4bab8bd675297ea4
name:"Webkinz"
_id:52cdef7c4bab8bd675297e96
name:"AOL"
_id:52cdef7c4bab8bd675297ee9
name:"Sun Microsystems"
_id:52cdef7c4bab8bd675297fcb
name:"Rakuten"
_id:52cdef7c4bab8bd675297fc2
name:"Nokia"
_id:52cdef7c4bab8bd67529809d
name:"Microsoft"
_id:52cdef7c4bab8bd675298189
name:"Apple"
_id:52cdef7c4bab8bd6752981b5
name:"NetApp"
_id:52cdef7c4bab8bd67529821b
name:"Motorola Solutions"

### 3. All the companies founded between 2000 and 2005, both years included. Retrieve only the `name` and `founded_year` fields.

name:"Zoho"
founded_year:2005
name:"Omnidrive"
founded_year:2005
name:"Wetpaint"
founded_year:2005
name:"StumbleUpon"
founded_year:2002
name:"Gizmoz"
founded_year:2003
name:"Helio"
founded_year:2005
name:"Digg"
founded_year:2004
name:"Technorati"
founded_year:2002
name:"Plaxo"
founded_year:2002
name:"Facebook"
founded_year:2004
name:"AddThis"
founded_year:2004
name:"Veoh"
founded_year:2004
name:"Wesabe"
founded_year:2005
name:"SmugMug"
founded_year:2002
name:"Jingle Networks"
founded_year:2005
name:"Meetup"
founded_year:2002
name:"LifeLock"
founded_year:2005
name:"Jangl SMS"
founded_year:2005
name:"Jajah"
founded_year:2005
name:"YouTube"
founded_year:2005

### 4. All the companies that had a Valuation Amount of more than 100.000.000 and have been founded before 2010. Retrieve only the `name` and `ipo` fields.

name:"Facebook"
name:"Twitter"
name:"Yelp"
name:"LinkedIn"
name:"Brightcove"
name:"Amazon"
name:"KIT digital"
name:"Nielsen"
name:"OpenTable"
name:"ChannelAdvisor"
name:"Jive Software"
name:"Zillow"
name:"Wix"
name:"Shutterfly"
name:"TripAdvisor"
name:"Salesforce"
name:"HomeAway"
name:"QuinStreet"
name:"Rackspace"
name:"BMC Software"


### 5. All the companies that have less than 1000 employees and have been founded before 2005. Order them by the number of employees and limit the search to 10 companies.
{$and: [{number_of_employees: {$lte: 1000}},{founded_year: {$lt: 2005}}]}

name:"Fox Interactive Media"
name:"Skype"
name:"Ticketmaster"
name:"stylediary"
name:"MindTouch"
name:"Simpy"
name:"Eurekster"
name:"Compete"
name:"EditGrid"
name:"Monster"

### 6. All the companies that don't include the `partners` field.
{$where: 'this.partners.length === 0'}

name:"AdventNet"
name:"Zoho"
name:"Omnidrive"
name:"Wetpaint"
name:"Geni"
name:"Postini"
name:"Scribd"
name:"StumbleUpon"
name:"Gizmoz"
name:"Slacker"
name:"Lala"
name:"Helio"
name:"MeetMoi"
name:"Joost"
name:"Viacom"
name:"CBS"
name:"Babelgum"
name:"Flektor"
name:"Digg"
name:"Fox Interactive Media"

### 7. All the companies that have a null type of value on the `category_code` field.
{$where: 'this.category_code === null'}

name:"Collective"
name:"Snimmer"
name:"KoolIM"
name:"Level9 Media"
name:"VidKing"
name:"Drigg"
name:"SpaceTime"
name:"Inside Group"
name:"Repeater Store"
name:"MMDAYS"
name:"Touch Clarity"
name:"Tapesh"
name:"iPersians"
name:"NewPersia"
name:"Pyra Labs"
name:"Feedmap"
name:"NuvoMedia"
name:"Intwine"
name:"The Weinstein Company"
name:"ExecuNet"

### 8. All the companies that have at least 100 employees but less than 1000. Retrieve only the `name` and `number of employees` fields.
{$and: [{number_of_employees: {$gte: 100}},{number_of_employees: {$lt: 1000}}]}

name:"AdventNet"
number_of_employees:600
name:"AddThis"
number_of_employees:120
name:"OpenX"
number_of_employees:305
name:"LifeLock"
number_of_employees:644
name:"Jajah"
number_of_employees:110
name:"Livestream"
number_of_employees:120
name:"Ustream"
number_of_employees:250
name:"iContact"
number_of_employees:300
name:"Yelp"
number_of_employees:800
name:"Dailymotion"
number_of_employees:120
name:"RockYou"
number_of_employees:106
name:"Meebo"
number_of_employees:200
name:"Eventbrite"
number_of_employees:200
name:"Box"
number_of_employees:950
name:"Conduit"
number_of_employees:215
name:"Redfin"
number_of_employees:100
name:"Simply Hired"
number_of_employees:100
name:"oDesk"
number_of_employees:120
name:"Spreadshirt"
number_of_employees:230
name:"PhotoBox"
number_of_employees:600




### 9. Order all the companies by their IPO price in a descending order.

name:"GREE"
name:"Facebook"
name:"Amazon"
name:"Twitter"
name:"Groupon"
name:"Tencent"
name:"Western Digital"
name:"LinkedIn"
name:"BMC Software"
name:"Rackspace"
name:"Baidu"
name:"TripAdvisor"
name:"HomeAway"
name:"Zillow"
name:"Nielsen"
name:"Yelp"
name:"Chegg"
name:"Chegg"
name:"RPX Corporation"
name:"Higher One"


### 10. Retrieve the 10 companies with more employees, order by the `number of employees`
name:"Siemens"
name:"IBM"
name:"Toyota"
name:"PayPal"
name:"Nippon Telegraph and Telephone Corporation"
name:"Samsung Electronics"
name:"Accenture"
name:"Tata Consultancy Services"
name:"Flextronics International"
name:"Safeway"
name:"Sony"
name:"LG"
name:"Ford"
name:"Boeing"
name:"Digital Equipment Corporation"
name:"Nokia"
name:"MItsubishi Electric"
name:"MItsubishi Electric"
name:"Comcast"
name:"Bertelsmann"

### 11. All the companies founded on the second semester of the year. Limit your search to 1000 companies.

<!-- Your Code Goes Here -->

<!-- ### 12. All the companies that have been 'deadpooled' after the third year. -->

<!-- Your Code Goes Here -->

### 12. All the companies founded before 2000 that have an acquisition amount of more than 10.000.000

<!-- Your Code Goes Here -->

### 13. All the companies that have been acquired after 2010, order by the acquisition amount, and retrieve only their `name` and `acquisition` field.

<!-- Your Code Goes Here -->

### 14. Order the companies by their `founded year`, retrieving only their `name` and `founded year`.

<!-- Your Code Goes Here -->

### 15. All the companies that have been founded on the first seven days of the month, including the seventh. Sort them by their `acquisition price` in a descending order. Limit the search to 10 documents.

<!-- Your Code Goes Here -->

### 16. All the companies on the 'web' `category` that have more than 4000 employees. Sort them by the amount of employees in ascending order.

<!-- Your Code Goes Here -->

### 17. All the companies whose acquisition amount is more than 10.000.000, and currency is 'EUR'.

<!-- Your Code Goes Here -->

### 18. All the companies that have been acquired on the first trimester of the year. Limit the search to 10 companies, and retrieve only their `name` and `acquisition` fields.

<!-- Your Code Goes Here -->

### 19. All the companies that have been founded between 2000 and 2010, but have not been acquired before 2011.

<!-- Your Code Goes Here -->
