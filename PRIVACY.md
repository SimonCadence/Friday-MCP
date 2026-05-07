# Friday MCP — Privacy Policy

**Effective date:** May 6, 2026
**Contact:** simon@cadencegtm.io

Friday MCP is a personal, locally-run application that connects to the Pinterest API on behalf of the user who installs and authenticates it. This document describes what the application does and does not do with data.

## Who the app is for

Friday MCP is operated by Simon Lang for personal use and use by immediate family members. The application is not offered to the general public and is not used to provide a service to third parties. There is no centralized server: each user runs their own copy on their own device.

## What data the app accesses

When a user authenticates with Pinterest, Friday MCP requests read-only access to:

- The user's own Pinterest account profile (username, account type)
- The user's own boards and board sections
- The user's own pins (titles, descriptions, source links, image URLs)

The app does **not** request the ability to create, modify, or delete pins, boards, or any other Pinterest content. The app does not access other users' content beyond what is publicly available through Pinterest's API on the authenticating user's behalf.

## What data the app stores

- **OAuth access and refresh tokens** are stored locally on the authenticating user's device, in `~/.pinterest-mcp/tokens.json`, with file permissions set to user-only read/write. Tokens are used solely to make subsequent Pinterest API requests on the user's behalf.
- **API responses** (pin, board, and section data) are not persistently stored by the application. They are returned to the locally-running tool that requested them and discarded.

No data is transmitted to any server other than Pinterest's official API endpoints.

## What the app does not do

- The app does not collect telemetry, analytics, or usage metrics of any kind.
- The app does not send data to any third party other than Pinterest itself.
- The app does not share, sell, or disclose any user data.
- The app does not advertise.
- The app does not create a centralized database of user data.

## Data retention and deletion

Tokens and any cached data persist on the user's own device until the user takes one of the following actions:

- Deletes the `~/.pinterest-mcp/` directory on their device.
- Revokes Friday MCP's access via Pinterest's account settings (Settings → Apps → Revoke).

Once tokens are revoked or deleted, the application can no longer access any Pinterest data.

## Children

The application is not intended for or directed to children under the age of 13.

## Changes to this policy

If material changes are made to this policy, the updated version will be published at the same URL with an updated effective date.

## Contact

Questions about this policy can be sent to simon@cadencegtm.io.
