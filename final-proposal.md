---
title: Proposal
template: page
---

## 1.0 Project Scope

### 1.1 Tentative Project Title

**Inclusive Harvard**

### 1.2 Project Goals

One of Harvard's goals is to create a sense of inclusion and belonging for all members of the university community. As a four-year residential liberal arts college, Harvard is particularly attuned to the importance of daily interactions among students, faculty, staff, and their guests on campus. One particular effort has been providing and identifying private facilities to accommodate the needs of gender-nonconforming members of the community and nursing mothers.

"Inclusive Harvard" will be a web application that serves the needs of those two groups, who simply want to to go about their jobs, research projects, and studies without needing to be overly concerned about how their biological needs will be met. To accomplish that, the app will display the locations gender-neutral restrooms and lactation rooms on the user's device. It will offer street-level directions between buildings, and provide simplified interior floor plans to help users find their way around inside.

### 1.3 Learning Goals

There are several advanced web technologies that I will be using to build on my existing knowledge building applications with the MERN stack: MongoDB, Express, React, and NodeJS. Primarily, these are:

- **Progressive Web Apps (PWAs)** allow mobile users to "install" a website to their device and run it like any other application.
- **Mapping**, both in generating street directions with Open Street Maps and generating interior maps from CAD floor plans.
- **Browser/Device Location APIs** to get the users current location and correlate it with mapping data.
- **Accessibility Technology** to make sure that the app will work for people with visual or mobility impairments.
- **Code Splitting** to generate a smaller, faster applications by serving only the minimum code necessary.
- **Docker** to run the application and database as scalable microservices through Amazon Web Services.

