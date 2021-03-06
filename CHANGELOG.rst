Changelog
#########

v0.10.1 (2017-10-02)
--------------------
* Minor: Fix line ending of schedule.csv

v0.10.0 (2017-09-16)
--------------------
* Breaking Change: Output markdown files are no longer produced

* New Feature: The ability to add 'unbounded' events which occur in all rooms
  on all days

* Minor: Speaker names in their original form are included within the pickled
  events dictionary

* Minor: The full slots list, with index number, is included in the log file

* Minor: Allocated and unbounded events now have tags added automatically
  which ensure uniqueness (no longer necessary to use e.g. 'morning' tag)

* Bug Fix: Durations for unbounded and allocated events are taken from their
  definition (previously hard coded as zero)

v0.9.1 (2017-09-06)
-------------------
* Minor: io functions now take the working directories as arguments

* Minor: All proposals now included in pickled resources

v0.9.0 (2017-09-06)
-------------------
* New Feature: --reload option on validate command to control whether the
  conference definition is reloaded from input YAML files

* Bug Fix: --help option threw an error if run outside a valid project folder
  structure

v0.8.4 (2017-09-04)
-------------------
* Minor: Subtitles from proposals are now imported

v0.8.3 (2017-09-02)
-------------------
* Bug Fix: Original schedule and new schedule were being passed to the diff
  function in the wrong order

v0.8.2 (2017-09-01)
-------------------
* Bug Fix: Pre-allocated events were being scheduled in addition to their
  pre-allocated slot when optimising for consistency

v0.8.1 (2017-08-24)
-------------------
* Minor: Order of fields altered in schedule.csv

v0.8.0 (2017-08-21)
-------------------
* New Feature: --diff option to control logging of schedule diff


v0.7.2 (2017-08-21)
-------------------
* Bug Fix: Consistency optimisation fixed

v0.7.1 (2017-08-21)
-------------------
* Minor: Updated log message for Unavailability

v0.7.0 (2017-08-21)
-------------------
* Bug Fix: Remove use of strings for Slot.starts_at

* New Feature: Unavailability and clashes can now be defined for events as well
  as people

* New feature: Capacity objective now split into efficiency or equity

v0.6.0 (2017-08-18)
-------------------
* New Feature: Pre-allocated events can be defined in allocations.yaml

* Breaking Change: venues.yml renamed to timetable.yml

v0.5.0 (2017-08-17)
-------------------
* Breaking Change: content previously in separate yaml files now in venues.yaml

* New Feature: objective function argument added to build command

v0.4.1 (2017-08-16)
-------------------
* Improved logging with counts of events and slots by event type

v0.4.0 (2017-08-14)
-------------------
* New Feature: Venue availability can be defined

* Minor Improvement: Order of columns in schedule.csv swapped to show index
  numbers at lhs of file

v0.3.1 (2017-08-10)
-------------------
* Bug Fix: Redundant export of schedule on rebuild removed

v0.3.0 (2017-08-10)
-------------------
* New feature: Rebuild command
  Rebuild the output files from a previously computed schedule

v0.2.0 (2017-08-10)
-------------------
* New Featue: Validate command
  Validate a previously computed schedule

v0.1.0 (2017-08-10)
-------------------
* Initial release
