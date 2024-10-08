---
layout: default
title: Changelog
---
# Changelog

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

