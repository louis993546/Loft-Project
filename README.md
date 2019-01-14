# Project Loft

## Index

- [Goal](#goal)
- [Objective](#objective)
- [Architecture](#architecture)
- [UX](#ux)
- [Why Project Loft](#why-project-loft)
- [Privacy](#privacy)
- [Security](#security)
- [Roadmap](#roadmap)
- [Idea dump](throughtNote.md)

## Goal

- Reduce the overhead in communicating with roommates
- Automate/Streamline/Coordinate common tasks

## Objective

- Native apps on Android and iOS
- Share chatroom for each share flat
- Share task/shopping list
- Share notes
- Share roommates informations
- Share calendar

## Architecture

### TL;DR

- GraphQL API
  - Authentication middleware
- PostgreSQL RDBMS
- Hosted on Heroku (for now)
- Native Android & iOS apps
  - Fetch data from GraphQL API into local storage

### Graph

TODO: draw it out on figma or something

### Graph explained

TODO: be more specific on which part takes care of which 

## UX

- Material-based design on Android
- Human Interface Guideline-based design on iOS
- TL;DR: Don't reinvent the wheel (expecially when you are not a wheel designer/engineer)

## Why Project Loft

- It's the 1-stop-shop for all your dealing-with-roommate needs
- It cares about your privacy

## Privacy

### Techical perspective

- It is design to don't ask for your email, phone number, real name, access to social media, anything
- It is built with GDPR compliance in mind
- All the source code is available right here on GitHub, you can proof (or disproof) if there is any melicious code

### Operation perspective

- (Almost) everything is free for anyone to check out, except
  - Keys, secrets, and other private resource to deploy to server, Play Store, and App Store
- We respect your rules to be forgotten
- (TODO: more GDPR stuff)

## Security

TODO: In progress

## Roadmap

- [Milestone](https://github.com/louistsaitszho/Loft-Project/milestones?direction=asc&sort=due_date&state=open) contains the general roadmap of the whole project
- [API progress](https://github.com/louistsaitszho/Loft-API/projects/1)
- [Android progress](https://github.com/louistsaitszho/Loft-Android/projects/2)
- [iOS progress](https://github.com/louistsaitszho/Loft-iOS/projects/1)