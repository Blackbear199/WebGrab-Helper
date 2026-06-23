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

- Windows
https://onedrive.live.com/download?id=%2Fpersonal%2F306f1b47acf88caf%2FDocuments%2FWebGrabHelper%2Fhelper%5Fv1%2E0%2E2%5Fwin%5Fx64%2Ezip&parent=%2Fpersonal%2F306f1b47acf88caf%2FDocuments%2FWebGrabHelper
- Linux
https://onedrive.live.com/download?id=%2Fpersonal%2F306f1b47acf88caf%2FDocuments%2FWebGrabHelper%2Fhelper%5Fv1%2E0%2E2%5Flinux%5Fx64%2Etar%2Egz&parent=%2Fpersonal%2F306f1b47acf88caf%2FDocuments%2FWebGrabHelper

Extract,Configure and run the executables for your platform.

## Notes

- No source code is included
- No external dependencies are required beyond what is listed in the setup files
