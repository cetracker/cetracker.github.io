---
layout: default
title: Changelog
nav_order: 5
---
# Changelog

Since 2026 the backend and the frontend are released and versioned independently;
entries below name both versions.

- 2023-03-28 - v0.1.0
  - first public release
- 2023-04-02 - v0.2.0
  - Bugfixes
  - PartTypes can be marked as mandatory.
  - Display details of part types and which parts have been used as such and when.
  - Include altitude and power details to tours.
  - Allow tours to be grouped by year and month.
  - Add calculated sum to each tour table's column.
- 2023-04-02 - v0.2.1
  - Offer multi platform container images, enabling it to run on Pi-OS 64
- 2023-07-23 - v0.2.2
  - Bugfixes
    - PartType was no longer pre selected on relation edit
    - internal fixes  
    - Current Time was used for initial validFrom value in relation edit dialog
  - Improvements
    - basic relation validation
    - upgrade MantineReactTable
    - updates for many libraries
- 2023-07-23 - v0.2.3
  - Maintainance
    - Library Updates
  - Bugfixes
    - Fix hibernate mapping mismatch
- 2024-09-12 - v0.2.4
  - Improvements
    - Value aggregation on tour list page when grouping
  - Maintainance
    - Library Updates
    - JDK update
- 2024-09-18 - v0.2.5 (frontend)
  - Improvements
    - Sorting by valid from by default on Part-PartType-Relations
    - Add 'last used at bike' on part list
    - Add an action to select a previously used part as the currently used one for the currently displayed part type
      on the part type - relation list
  - Maintainance    
    - Upgrade vite, eslint etc
  - Bugfixes
    - Fix errors related to framework and dependency upgrades
- 2026-06-18 - BE v0.5.0 / FE v2.2.0 — development resumed after a longer break
  - Improvements
    - Structured part attributes (manufacturer, model, serial number, …) instead of an overloaded name
    - Sorting for parts and part types; part info disclosure in the usage report
  - Bugfixes
    - A whole batch of error-handling fixes: proper HTTP statuses, no more silent deletes/no-ops
- 2026-06-25 - BE v0.6.0 / FE v2.3.0
  - Features
    - Import new tours directly from an uploaded MyTourBook database, with review and duplicate warnings
    - Filter retired parts and search in part/part-type pickers
    - Tour import can take the bike per tour from the JSON file
- 2026-06-30 - BE v0.7.0 / FE v2.4.2
  - Features
    - **FIT file import** — CETracker no longer depends on MyTourBook for tour data
    - Auto-derive a part's first-used date from its first relation
  - Bugfixes
    - Correct power/work semantics and the usage report summary row
- 2026-07-03 - BE v0.8.0 / FE v2.5.0
  - Features
    - Landing page makeover
    - Info box with backend/frontend version numbers
- 2026-07-10 - BE v1.0.0 / FE v3.0.0 — major release
  - New domain model: parts became **components**, which can be grouped into **assemblies**
    (e.g. wheelsets) and mounted or swapped as one unit
  - **Maintenance tasks** with distance/time intervals, event history and overdue notifications
  - Usage report for a selectable time frame, per component or per bike
  - Bike history: composition on any past date, full mounting history
  - Translations — English / German for a start; configurable date/time display
  - Backend moved from MySQL to **PostgreSQL** with a fresh migration baseline
  - Landing page with getting-started cards and a guided tour
- 2026-07-13 - BE v1.0.1 / FE v3.0.1
  - Features
    - Cross-links between component detail and assembly views
  - Bugfixes
    - Mounting overlap on membership correction was reported as an internal error
