# Timesyncd Configuration Role

Configure Ubuntu [timesyncd](https://ubuntu.com/server/docs/about-time-synchronisation#about-timesyncd) to use specific NPT servers.

## Requirements

This role is tested on Ubuntu 22.04. There are no other requirements.

## Role Variables

By default we use the [NRC NTP servers](https://nrc.canada.ca/en/certifications-evaluations-standards/canadas-official-time/network-time-protocol-ntp).

| Variable                       | Default         |
| ------------------------------ | --------------- |
| timesync_primary_ntp_server    | time.nrc.ca     |
| timesync_secondary_ntp_server  | time.chu.nrc.ca |
| timesync_root_distance_max_sec | 5               |
| timesync_poll_interval_min_sec | 32              |
| timesync_poll_interval_max_sec | 2048            |
| timesync_timezone              | UTC             |
