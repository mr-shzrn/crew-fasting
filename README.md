# crew-fasting
# Pilot Fasting Tool (JAKIM Standard)

## Overview
This tool calculates the start (Sahur) and end (Iftar) of fasting based on **visual reality at altitude**, complying with Malaysian (JAKIM) standards.

### Key Features
* **Live Mode:** Uses iPad GPS for real-time status.
* **Manual Mode:** Allows input of Flight Plan data (Speed/Track).
* **Prediction:** Estimates Iftar/Sahur times for the next 2 hours.

## How to Use

### 1. GPS Mode (Default)
* **Best for:** Cruising with good satellite reception.
* **Action:** Open the app. Allow Location Services.
* **Note:** If the "GPS" indicator is Red, move the iPad closer to a side window.

### 2. Manual Mode (Backup)
* **Best for:** Pre-flight planning or if GPS is unavailable.
* **Input Format:** You can type coordinates exactly as seen on the FMC.
    * *Example:* `N03 15.4` or `3 15.4` (Space separated).
    * *Example:* `S 22 10.0` (South is handled automatically).

### 3. Prediction Tool
Calculates when the sun will set/rise based on your current path.
* **Mins to Turn:** Enter how many minutes until your next waypoint. The app will stop looking beyond this time to avoid false predictions.
* **Vertical Speed (VS):** * Enter `-1500` if descending. 
    * *Crucial:* Descending makes the sun set faster! Always input your VS during top-of-descent.

## Troubleshooting
* **"Waiting for GPS":** Switch to Manual Mode and enter coordinates from the ND.
* **Screen Sleep:** Keep the app open on screen; backgrounding it may stop the timer.

## Technical Data
* **Fajr Angle:** 20.0° (JAKIM).
* **Sunset Angle:** 0.833° + Dip of Horizon.
* **Safety Buffer:** +/- 2 minutes added to all calculations.
