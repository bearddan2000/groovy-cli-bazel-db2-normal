# groovy-cli-bazel-db2-normal

## Description
Creates a small database table
called `dog`. This table, `dog`, has been normalized to 3NF.
All output normally
seen in a terminal will be in `groovy-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- docker-wait
- groovy
- bazel
  - log4j
  - db2 driver

## Docker stack
- l.gcr.io/google/bazel:latest
- ibmcom/db2

## To run
`sudo ./install.sh -u`
Creates groovy-srv/log

## To stop
`sudo ./install.sh -d`
Removes groovy-srv/log

## For help
`sudo ./install.sh -h`
