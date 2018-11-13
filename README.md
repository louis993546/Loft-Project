# Project Loft

## What is this?

- A service that helps people who live together (roommates)
- A bunch of little things that make their life just a bit easier

### Components

- [API](https://github.com/louistsaitszho/Loft-API)
- Clients
  - [Android](https://github.com/louistsaitszho/Loft-Android)
  - [iOS](https://github.com/louistsaitszho/Loft-iOS)

### How it helps users

- Make it easier for people to keep track of what the apartment needs
  - Shared todo list
- Make it easier for people to keep in touch
  - Chatroom
- Make it easier for new joiners to catch up
  - Share notes
    - Share gallery
    - Share folder
    - Share schedule
  - Who is living here right now
  - Share schedule
    - Cleaning
    - Who want to take over the share space on which day
    - etc

## What is this repository?

- Share components of several repos
  - Client designs/mockups
- Higher level documents
  - Goal
    - Decisions

### Data & storage

- Industry standard structure
    - Relational Database (Postgres probably)
    - REST API (written in either golang or kotlin)
    - Android & iOS client
- Unique designs that fit the product needs
    - No username/password user flow
        - "We will never sell data & there is no meaningful data to sell. We don't even know who you are"

### Designs

- 90% platform specific + 5% loft branding + 5% user customization
    - It's personal: I want to learn more about UX in each platform
    - Loft is not something that's really necessary, the last thing I want is to have weird design that drive users away
        - "If it ain't broke don't fix it"
    - 5% branding mostly on colors and font
    - 5% customization allows user to have slightly higher personal connection with the product?

### Target users

1. People who live in shared apartment
2. 18-35 (probably)
3. 1 + 2 => probably without major disassability
4. it's an app =>  