# BioMetaCalc

![Version](https://img.shields.io/badge/version-1.0-blue)
![License: AGPL v3](https://img.shields.io/badge/license-AGPL%20v3-blue.svg)
![Single file](https://img.shields.io/badge/single--file-HTML%2FCSS%2FJS-orange)
![Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)
![Language](https://img.shields.io/badge/UI-English-lightgrey)

**Live app: <https://tagtthespellcaster.github.io/BioMetaCalc/>**

BioMetaCalc is a single-file web application (HTML, CSS and JavaScript in one `index.html`) for body metrics, calorie needs, weight-loss planning, training logs and macronutrient calculation. It was originally a complex Excel workbook, rewritten as a self-contained web app. It runs entirely in the browser, needs no server, no installation and no external libraries, and works offline once loaded.

> The interface is in English. Food names are shown in English, and the original Italian names remain searchable.

## Features

| Section | What it does |
|---|---|
| **Overview dashboard** | Current weight, progress track from start to target, weight chart (actual vs. planned), key stats (BMI, body fat, energy need, forecast finish), energy balance, body composition, weekly walking distance, vitals and a list of items that need attention. |
| **Profile and composition** | BMI with category and healthy weight range; lean and fat mass with two methods (US Navy and Deurenberg); waist-to-hip ratio, ideal waist and waist to lose. |
| **Calorie needs** | Basal metabolic rate with four methods (weight-based, age-band table, Harris-Benedict, Mifflin-St Jeor); resting needs adjusted by lean mass; 24-hour activity schedule giving total daily energy expenditure. |
| **Goal and forecast** | Suggested daily intake for a target weight and date, with a warning below 1200 kcal/day; projected duration and end date for a chosen intake. |
| **Weight diary** | Day-by-day log with theoretical vs. actual weight, daily change, BMI and body fat estimate, notes, summary figures and an interactive chart. |
| **Walks** | Distance and steps log; estimated calories and fat use for walking and Nordic walking, with running totals. |
| **Blood pressure** | Morning and evening readings (systolic, diastolic, pulse) with averages. |
| **Runs** | Run log with pace and average speed; shoe mileage tracking. |
| **Heart rate** | Maximum heart rate (two formulas), resting heart rate, heart rate reserve, training zones and safe training ranges. |
| **Calorie expenditure** | Energy use for about 60 sports and activities by duration and body weight. |
| **Zone blocks** | Protein requirement and daily block distribution for the Zone-style diet. |
| **Meal calculator** | Calories, macronutrients, fibre, Zone blocks and points for any number of meals or days. |
| **Recipe calculator** | Totals and per-100 g values for recipes, built from the food database. |
| **Food table** | Searchable and sortable database of 846 foods (per 100 g) with English names and the original Italian names, plus custom foods. |

## Data and privacy

- All data stays in your browser (`localStorage`). Data saved by the earlier Italian version is migrated automatically. Nothing is sent to any server.
- Use **Export data** / **Import data** to back up or move your data as a JSON file. Clearing the browser's site data deletes it, so export regularly.
- **Reset to initial data** restores the sample data from the original workbook.

## Run locally

Download `index.html` and open it in any modern browser. No build step is required.

## Formulas and references

The calculations follow established published formulas, including:

- Body Mass Index (weight / height²)
- Harris-Benedict and Mifflin-St Jeor equations (basal metabolism)
- US Navy body fat method and the Deurenberg equation (body composition)
- Maximum heart rate estimates (220 − age; 208 − 0.7 × age) and the Karvonen reserve method

The implementation of every formula in the original workbook, and in this app, is original work. A conversion constant of 7000 kcal per kg of body weight is used for weight-loss forecasts.

## Disclaimer

BioMetaCalc provides estimates for informational purposes only. It is not a medical device and does not replace advice from a physician or registered dietitian. Very low calorie intakes can be harmful to health. Consult a professional before starting a diet or training programme.

*Zone®* is a registered trademark of its respective owner. It is mentioned only to describe the dietary method; this project is not affiliated with or endorsed by the trademark owner.

## License

BioMetaCalc is free software, released under the [GNU Affero General Public License v3.0](https://www.gnu.org/licenses/agpl-3.0.html) (AGPL-3.0). See the `LICENSE` file for the full text.
