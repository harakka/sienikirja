# sienikirja
Sienikirja is a mushroom foraging journal web app built on Django, currently in early design stage. The main motive is helping keep track of mushroom finds and good mushroom harvesting spots over long period of time.

## Design
The technologies used are Django and PostgreSQL (+PostGIS for geodata) for backend, Leaflet for map layer, and custom HTML and JS for various input forms. The main target platform is mobile, because user is expected to use the app while they're in the woods picking mushrooms.

The main UI view is a map that automatically locates the user. User can add pins to map, which opens an input form for recording mushroom findings into their journal. User can input the type and number of mushrooms and other notes. The input form automatically fetches current and past weather info from FMI database API and the weather info is recorded into the journal entry automatically.

User has an option to login, which is a prerequisite for creating journal entries. User can manage their profile and view previous journal entries as a list, grouped by time (or location if possible). The app is not meant to be social, as mushroom pickers generally don't want to share their findings such features are not necessary.
