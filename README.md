# DJS05: Show Detail Page with Routing and Navigation

## Project Overview

🎧 DJS05: Podcast Show Detail Page with Routing & Navigation
✅ What I Built
As part of the DJS05 module, I developed a dynamic podcast show detail page for a React-based podcast browsing application. This feature allows users to click on a show from the homepage or listing page and navigate to a dedicated page displaying all relevant details about that show.

I implemented dynamic routing using React Router, handled asynchronous data fetching based on show IDs, and built a responsive UI that gracefully manages loading, error, and empty states. I also ensured that search filters and pagination are preserved when users return to the homepage, creating a seamless browsing experience.

🧠 Key Features & Highlights
🔗 Dynamic Routing: Each show has its own unique URL, powered by route parameters.

📡 Data Fetching: Show details are fetched using the show ID from the URL, with robust handling of loading and error states.

🧭 Season Navigation: Users can expand/collapse seasons and browse episodes efficiently without excessive scrolling.

🧾 Episode Display: Each episode includes its number, title, image, and a shortened description for clarity.

🔍 State Preservation: Filters and search terms persist when navigating back to the homepage.

📱 Responsive Design: The layout adapts smoothly across mobile, tablet, and desktop devices.

🧼 Code Quality: All major functions are documented with JSDoc, and the codebase follows consistent formatting and modular structure.
![alt text](<Show Page Podcast.png>)

---

## Core Objectives

- Implement **dynamic routing** for unique show detail pages.
- Pass the correct show ID via route parameters and use it to **fetch specific show data**.
- Gracefully handle **loading, error, and empty states** during data fetching.
- Display comprehensive show details including title, image, description, genres, and last updated date.
- Preserve previous **filters and search state** when navigating back to the homepage.
- Create an intuitive **season navigation** UI to expand and switch between seasons without excessive scrolling.
- Display episode information clearly with numbering, titles, images, and shortened descriptions.
- Maintain **high code quality** with documentation (JSDoc) and consistent formatting.

---

### API Endpoints

Data can be called via a `fetch` request to the following three endpoints. Note that there is not always a one-to-one mapping between endpoints and actual data structures. Also note that **\*`<ID>`** indicates where the dynamic ID for the requested item should be placed. For example: `[https://podcast-api.netlify.app/genre/3](https://podcast-api.netlify.app/genre/3)`\*

| URL                                          |                                                                                        |
| -------------------------------------------- | -------------------------------------------------------------------------------------- |
| `https://podcast-api.netlify.app`            | Returns an array of PREVIEW                                                            |
| `https://podcast-api.netlify.app/genre/<ID>` | Returns a GENRE object                                                                 |
| `https://podcast-api.netlify.app/id/<ID>`    | Returns a SHOW object with several SEASON and EPISODE objects directly embedded within |

### Genre Titles

Since genre information is only exposed on `PREVIEW` by means of the specific `GENRE` id, it is recommended that you include the mapping between genre id values and title in your code itself:

| ID  | Title                    |
| --- | ------------------------ |
| 1   | Personal Growth          |
| 2   | Investigative Journalism |
| 3   | History                  |
| 4   | Comedy                   |
| 5   | Entertainment            |
| 6   | Business                 |
| 7   | Fiction                  |
| 8   | News                     |
| 9   | Kids and Family          |

## Deliverables

1. **Homepage / Listing Page**

   - List of shows with clickable links or buttons that navigate to each show's detail page.
   - Filters and search functionality that maintain state when navigating back from detail pages.

2. **Dynamic Show Detail Page**

   - A unique page for each show, accessible via a dynamic route.
   - Fetch and display show details including:
     - Title
     - Large podcast image
     - Description
     - Genre tags
     - Last updated date (formatted)
   - Display loading indicator while fetching data.
   - Display user-friendly error message if fetching fails.
   - Handle empty states gracefully (e.g., show not found).

3. **Season Navigation Component**

   - UI to expand/collapse seasons.
   - Show season title and episode count.
   - List episodes per season including:
     - Episode number
     - Episode title
     - Season image
     - Shortened episode description

4. **State Preservation**

   - Maintain applied filters and search terms when navigating back to the homepage from a show detail page.

5. **Code Quality**

   - Well-structured, modular React components.
   - JSDoc comments for all major functions and modules.
   - Consistent and readable formatting across all files.

6. **Responsive Design**

   - The UI adapts smoothly across different device sizes (mobile, tablet, desktop).

7. **README Documentation**
   - Brief project overview.
   - Instructions for running the project locally.
   - Description of main features and any known limitations.

---
