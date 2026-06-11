# f1-tracking-poster

A print-ready F1 Season Tracker Poster coded using HTML, CSS, and JavaScript. Designed to be printed on a large format so you can manually write down race and sprint results with your family or friends throughout the season.

## ☰ Features & Design Elements

* **Complete 24-Race Calendar:** Includes accurate dates, locations, national flags, and circuit layouts for the entire 2026 season.
* **Dynamic Weekend Layouts:** The code automatically adjusts the tracking grid based on whether a round is a standard race or a **Sprint Weekend**.
* **Stat Tracking:** Dedicated write-in rows for:
  * Podium Finishers (**P1, P2, P3**)
  * **Pole Position** (indicated by the 1 icon)
  * **Fastest Lap** (indicated by the stopwatch icon and purple accent border)
  * **Driver of the Day** (indicated by the star icon)
* **Print-Optimized Styling:** The CSS configuration is set to handle high-resolution large-format printing layouts and can be edited before printing.

## 🛠️ Usage

1. **Download the Repository:** Clone or download the assets to your local machine. Ensure the `fonts/` and `circuits/` directories remain in the same relative path as `f1.html`.
2. **Open the File:** Open `f1.html` in any modern web browser.
3. **Print to Poster:** 
   * Press `Ctrl + P` (or `Cmd + P` on Mac) to bring up the print dialogue.
   * Set your destination to **Save as PDF** or send it directly to your printer.
   * Expand `More settings` and adjust `Margins` and set a custom `Scale` if needed. 
   * Ensure background graphics are enabled in your browser's print settings to preserve colors, borders, and gradients.
4. **Track the Season:** Hang it on your wall and write down the drivers' names or abbreviations after every race!

## ✏️ Editing for Future Seasons

You can easily repurpose this poster for future F1 seasons by opening the HTML file in a text editor and modifying the JavaScript script tag at the bottom:

1. **Update the Calendar:** Locate the `const races = [...]` array. You can add, remove, or reorder races here based on the updated official calendar. Simply update the round number (`r`), country name (`c`), country code (`fc` for flags), city location (`loc`), and dates (`d`) for each race card.
2. **Adjust Sprint Weekends:** Modify the `const sprintRounds = [...]` array. Just list the round numbers (e.g., `'02'`, `'06'`) that will host a Sprint shootout and race for that year, and the layout will dynamically adjust.
3. **Add New Track Graphics:** If a new circuit joins the calendar, drop its SVG map into the `circuits/` directory. Name the file following the established `[RoundNumber]_[Location].svg` format matching your array configuration (e.g., `circuits/01_Melbourne.svg`).

## ⚠️ Disclaimer

This is an unofficial fan project. This project is completely free, open-source, and non-commercial. Formula 1, F1, and related marks are trademarks of Formula One Licensing BV.