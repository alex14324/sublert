                                       _____       __    __          __
                                      / ___/__  __/ /_  / /__  _____/ /_
                                      \__ \/ / / / __ \/ / _ \/ ___/ __/
                                     ___/ / /_/ / /_/ / /  __/ /  / /_
                                    /____/\__,_/_.___/_/\___/_/   \__/

                                        Author: alex14324
                                            Version: 1.4.7

## What's this about?
Sublert is a security and reconnaissance tool that was written in Python to leverage certificate transparency for the sole purpose of monitoring new subdomains deployed by specific organizations and issued TLS/SSL certificate. The tool is supposed to be scheduled to run periodically at fixed times, dates, or intervals (Ideally each day). New identified subdomains will be sent to Slack workspace with a notification push. Furthermore, the tool performs DNS resolution to determine working subdomains.

## Requirements
- Virtual Private Server (VPS) running on Unix. (I personally use digitalOcean)
- Python 2.x or 3.x.
- Free Slack workspace.

## Installation & Configuration
## Usage

Short Form    | Long Form     | Description
------------- | ------------- |-------------
-u            | --url       | Adds a domain to monitor. E.g: yahoo.com.
-d            | --delete      | Domain to remove from the monitored list. E.g: yahoo.com.
-a            | --list       | Listing all monitored domains.
-t            | --threads       | Number of concurrent threads to use (Default: 20).
-r            | --resolve      | Perform DNS resolution.
-l            | --logging     | Enable Slack-based error logging.
-m            | --reset        | Reset everything.

## Feedback and issues?
If you have any feedback, anything that you want to see implemented or running into issues using Sublert, please feel free to file an issue on https://github.com/alex14324/sublert