This will also be an opportunity for me to develop my skills in user experience testing. I plan to make use of [Harvard Library's User Research Center][hlurc] for formalized testing, as well as conduct more informal testing with students, faculty, and staff.

From a more personal standpoint, I also want to learn more about Harvard's broader community, its ongoing efforts for diversity and inclusion, and how I can be a better ally in those efforts. I'm aware that as a straight white man I am outside the target audience of my own application, so I will need to communicate with and listen to people outside my regular peer group in order to make this successful.

### 1.4 Target Audience

#### Demographics

According the recently published report of the [Harvard University Presidential Task Force on Inclusion and Belonging][huptfib], there are about 50,000 students, faculty, and staff at Harvard. Of these, there are roughly equal numbers of people identifying as male and female--with about 0.6% identifying themselves as non-binary.

The two data sets that will be included in the app, gender-neutral restroom and lactation rooms, would imply that the target audiences are gender-nonconforming individuals and mothers, which would be a relatively small percentage of the overall Harvard population.

However, I do think the app could be useful to a some other audiences. For instance, gender-neutral restrooms can also benefit parents and caretakers who need to assist people of the opposite gender in the restroom. Harvard (and, by extension, Harvard Square) also hosts a wide range of guests on campus, from visiting students and faculty to tour groups and shoppers. As much of the university is publicly accessible, the app will also be freely available on the web to anyone on the web.

#### Persona 1: Alex

![Alex]({{"/assets/alex2.jpg" | absolute_url }})

_[Image by Greg Peverill-Conti](https://www.flickr.com/photos/gregpc/10806687066/)_

_"Back in Sweden, my friends and I always made jokes about Americans and their obsession with bathrooms... Now that's always in my mind whenever I'm looking for one here."_

**Profile:** Extension student on campus for the summer

**Gender**: nonconforming

**Age**: 23

**Current Location:** Harvard Square

**Hometown:** Gothenburg, Sweden

**Occupation:** Grad Student

**Motivations:** Alex is working on an ALM program through the extension school and will be fulfilling the on-campus requirement during the summer. Alex doesn't believe that gender should be treated as binary, and doesn't identify as male or female. Back at home in Sweden, Alex knows all the best places to find single-person and gender-neutral bathrooms. But all the news stories about debates in America over who is allowed to use which bathrooms have made Alex a little uneasy and concerned about what to do at Harvard.

**Goals:**

- Wants to enjoy Harvard and get the full campus experience
- Holds a strong conviction that gender is a societal construct and wants to live their own life.

**Frustrations:**

- News stories about "Bathroom Bills" and hate crimes in America make it seems like asking the wrong person can end badly.
- Even liberal Cambridge is more conservative than Sweden, and Alex doesn't want to be ostracized by classmates.

#### Persona 2: Beverly

![Beverly]({{"/assets/bevery2.jpg" | absolute_url}})

_[Image by Greg Peverill-Conti](https://www.flickr.com/photos/gregpc/14193274415/in/album-72157629602035180/)_

_"Even with no sleep I can deal with professors making outrageous last minute requests for extra funding, but trying to track down a lactation room M-112B in a building I've never seen before may be my breaking point."_

**Profile:** New mother

**Gender:** female

**Age:** 32

**Current Location:** Living in Framingham, Mass., working at Harvard

**Occupation:** Research Portfolio Manager at SEAS

**Motivations:** Beverly recently came back to work after the birth of her first child. She shares with two other admins, but fortunately there's a lactation room nearby office so she has regular access to a private space when she needs to pump. However, her job often requires her to a number of different labs and offices across different schools at the University, including across the river at the innovation lab and the Med School. Some days, Beverly never even makes it back to her own office. She doesn't want to let motherhood hold her back from doing her job, but also worries about getting stranded on the other side of campus and not knowing where to go when its time to pump.

**Goals:**

- Beverly prides herself on meeting all the needs of the faculty members that she assists.
- She's thinks that she's excellent at her job, and hopes to one day get promoted to Area Director.
- This is her first child, but she and her husband are hoping to continue growing their family.

**Frustrations:**

- An unexpected trip to the Medical School can send her away from campus for half the day or more.
- Even though she's read through the list of lactation rooms on the HR website, many of the old buildings at Harvard have unintuitive floor- and room-numbering schemes, making it harder to find the room she needs.
- Registering to use a lactation room requires her print, fill out, scan and email a form in advance.

### 1.5 Elevator Pitch

Everyone at Harvard should feel welcome within the University's walls; after all, it's not just a premiere academic institution, but also one of the state's largest employers. But even as Harvard has tried to make its students, faculty, and employees feel like they belong by, among other things, adding gender-neutral restrooms and lactation rooms around campus, sometimes Harvard itself can get in the way--crazy acronyms, multiple campuses, and different numbering schemes in every building. My app, "Inclusive Harvard", will try to cut back at least a little of that obscurity by providing simple, sensible direction to the gender-neutral restrooms or lactation rooms closest to the user.

### 1.6 Metrics

The primary metric I plan to track will simply be awareness of these facilities across the university. I am working on this as a pilot within the School of Engineering and Applied Sciences (SEAS), which recently undertook a Climate Survey to determine how members of the community feel about their own belonging on campus. Any change in awareness correlated with the app could be measured by conducting a similar follow-up survey after the app is released.

Given the somewhat private nature of the app, I'm hesitant to collect detailed statistics about when, where, and how the app is used--I certainly wouldn't want any user to feel that they were being followed into the bathroom. However, I do plan to collect anonymous statistics about how many times the app is loaded to help get a general sense of its rate of adoption, and to assist with scaling and load-balancing.

### 1.7 Life of the Project Beyond the Capstone

Inclusive Harvard will be publicly available online after the capstone, and I plan to release the core application code as an open source project on GitHub. One of my design goals is to make the code location-agnostic; it will rely on the underlying database to provide facility locations and floor plans data, so anyone will be able to use their own data to create a customized version of the app for any organization.

As mentioned above, this will initially be a pilot within SEAS. It will focus on three buildings at the core of the current SEAS campus: Maxwell-Dworkin, Pierce Hall, and Northwest. If the pilot is successful, there's the potential to include more buildings in the dataset, including two new SEAS buildings in Allston that are slated to open in 2020.

## 2.0 Competitor Review

### Competitor #1: Inclusive U

![UT-Austin's Inclusive U]({{ "/assets/utaiu.png" | absolute_url }})

A [web and mobile app][utaiu] mapping gender inclusive restrooms on the campus of the University of Texas at Austin.

**Market Share:** The University of Texas has over 50,000 undergraduates, and the city of Austin has around 1 million residents, so the potential market for this app is fairly large. Apple's app store doesn't list download numbers and Google Play no longer seems to carry the app, so it's hard to approximate the number of downloads.

**Tone of Language:** The app is presented by the [University's Gender & Sexuality Center][utaugsc], which has an overall tone that is positive and inclusive while taking it's subject matter seriously. It doesn't use playful language while discussing restrooms, and doesn't make any assumptions about its users.

**Key Differences:** Compared to the others, this is the most narrowly focused: Only gender-inclusive restrooms and only on the UT-Austin campus. In this way it is very similar to my app (and in fact was one of its inspirations). I think this narrow focus is a benefit, in that it's very easy to explain the app and its usefulness.

**Target Audience:** The copy on the Gender & Sexuality Center website specifically says that it serves "Women & LGBTA communities," and obviously it is aimed at people on the UT-Austin campus.

**User Response:** UT-Austin was ranked number 16 on a list of the [50 best colleges for LGBTQ Students](https://www.collegechoice.net/rankings/best-lgbt-friendly-colleges-and-universities/) with a specific mention of the work being done by the Gender & Sexuality Center. Harvard did not appear on the list.

**Competitor Goals:** The goals for this app are very closely aligned to those of my own app--making all students and visitors feel welcome on the UT campus by locating gender-neutral restrooms. The user goals are also very similar: wanting to get the typical college experience without needing to worry about things like finding an appropriate restroom.

**Data Accuracy:** Inclusive U appears to be relying on the University's own data about restroom locations on campus, and invites users to submit additions or corrections to the Gender & Sexuality Center. The website also has notes on many of the restrooms and photos stored on Google Drive. It is unclear how often this data is updated though.

### Competitor #2: Harvard Mobile

![Harvard Mobile Homepage]({{ "/assets/harvard_home.png" | absolute_url }}) ![Harvard Mobile map]({{ "/assets/harvard_map.png" | absolute_url }})

![Harvard Web Map]({{ "/assets/harvard_map_web.png" | absolute_url }})

Harvard's primary mobile app combines an interactive campus map, person directory, news and events listing, shuttle tracker, and other features that are useful for people on campus. Much of the information is similar to what can be found on the [main university site][hedu], and the campus map in particular can be found online at [https://map.harvard.edu/][hmap]

**Market Share:** The Harvard Community comprises about 50,000 people, including faculty, staff and students. The Harvard Mobile app has over 50,000 downloads on Google Play, dating back to around 2013, with similar number likely on the Apple app store, dating back to 2010. Given that the app is heavily promoted on campus, I suspect that more than half of the population on campus has downloaded it at one point or another.

**Tone of Language:** The overall app is very direct and to-the-point. In some of the news and informational sections it can be very booster-ish of the university, and maintains the overall air of academic prestige that the university's communications put forward.

**Key Differences:** This is sort of a "Swiss army knife" app for Harvard. It does a lot of things pretty well, though I suspect most people use it for one or two specific things. However, I know that I personally don't keep it on my phone because the features that I would need from it are better served by the school's website, or by other apps.

**Target Audience:** The app seems to primary target current students, with lists of course offerings, dining hall information, and shuttle bus schedules. There is also an admissions section, so there's likely some push for potential students. It doesn't seem particularly targeted at staff or faculty, which is one audience that I plan to include in my app.

**User Response:** Overall good reviews, with 4.4 stars out of 5 on Google Play (though several of those just say "nice" or "I like Harvard" so take that with a grain of salt). My anecdotal impression is that many people think the Harvard app is fine, but not essential.

**Competitor Goals:** I think that overall, this is a marketing app for Harvard and was originally released during the early smart phone days when it seemed like everyone needed to have an app. That said, the app's goal is to keep people up to date and informed about news and events at Harvard. I think, though, that most users are more interested in one or two things the app offers (like the shuttle schedule) and may not need all of this in one place.

**Data Accuracy:** This app also relies on official university data, especially around mapping. The online map in particular includes footprints of all the buildings and a number of additional data points. The map layers include features for things like accessibility, public safety, and bike facilities, but it does not include any overlay data about restrooms.

### Competitor #3: Sit or Squat

![Sit or Squat instructions]({{ "/assets/sos_overview.png" | absolute_url }}) ![Sit Or Squat Map]({{ "/assets/sos_map.png" | absolute_url }})

[Sit or Squat][sos] is a mobile app from Charmin that shows the locations of public restrooms near the user, with the ability to rank them on cleanliness as either Sit (clean enough to sit on the toilet) or Squat (when it's better to not).

**Market Share:** The app lists over 100,000 downloads on Google Play. Given that its bathroom database covers the US and few other countries, that implies a fairly small market share relative to its potential audience.

**Tone of Language:** As could be surmised from the name, the tone is very playful and jokey. It fits into the tone of Charmin's overall marketing strategy (slogan: "Enjoy the go!") and prominently features the company's cartoon bear mascots. It is also far more subjective, as it aims to rank bathrooms not just locate them.

**Key Differences:** This app covers a significantly larger area than either of the others, and as such it relies on users to contribute reviews and information about bathrooms. It also incorporates Facebook Connect to add a social element (signing in to add reviews and post pictures).

**Target Audience:** The marketing materials don't seem oriented toward any specific audience, but some of the reviews and testimonials specifically mention that it's great for parents with small children.

**User Response:** It has an overall rating of 3.9 stars out of 5 on Google Play, and 4.2 out of 5 on Apple. Many of the recent reviews are more negative, focusing on out-of-date data and issues with the connectivity. A review from Parenting Magazine on the Charmin website says that it is "one of the best apps for simplifying a parent's life."

**Competitor Goals:** Organizationally, this is marketing for Charmin by trying to make the brand synonymous with going to the bathroom and using the social side of the app to keep users connected. On the user side, most users are trying to find a bathroom near them, and would like to get a sense ahead of time whether it will be clean or not.

**Data Accuracy:** This is the only one that explicitly relies on user-contributed data, which may be why many of the recent reviews specifically cite out-of-date and faulty data as problems. It also provides a way to connect with Facebook. I don't think that's a good idea--even without the recent news about Facebook's data collection practices, I personally would not want to share information about when and where I use the bathroom, correlated with other personality traits, with a corporation like Charmin.

### Comparison with "Inclusive Harvard"

I think the biggest strength for my app is focus. Rather than try to solve every possible problem faced by every user on campus, the goal is to solve its particular problems as well as it can. In that way, it's probably closest to the Inclusive U app from Texas. But I intend to provide some additional functionality beyond what that app offers. The web version of Inclusive U, for instance, is only an annotated Google Map. I hope to be able to offer additional detail based on the specific location provided, and to do so with a mobile-friendly product.

That said, the opportunity I would most like to address is one to bring everyone closer into the community. I've been fortunate enough to work at Harvard for almost a decade, and in that time I've absorbed plenty of useful knowledge that I draw on every day. I think that the Charmin app tried to get people to share that kind of information, and they didn't; without a fall-back plan, the app has wilted. At the other end of the spectrum, the Harvard app has all kinds of official data, but it doesn't offer a true window in the community.

## 3.0 Technology Requirements

### Data

For navigation inside of buildings, I have obtained AutoCAD files for the three buildings in the initial pilot from the FAS planning office. Because private office locations are considered level 2 secure data, I will need to remove all non-public spaces from the plans (using LibreCAD, or another open-source CAD editor), then convert the files into SVG (scalable vector graphics) data and store it in MongoDB.

I also currently have Excel files with the locations of restrooms, and plain-text list of the locations for lactation rooms. All of that data will also be stored in MongoDB. Additionally, I may need to manually correlate those locations with latitude and longitude values for the maps

### Front End

I will be building a web-based application based on Google's [Progressive Web App][gpwa] (PWA) standards. Essentially, this means that the app will be able to function with or without a web connection and will feel more like a native mobile apps; it even offers the option to save the app to the user's home screen. I hope that this will bridge that gap between a web-only app and native mobile app by providing a reliable mobile experience for those who use the application on their phones.

The front-end code will be written in JavaScript, using the React framework. I will also be using either Google Maps or Open Street Maps for street-level navigation. I would prefer to use Open Street Maps as some users my be concerned about privacy with Google's maps, but ease-of-use will be the ultimate determining factor. I will be using D3.js or another graphics-manipulation library to render the SVG data for interiors.

In the interest of privacy, I plan to cache the user's destination locally and then do the location-based computations on the client-side. Ideally the user's location will never actually be sent to the server, so that users don't need to be concerned about their location being shared widely. This will also help ameliorate any issues with signal loss while moving around in doors.

While I have built a few applications in React already, this will be my first experience building a PWA. As such, I will need to do more research to figure out if there are other technical concerns I need to be aware of.

### Back End

The server for my app will be written in NodeJS and hosted through Amazon Web Services (AWS). I will use MongoDB to store the information about bathrooms and lactation room locations, along with the map data for all of the buildings. A document-based database like MongoDB makes sense for storing coordinates and polygon information for the building, as the schema for each object may be completely different.

The app will initially focus on just the primary SEAS campus, using data for Pierce Hall, Maxwell-Dworkin, and Northwest. However, I plan to set up the architecture such that expanding the number of buildings will only require adding the necessary building data to the database.

I would also like to use this capstone as an opportunity to experiment with running Docker containers in production. This would be a fairly small application, so I will likely only need server and database containers. This may be overkill, but starting with the scalability and flexibility of Docker will be helpful if the app is adopted more widely. As I continue with the proposal I will look for other services I can split off into their own containers.

The user documentation and any additional training materials will be created with the Gatsby static site generator, hosted in a separate GitHub repository and served from a sub-domain of the primary app.

## 4.0 Design Workflow

I want the app's interface to be simple and easy to navigate on a variety of devices. To accomplish that, I'm going to focus on two main interface modes: Map Mode, and List Mode. I do plan to start with with simple HTML mock-ups, or even pen and ink drawings, of the interface that I can use for informal testing before moving on to the true coding phase of development. I will probably start with a few of my co-workers as testers, and eventually bring in some real users within SEAS for more formalized testing in small groups (6-10 people). Toward the end of the project, I will consult the User Research Center about more in-depth accessibility training.

### Map Mode

Map mode will be the primary user interface, as many users are already familiar with that model for finding directions.

1.  The app will open to a typical street map view that will default to Harvard's campus.
2.  If the user allows the app to use the device location, the map will move to that location.
    - If the user does not allow location access, they will need to manually enter the location or scroll the map to find it.
3.  The user will be able to select which kind of facility (gender-neutral restroom or lactation room) they want to display.
    - These will be displayed as different symbols on the map
4.  If the user selects a building, the app will switch to an indoor floor plan mode showing where the facilities are located.

### List Mode

There will also be a separate list mode within the app that will show addresses/room numbers of nearby facilities. This will improve accessibility for users who are visually impaired, but can also be useful for those who are using the app to search and plan ahead.

1.  The app will still load into map mode initially.
2.  Once loaded, there will be a tab at the top of the screen to move over to the list view.
3.  List view will show the names and distances of all possible buildings, with an option to filter by type of facility.
4.  If the user shares their location data, the app will pre-select their current building.
    - The user can also scroll through a list of buildings that will show a count for the different types of facilities available.
5.  When a building is selected, the app will list all of those facilities.
6.  Once a facility is selected, the app will provide text directions (e.g. "third floor, room 325. Right-hand side of the hall.").

## 5.0 Work Plan and Milestones

### The Deliverables

- The open-source codebase for the app hosted on GitHub
- A running version of the application, public to the world
- User documentation
- Developer documentation
- Slide deck for training and outreach

### Milestones and Timelines

1.  Access to building floorplans
2.  Access to listing of all bathroom and lactation room locations
3.  Floorplans modified to meet Harvard Security guidelines
4.  Initial interface mockups in static html
5.  Design of database schema
6.  Functioning REST API for communication between database and client
7.  Successful connections between client and server
8.  App infrastructure provisioned on AWS
9.  App served at official domain.

### Rough Timeline

I will try to stay as close to the Agile methodology as possible, so all deadlines are based on roughly two-week increments, beginning September 1st, 2018.

**Before September 1st**: All data should be acquired or confirmed as available. May still need to be modified before use. (Milestones 1-3)

**Sept. 1 - Sept. 15**: Initial UI should be planned out and rendered. Begin informal user testing of UX. (Milestone 4)

**Sept. 15 - Oct. 1**: All data modifications complete; data loaded in MongoDB. (Milestone 5)

**Oct. 1 - Oct. 15**: REST API in place, with app configured to pull data from the server. (Milestones 6-7)

**Oct. 15 - Nov. 1**: Additional user testing of app interactions, formalized testing with User Research center. Make any additional changes necessary.

**Nov. 1 - Nov. 15**: Ensure app meets all PWA guidelines. Deploy server and database to AWS as Docker containers. (Milestone 8)

**Nov. 15 - Dec. 1**: Final configuration, testing, code cleanup. Write user documentation. Ensure data security standards have been met. Request SEAS domain name.

**Dec. 1 - Dec. 17**: Host application on AWS. Release code as open source library.

## 6.0 References

1.  Charmin SitOrSquat Bathroom Locator App. Retrieved from [https://www.charmin.com/en-us/about-us/sitorsquat][sos]

2.  Harvard IT Data Classification Table. Retrieved from [https://security.harvard.edu/dct][huitdct]

3.  Harvard Mobile App. Retrieved from [https://play.google.com/store/apps/details?id=edu.harvard.harvardmobile][happ]

4.  Inclusive U App from the University of Texas. Retrieved from [http://diversity.utexas.edu/genderandsexuality/gender-inclusive-restrooms/][utaiu]

5.  "Progressive Web Apps", Google. Retrieved from [https://developers.google.com/web/progressive-web-apps/][gpwa]

6.  "Pursuing Excellence on a Foundation of Inclusion," Report of the Harvard University Presidential Task Force on Inclusion and Belonging. Published March 27,2018. Retrieved from [https://inclusionandbelongingtaskforce.harvard.edu/final-report][huptifib]

7.  "Who’s Afraid of Gender-Neutral Bathrooms?" Jeannine Suk Gerson, The New Yorker. January 25, 2016. Retrieved from [https://www.newyorker.com/news/news-desk/whos-afraid-of-same-sex-bathrooms][nyrssb]

[huitdct]: https://security.harvard.edu/dct
[sos]: https://www.charmin.com/en-us/about-us/sitorsquat
[happ]: https://play.google.com/store/apps/details?id=edu.harvard.harvardmobile
[hmap]: https://map.harvard.edu
[hedu]: https://www.harvard.edu
[utaiu]: http://diversity.utexas.edu/genderandsexuality/gender-inclusive-restrooms/
[utaugsc]: http://diversity.utexas.edu/genderandsexuality/
[hlurc]: https://urc.library.harvard.edu/
[gpwa]: https://developers.google.com/web/progressive-web-apps/
[huptfib]: https://inclusionandbelongingtaskforce.harvard.edu/final-report
[nyrssb]: https://www.newyorker.com/news/news-desk/whos-afraid-of-same-sex-bathrooms
