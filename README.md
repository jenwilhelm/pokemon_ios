Pokemon iOS
===========

### Releases

Use ionic? Go native (swift?)?

##### MVP
1. Sign up (oAuth? custom account?)
2. Login/Logout
3. Find current location, list nearby locations (Foursquare, Google maps API?)
4. Check in to location
5. Display which Pokemon spawned at check in
6. List Pokemon at location
7. Swap/trade Pokemon at location
8. Maintain history of when/where Pokemon spawned/who owned it?
9. User Account (profile page, list of current Pokemon)

##### v2
1. Trade Pokemon with players
2. Add/remove friends

##### v3
1. Items (Rare candy!)
2. Ability to purchase items with real $?
3. Do items spawn at check in?

##### v4
1. Battle other players (friends? anyone?)

### Database structure

**User**
- id
- firstName
- lastName
- email
- image

**Parents** (master list of all 700+ Pokemon)
- id
- name
- image
- spawn_rate

**Pokemon** (spawned)
- id
- parent_id (from master list)
- user_id
- date_created
- location_ids (we need a better way to reference history)
- owner_ids (we need a better way to reference history)

**Location**
- id
- name
- lat
- long
- pokemon_ids
- type (restaurant, retail, etc)
- date_created
- last_checkin

### Tasks

So that Jen doesn’t forget while she’s thinking of them. Trello board?

* Enter all 700+ Pokemon into database (use a scraper for this?)
* Decide spawn rates for each Pokemon
* Decide which Pokemon go into Pokemon iOS & Pokemon Android

<img src="http://cdn.bulbagarden.net/upload/thumb/e/e2/133Eevee.png/250px-133Eevee.png">
