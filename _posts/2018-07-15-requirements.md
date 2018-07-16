---
title: Requirements
---

My elevator pitch for reference:

> Everyone at Harvard should feel welcome within the University’s walls. It’s not just a premiere academic institution, but also one of the state’s largest employers. But even as Harvard has tried to make its students, faculty, and employees feel like they belong by, among other things, adding gender-neutral restrooms and lactation rooms around campus, sometimes Harvard itself can get in the way–crazy acronyms, multiple campuses, and different numbering schemes in every building. My app, “Inclusive Harvard”, will try to cut back at least a little of that obscurity by providing simple, sensible direction to the gender-neutral restrooms or lactation rooms closest to the user. 

## How does it work?

### Map Mode

Map mode will be the primary user interface, as many users are already familiar with that model for finding directions.

1. The app will open to a typical street map view that will default to Harvard's campus. 
2. If the user allows the app to use the device location, the map will move there.
    - If the user does not allow location access, they will need to manually enter the location or scroll the map to find it.
3. The user will be able to select which kind of facility (gender-neutral restroom or lactation room) they want to display.
    - These will be displayed as different symbols on the map
4. If the user selects a building, the app will switch to an indoor floor plan mode showing where the facilities are located.

### List Mode

There will also be a separate list mode within the app that will show addresses/room numbers of nearby facilities. This will improve accessibility for users who are visually impaired, but can also be useful for those who are using the app to search and plan ahead. 

1. The app will still load into map mode initially.
2. Once loaded, there will be a tab at the top of the screen to move over to the list view.
3. List view will show the names and distances of all possible building, with an option to filter by type of facility.
4. If the user shares their location data, the app will pre-select their current building.
    - The user can also scroll through a list of buildings that will show a count for the different types of facilities available.
5. When a building is selected, the app will list all of those facilities.
6. Once a facility is selected, the app will provide text directions (e.g. "third floor, room 325. Right-hand side of the hall."). 


## The Tech

### Front End

My initial target is to build a web-based application, based on Google's [Progressive Web App](https://developers.google.com/web/progressive-web-apps/) (PWA) standards. I hope that this will bridge that gap between a web-only app and native mobile app by providing a reliable mobile experience for those who use the application on their phones. 

The front-end code will be written in JavaScript, using the React framework. I will also be using either Google Maps or Open Street Maps for street-level navigation. I would prefer to use Open Street Maps as some users my be concerned about privacy with Google's maps, but ease-of-use will be the ultimate determining factor. 

I have not yet chosen a library for navigation within buildings. I'm currently looking into available floor plan data now and will decide what makes sense based on which formats are available. I suspect that the answer will use some kind of CAD-to-SVG translation for rendering floor plans in an HTML canvas element.

In the interest of privacy, I plan to cache the user's destination locally and then do most of the location-based computations on the client-side. Ideally the user's location will never actually be sent to the server, so that users don't need to be concerned about their location being shared widely. This will also help ameliorate any issues with signal loss while moving around in doors. 

While I have built a few applications in React already, this will be my first experience building a PWA. As such, I will need to do more research to figure out if there are other technical concerns I need to be aware of.

### Back End

The server for my app will be written in NodeJS and hosted through Amazon Web Services (AWS). I will use MongoDB to store the information about bathrooms and lactation room locations, along with the map data for all of the buildings. A document-based database like MongoDB makes sense for storing coordinates and polygon information for the building, as the schema for each object may be completely different. 

The app will initially focus on just the primary SEAS campus, using data for Pierce Hall, Maxwell-Dworkin, and Northwest. However, I plan to set up the architecture such that expanding the number of buildings will only require adding the necessary building data to the database.

I would also like to use this capstone as an opportunity to experiment with running Docker containers in production. This would be a fairly small application, so I will likely only need server and database containers. This may be overkill, but starting with the scalability and flexibility of Docker will be helpful if the app is adopted more widely. As I continue with the proposal I will look for other services I can split off into their own containers.

The user documentation and any additional training materials will be created with the Gatsby static site generator, hosted in a separate GitHub repository and served from a sub-domain of the primary app. 

## The Deliverables

- The open-source codebase for the app hosted on GitHub
- A running version of the application, public to the world
- User documentation
- Developer documentation
- Slide deck for training and outreach
