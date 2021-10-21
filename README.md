# Mindless Minutes

To take the stress out of meditations.

## Usage

```sh
$ ./mindless_minutes -h
Usage: mindless_minutes - Post meditation sessions every day in specified date range

Required:
    -T token                Authentication token
    -M meditation_uuid      The meditation_uuid specifying an audio class

Optional:
    -s YYYY-MM-DD           Start date in YYYY-MM-DD format (Defaults to today)
    -e YYYY-MM-DD           End date in YYYY-MM-DD format (Default to today)
    -d seconds              Duration of meditation (Defaults to 600 seconds)
    -t HH:mm:ss             The time to start meditation around each day. (Defaults to 07:00:00)
    -j seconds              The "jitter" in time for each meditation session. (Defaults to 10 seconds)
    -u seconds              The timezone offset. E.g. LA timezone is -7 which is -25200 seconds.
    -D                      Dry run without posting. Inspect sessions.json for debugging.

Examples:
    Post meditation for today:
        mindless_minutes -T AUTH_TOKEN -M MEDITATION_UUID
    Post meditation from 10/01 to 10/30:
        mindless_minutes -T AUTH_TOKEN -M MEDITATION_UUID -s "2021-10-01" "2021-10-30"
```

