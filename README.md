# Helper Service

The Helper Service is a small standalone tool that handles network requests for any client
that connects to it. It supports normal HTTP requests, browser‑based requests, and
Flaresolverr‑style challenge solving when needed. The service cleans and normalizes the
responses so the client doesn’t have to deal with headers, cookies, redirects, or
JavaScript‑heavy sites.

It doesn’t depend on any specific application. Anything that can send JSON can use it.

## What It Does

- Runs HTTP, browser, mixed‑mode, and Flaresolverr‑style requests
- Normalizes and cleans the response body
- Handles proxies, VPN detection, and IP verification
- Automatically restarts safely when idle or when the console buffer grows too large
- Works on Windows and Linux
- Client‑agnostic: any external program can connect and process the responses

## Setup & Usage

- helper.ini                       — Helper configuration file
- helper-daemon.ini                — Daemon configuration file
- Helper-Payload-Readme.txt        — how to configure the Helper Payloads
- Helper-Payload-Web-UI-Readme.txt — how to use Helper Web Ui 
- Helper-Daemon-Install-Readme.txt — how to configure the Helper Daemon
- Helper-Daemon-Files-Readme.txt   — how to use new cdp file system

Refer to those files for installation, configuration, and usage details.

## End Points
Helper
http://ip:port/helper

Helper Web UI
http://ip:port/web

## Releases

## [2026-06-30] V1.0.4
### Added
- 
### Fixed
- Web UI monaco validation changed to auto mode
- Silence monaco traffic from console
- WEBUI added payload schema
- WEBUI added valid/invalid json/schema indicators
- WEBUI bug fixes.

Binary‑only releases are provided:

Windows
https://mega.nz/file/nyZHmZYK#LRjd8fkavuQMAuSx_abUWEuRsdiSANNbaUEbwHkz5Hg

Linux
https://mega.nz/file/Pv4lnSrQ#w8-CCp0QYa2ATQ7pyyIktEsSUuEp2a-KGlwak4e9NgY

Extract,Configure and run the executables for your platform.

## Notes

- No source code is included
- No external dependencies are required beyond what is listed in the setup files
