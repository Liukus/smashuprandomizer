# Smash Up Randomizer <img height=100% src=favicon.ico>

A web-based and mobile-friendly application designed to streamline the faction drafting process for the popular card game, **Smash Up!** This tool helps players quickly and fairly select their two factions for a game, offering multiple draft modes to suit different playstyles.

## ✨ Features

* **Player Setup:** Easily set up 2, 3, or 4 players and customize their names.

* **Dynamic Faction Selection:**
    * Select which Smash Up! sets you own and want to include in the draft pool.
    * Granular control to include or exclude individual factions from chosen sets.
    * **Custom Factions Support:** Toggle to include or exclude custom factions (if available from the data source).
    * Visual indicators for partially selected sets (indeterminate checkboxes).
    * "Select All" and "Select None" options for quick configuration.
    * Displays the total number of factions available and a summary of excluded factions with a detailed tooltip.

* **Multiple Draft Modes:**
    * **Snake Draft:** Players take turns picking one faction from a presented choice, following a snake draft order.
        * **Customizable Choices:** Configure how many factions are presented (e.g., "Pick 1 of 2", "Pick 1 of 5", or "Pick 1 of All").
        * **Unchosen Faction Handling:** Choose whether unchosen factions are removed from play or re-integrated into the pool.
        * **Random Subset:** Create a draft pool from a random subset of your selected factions.
        * **Official : Custom Ratio:** When using a random subset, specify a ratio for official vs. custom factions (e.g., 1:1, 3:1).
        * **Filter Options:** Filter factions by name when presenting "all" factions for selection.
    * **Pick 2 of X:** Each player is presented with 'X' random factions and chooses two to keep.
        * **Customizable 'X':** Define how many factions are presented (e.g., "Pick 2 of 4", "Pick 2 of 6").
        * **Unchosen Faction Handling:** Choose whether unchosen factions are removed from play or re-integrated into the pool.
    * **Discard 1 of 3:** Each player is dealt three random factions and chooses one to discard, keeping the remaining two.
    * **Pure Random Assignment:** Factions are randomly assigned to players without any player interaction.

* **Interactive Draft Process:**
    * Clear indication of the current player's turn and pick number.
    * Visual feedback during faction selection/discard.
    * **Undo Last Pick:** Revert the last draft action, allowing for corrections or re-thinking.

* **Draft History:** A detailed log of all picks and discards throughout the draft.

* **Persistent Settings:** Your selected sets, custom faction toggle state, player names, and draft mode options are saved locally in your browser, so your preferences are remembered for your next session.

* **View Last Draft Results:** Re-open the modal to review the results of the most recently completed draft.

* **Comprehensive Reset:** The "Reset All" button now clears all saved preferences, resets all settings to their defaults (including faction selections and custom faction toggle), and prepares the app for a completely fresh start.

* **Responsive Design:** Optimized for a seamless experience across desktop, tablet, and mobile devices.

## 🚀 How to Use

1.  **Access the App:**
    * **Web:** Visit the deployed application [here](https://liukus.github.io/smashuprandomizer/).
    * **Mobile (Hybrid App):** (Coming Soon, I hope)

2.  **Player Setup:**
    * Choose the number of players (2, 3, or 4) using the buttons.
    * Enter custom names for each player in the text fields. If left blank, default names like "Player 1" will be used.

3.  **Select Sets & Factions:**
    * Browse through the list of Smash Up! sets.
    * **To include/exclude an entire set:** Click the checkbox next to the set name.
        * A fully checked box means all factions in that set are included.
        * An indeterminate box (partially filled) means some, but not all, factions from that set are included.
        * An unchecked box means no factions from that set are included.
    * **To include/exclude individual factions:** Click on a set's name to expand it and reveal the factions within. Then, check/uncheck individual faction checkboxes.
    * Use the "Select All" button to quickly include all active sets and factions.
    * Use the "Select None" button to quickly clear all selections.
    * **Custom Factions Toggle:** Use the "Custom Factions" switch to include or exclude custom factions from your available pool. By default all custom factions selected.
    * The app will display the total number of factions available for the draft and how many are excluded. Hover over "Factions excluded" for a detailed list.

4.  **Choose Mode:**
    * Select your preferred draft method:
        * **Snake Draft:**
            * Choose the "Number of factions presented (1 of X)" from the dropdown. Selecting "All" will show all available factions.
            * Decide how "Unchosen factions" are handled: "Remove from Play" (they won't be picked again) or "Re-integrate into Pool" (they can be drawn again).
            * **Use Random Subset for Draft Pool:** Check this to create a smaller, randomized pool. Enter the "Desired Subset Size".
            * **Use Official : Custom Faction Ratio:** If "Use Random Subset" is active, check this to enforce a ratio between official and custom factions in the subset (e.g., "3:5")
                * This option requires Random Subset to be picked to display. Your total draft pool will be seeded based on your ratio and will total the number selected for the random subset.
        * **Pick 2 of X:**
            * Choose the "Number of factions presented (2 of X)" from the dropdown.
            * Decide how "Unchosen factions" are handled: "Remove from Play" or "Re-integrate into Pool".
        * **Discard 1 of 3:** For a quicker draft where players discard one unwanted faction from three.
        * **Pure Random Assignment:** For an instant, completely random setup.

5.  **Start Draft:**
    * Click the "Begin Draft" button to start the process.
    * If you don't have enough factions selected for the chosen mode and player count, a warning message will appear.
    * A modal will appear showing the draft progress:
        * In interactive modes, the current player will be prompted to make their choice.
        * The "Draft History" section will log each action.
    * **Undo Last Pick:** During an active draft (except Pure Random Assignment), click "Undo Last Pick" to revert the most recent selection or discard.
    * Once the draft is complete, the modal will display the final faction assignments for each player.
    * Click "Close" to dismiss the modal.
    * **View Last Draft Results:** Click this button to re-open the modal and review the details of your previous completed draft.
    * **Reset All:** Click this button to clear all player names, draft history, reset all draft settings to their default values, and deselect all factions (including turning off the Custom Factions toggle). This provides a complete fresh start.

## 🛠️ Technologies Used

* **React:** Frontend JavaScript library for building user interfaces.
* **Tailwind CSS:** A utility-first CSS framework for rapid styling.
* **Material-UI (MUI):** Used for the `TextField` component, integrated with a custom dark theme.
* **Capacitor:** (For future mobile app deployment) A cross-platform native runtime for web apps.

## 🙏 Support

If you find this app useful and would like to support its development, you can buy me a coffee!

[![Buy Me A Coffee at ko-fi.com](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/liukus)

## 📄 License

This project is open-source and available under the [GNU GPLv3 License](LICENSE).
