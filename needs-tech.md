# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given : There is a power shutdown
  When : Power restarts
  Then : Document data

Scenario: Reconcile counts if the sensor is offline for a while

  Given : The sensor that scans and counts is offline
  When : There needs to be details of people documented
  Then : Count the number once it restarts
