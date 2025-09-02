Insecure Design

-missing or ineffective control measures.
When your system is built without proper security controls in the first place.

Note: There is a difference between insecure design and insecure implementation. A secure design can still have imperfect implementation that may be exploited. An insecure design can not be fixed by perfect implementation as by definition, needed security controls were never created to defend against specific type of attacks.

Root causes
-No threat modeling (not thinking about how an attacker can abuse the system)
-No secure design patterns (re-using known good security practices)
-Not aligning with business risk profile (underestimating how valuable/sensitive the data/system is)
-ignoring secure-by-design (security is will implemented later)


Prevention
-Establish and use a secure development lifecycle with professionals to help evaluate and design security and privacy related controls.
-use a library of secure design pattern. 
-use threat modeling for critical authentication, access control, business logic and key flows.
-integrate plausible security checks at each tier of the application.
-write unit and integration test cases to validate that all critical flows are resistant.
-segregate tier layers on system and network depending in exposure and protection needs.
-segregate tenants robustly by design
-limit resource consumption by user or service.

examples
-protection against bots.
-question and answer as evidence of identity.
-Generating error message with sensitive information.
-Exposure of sensitive information due to incompactible policies/encryption.
-Broser caching/cookie preservation - sensitive data 
-improper handling of extra paramters.
-unprotected credentials - storage or recoverable.
-incorrect/improper/insufficient priviledge assignment.
-unrestricted uploads