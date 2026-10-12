# Shodan Bulk Host Lookup

A Python utility for performing bulk IP address lookups using the Shodan API. Designed to streamline external attack surface reconnaissance by collecting host information for multiple IP addresses and exporting the results in a structured CSV format.

## Features

- Bulk Shodan host lookups from a list of IP addresses.
- Collects organisation, hostname, open port, operating system and ASN information.
- Exports results to CSV for analysis and asset inventory.
- Records lookup success and errors.
- References raw JSON responses for further investigation.

## CSV Output

| Field | Description |
|---|---|
| `ip` | Queried IP address |
| `found` | Whether Shodan returned host information |
| `org` | Associated organisation |
| `hostnames` | Hostnames associated with the IP |
| `ports` | Ports identified by Shodan |
| `os` | Detected operating system |
| `asn` | Autonomous System Number |
| `raw_json_path` | Path to the raw Shodan JSON response |
| `error` | Any errors encountered during lookup |

## Use Cases

Useful for penetration testing, external attack surface assessments, asset discovery and infrastructure reconnaissance.

**Note:** Results reflect Shodan's indexed data and may not represent the current state of a host. Findings should be independently verified.
