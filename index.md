---
title: Cycle Equipment Usage Tracker
layout: home
---
# Cycle Equipment Usage Tracker

## About

If you own and use a bicycle extensivly, you might have wondered how many miles and hours you have used certain parts of it.  
How many miles has lasted your the last chain. How many miles the brake pads have been attached to the bike?

If you have ever asked yourself these questions, CETracker might help you.

Even more so, if you are used to change parts frequently. You have a second set of wheels, you choose to ride with based on the type of the tour? If your are up to keep track of your bike maintance in CETracker, the answer of your questions is only one click away.

As a personal project, it was born after I had these questions mentioned above. Since using [MyTourBook](https://mytourbook.sourceforge.io/) to keep track of all my tours, I've joined the discussion about a feature sugesting issue [777](https://github.com/mytourbook/mytourbook/issues/777) on the MyTourBook GH project. Basically, this project spawned from the ongoing discussion.  
Even though, it's still more or less a showcase for this feature, it's still usable on it's own.

## Prerequesite

- MyTourBook is used for tour statistic
  - Alernativly, the cumbersome work of manually entering the basic details about the completed tours would be possible
  - Importing tours from exports of well known tour tracking sites is imaginable
- Docker-Compose for [cetracker-compose](https://github.com/cetracker/cetracker-compose), Docker or Podman is installed on your local computer (There are no plans of hosting CETracker anywhere.)
  - Alternativly you could build and run the [cetracker-backend](https://github.com/cetracker/cetracker-backend) (Kotlin - Java 17)  and the [cetracker-frontend](https://github.com/cetracker/cetracker-frontend) (npm/yarn - vite - React). There will be build instructions on the projects repository.
- A rudimentary basic understaning of SQL to export the data from the MyTourBook Derby database. See [Data Export Documentation](./data-export.md) for instructions.

## Known Limitations

Currently there a couple of known limiations and places in the need of polishing. It's a showcase or a MVP only.

- Error handling needs to be improved in quite a few places
- User input validation needs to be extended quite a bit.
- Entered data can't be modified or deleted via the UI.
- Glitches in the UI.
- Currently tested for one single bike only. For supporting more than one bike, the code needs some refactoring on a few places.
- No multi user support (currently not planned either)
- A basic report is generated only. Time range can't be selected. No filtering, grouping is supported currently.

[GH Pages at:](cetracker.github.io)
