# Smash Up Randomizer <img height=100% src=favicon.ico>

 A web-based and mobile-friendly application designed to streamline the faction drafting process for the popular card game, **Smash Up!** This tool helps players quickly and fairly select their two factions for a game, offering multiple draft modes to suit different playstyles.

## ✨ Features

* **Player Setup:** Easily set up 2, 3, or 4 players and customize their names.

* **Dynamic Faction Selection:**

    * Select which Smash Up! sets you own and want to include in the draft pool.

    * Granular control to include or exclude individual factions from chosen sets.

    * Visual indicators for partially selected sets (indeterminate checkboxes).

    * "Select All" and "Select None" options for quick configuration.

    * Displays the total number of factions available and a summary of excluded factions.

* **Multiple Draft Modes:**

    * **Pick 1 of 2 (Snake Draft):** Players take turns picking one faction from two randomly presented choices, following a snake draft order.

    * **Discard 1 of 3:** Each player is dealt three random factions and chooses one to discard, keeping the remaining two.

    * **Pure Random Assignment:** Factions are randomly assigned to players without any player interaction.

* **Interactive Draft Process:**

    * Clear indication of the current player's turn and pick number.

    * Visual feedback during faction selection/discard.

* **Draft History:** A detailed log of all picks and discards throughout the draft.

* **Persistent Settings:** Your selected sets and player names are saved locally in your browser, so your preferences are remembered for your next session.

* **Responsive Design:** Optimized for a seamless experience across desktop, tablet, and mobile devices.

## 🚀 How to Use

1.  **Access the App:**

    * **Web:** Visit the deployed application [here](https://liukus.github.io/smashuprandomizer/).

    * **Mobile (Hybrid App):** (Instructions for installing the Android/iOS app would go here if published to app stores).

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

    * The app will display the total number of factions available for the draft and how many are excluded.

4.  **Choose Mode:**

    * Select your preferred draft method:

        * **Pick 1 of 2 (Snake Draft):** For a more interactive draft where players choose between two options.

        * **Discard 1 of 3:** For a quicker draft where players discard one unwanted faction from three.

        * **Pure Random Assignment:** For an instant, completely random setup.

5.  **Start Draft:**

    * Click the "Begin Draft" button to start the process.

    * If you don't have enough factions selected for the chosen mode and player count, a warning message will appear.

    * A modal will appear showing the draft progress:

        * In "Pick 1 of 2" or "Discard 1 of 3" modes, the current player will be prompted to make their choice.

        * The "Draft History" section will log each action.

    * Once the draft is complete, the modal will display the final faction assignments for each player.

    * Click "Close" to dismiss the modal.

    * Click "Reset All" to clear all settings and start fresh.

## 🛠️ Technologies Used

* **React:** Frontend JavaScript library for building user interfaces.

* **Tailwind CSS:** A utility-first CSS framework for rapid styling.

* **Material-UI (MUI):** Used for the `TextField` component, integrated with a custom dark theme.

* **Capacitor:** (For future mobile app deployment) A cross-platform native runtime for web apps.

## 🙏 Support

If you find this app useful and would like to support its development, you can buy me a coffee!

[![Buy Me A Coffee at ko-fi.com](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/liukus)

## 📄 License

This project is open-source and available under the [GNU GPLv3 License](LICENSE). ```
