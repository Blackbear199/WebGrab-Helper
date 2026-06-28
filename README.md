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
- Helper-Daemon-Install-Readme.txt — how to configure the Helper Daemon

Refer to those files for installation, configuration, and usage details.

## Releases

Binary‑only releases are provided:

Windows
https://mega.nz/file/T3ZF0AhY#WYnWn_FXKQ4P5Ds8k_1Qnvi0-78NaldV0eBpO9WDBjg

Linux
https://mega.nz/file/yvQBRTCQ#cDynR6q-K0M74J4j9Urw-gWxNWpgggAs0gUawOpd_eI

Extract,Configure and run the executables for your platform.

## Notes

- No source code is included
- No external dependencies are required beyond what is listed in the setup files
