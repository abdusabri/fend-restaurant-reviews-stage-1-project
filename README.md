# Restaurant Reviews App - Stage 1

## Project Summary

This is the fifth project as part of my Front-End Web Development Nanodegree. The original code was provided, and the scope of this project was to make the website/app responsive, support accessibility (keyboard navigation, and screen readers), and add offline support. It is a simple restaurants reviews app, with an embedded map to show the locations of the restaurants.

## Technical Implementation Notes

- The app is fully usable with a keyboard, including the map and the markers on it (restaurant locations). Arrows can be used to pan the map

- I set the map to be focusable so that arrows can be easily used for panning

- I also set the restaurants list and the reviews element to be focusable, and that is to make it easy for users to use up and down arrows to scroll once focus is on them

- For caching and offline support, I've a progressive implementation, where i don't create chases upfront when the service worker is installed. The cache will incrementally grow to add the visited pages and requested resources

- Leaflet version 1.3.1 is used ([link](https://unpkg.com/leaflet@1.3.1/dist/leaflet.js))

- [Mapbox](https://www.mapbox.com/) and [OpenStreetMap](https://www.openstreetmap.org/) are also used

- Besides Leaflet, no other frameworks or libraries are used

- The app doesn't use server-side code

- To run the application locally, clone the repo, or download a zipped version, then unzip it. After that, you need to host the application on a web server, and then navigate to the root directory (for example, `localhost:3000`)

- Any simple python or NodeJs-based webserver would be enough

## References and Credits

Following are some articles, links, and tools that were very helpful for me while completing the project work:

- Leaflet map accessibility and tab handling:

  - [Tabbing through leaflet markers breaks the map](https://github.com/Leaflet/Leaflet/issues/3385)
  - [Accessibility improvements](https://github.com/Leaflet/Leaflet/issues/3210)
  - [Another discussion on accessibility](https://github.com/Leaflet/Leaflet/issues/3472)

- [Web Accessibility Checklist](https://a11yproject.com/checklist)

- [Nu Html Checker](https://validator.w3.org/nu/#textarea)

- [Quick tip: Using alt text properly](https://a11yproject.com/posts/alt-text/)

- [Service Workers: an Introduction](https://developers.google.com/web/fundamentals/primers/service-workers/)
