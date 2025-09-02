Broken Access Control

Access Control enforce policy such that user cannot act outside of intended permissions.

common access control vulnabilities
-violation of principle of least priviledge.
-bypassing access control checks by modifying URL/API request - parameter tampering.
-permitting viewing/editing someone else's account by unique identifier.
-accessing api with missing access controls for POST, PUT and DELETE.
-Elevation of previledge (NOT USER-> acting as USER | USER-> acting as ADMIN).
-Metadata manipulation - (JWT, access control token, cookie or hidden fields)
-CORS misconfiguration - allowing API access from unauthorised/untrusted origin.
-Forcing browser to authenticate pages as unauthenticated user or to privileged pages.

Preventions
-except for public resources, deny bu default.
-Centralize access control logic/module -> if logic is scattered, one missed check = vulernability. A single system is easy to audit.
-Enforce ownership on the records -> user should only see/update their own data.
-apply business rule on domain level -> user can't transfer more than fixed amount, can't approve my own leaves...
-Harden Server/File configurations -> not visible from web root, disable directory listing.
-Log and monitor access control failure and trigger alert on repeated failures.
-Rate limit API and sensitive Endpoints -> helps with automated attacks.
-Secure session and token management -> invalidate session ids after logout and make JWT short lived, for long lived use oauth revocation/refresh token flow.
