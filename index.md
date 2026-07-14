---
title: Home
layout: home
nav_order: 1
---
# Cycle Equipment Usage Tracker

## About

If you use one or more bikes extensively, you may have wondered how many miles and hours certain parts of your bike have been in use.
How many miles did the last chain last before it had to be replaced? How many hours did the last brake pads last?

If you've ever asked yourself these questions, CETracker can probably help.

Even more so if you change the parts on your bike frequently. Do you have several sets of wheels that you use depending on the type of tour? If you are prepared to keep track of your bike maintenance with CETracker, the answers to these questions are just a click away.

![landing page](./pictures/landing.png)

## What it does

- Track any number of **bikes**, each with the mount points you care about (chain, cassette, tires, …).
- Manage your **components** with purchase details and see where each one is — or was — mounted.
- Group components into **assemblies** (e.g. a wheel with its tire and cassette) and mount or swap them as one unit.
- Import your **tours** from [MyTourBook](https://mytourbook.sourceforge.io/) or directly from `.fit` files (Garmin, Wahoo, Coros, Suunto, …).
- Get a **usage report** — distance, moving time, climbing and work — per component or per bike, for any time range.
- Define **maintenance tasks** with distance or time intervals and get notified when they are overdue.
- Travel back in time: view a bike's **composition on any past date** and browse the full mounting history.

See the [Getting Started](./getting-started.html) guide for a step-by-step walk-through of the initial setup,
and the [Screenshots](./screenshots.html) page for more impressions.

## Prerequisites

- Docker or Podman with Compose on your local computer, for running [cetracker-compose](https://github.com/cetracker/cetracker-compose). (There are no plans of hosting CETracker anywhere.)
  - Alternatively you could build and run the [cetrack-backend](https://github.com/cetracker/cetrack-backend) (Kotlin - Spring Boot) and the [cetrack-frontend](https://github.com/cetracker/cetrack-frontend) (npm/yarn - vite - React) yourself. There are detailed building instructions in each sub project's repository.
- Tour data from one of the supported sources — see [Importing Tours](./tour-import.html):
  - `.fit` files recorded by your bike computer or sports watch,
  - or a [MyTourBook](https://mytourbook.sourceforge.io/) tour database (JSON export or direct Derby database import).

## Known Limitations

There are still some rough edges:

- Backend error messages aren't always surfaced properly in the UI yet.
- Imported tours can't be modified or deleted via the UI.
- No multi user support, let alone with data separated from each other (currently not planned either).

## History

CETracker is a personal project that came about after I had the issues mentioned above. Since I have been using
[MyTourBook](https://mytourbook.sourceforge.io/) for many years to keep track of all my tours, I've joined the discussion in suggested feature issue [777](https://github.com/mytourbook/mytourbook/issues/777) about adding this functionality on the MyTourBook GH project. Basically, this project grew out of that discussion.
CETracker has evolved from being just a showcase for this suggested feature to a tool usable on its own.
Even though MyTourBook now offers this functionality, I got used to using CETracker and accumulated a huge amount of data inside it, which I would have to migrate.

[The source for this GH-Page:](https://cetracker.github.io) [is in this repo](https://github.com/cetracker/cetracker.github.io.git)
