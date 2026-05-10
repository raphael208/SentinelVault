# SentinelVault
SentinelVault: AI-Driven Password Analyser 🛡️
A Proof of Concept (POC) for the CDV Science Expo 2026 Category: Computer Science and Software Engineering

Developer: Raphael Murphy

  Project Overview
SentinelVault is a high-fidelity password security tool designed to move beyond traditional "complexity rules" (e.g., must contain a number/symbol). This project focuses on True Information Entropy and Privacy-Preserving Breach Detection to provide users with a scientifically grounded security score.

Key Features
Heuristic Pattern Analysis: Uses the zxcvbn library to detect dictionary words, names, l33t-speak, and keyboard patterns (e.g., qwerty).

k-Anonymity Leak Check: Integrates the "Have I Been Pwned" API. The application hashes the password locally (SHA-1) and only transmits the first 5 characters to the server, ensuring the user's plain-text password never leaves the browser.

Entropy Calculation: Converts pattern-guessing log-values into bits of entropy for a mathematical strength assessment.

Secure Suggestions: Recommends high-entropy passphrases over complex but guessable passwords.

  Technical Stack
Frontend: HTML5, CSS3 (Custom Dark Mode UI)

Logic: JavaScript (ES6+)

Security: Web Crypto API (SubtleCrypto)

APIs/Libraries: * zxcvbn for strength estimation.

HIBP Pwned Passwords for breach detection.

  Repository Structure
To show the Engineering Evolution required for the 2026 Science Expo, this repository includes:

index.html: The final production-ready code (SentinelVault).

/prototypes:

  v1_basic_ui.html: Initial layout and CSS.

  v2_logic_integration.html: Integration of the entropy library without the API.

/docs: Contains the digital versions of the Project Report and Research Plan.

  Ethics & Privacy
In alignment with the Eskom Expo Ethics Guide, this project is designed with a "Privacy-First" architecture:

No plain-text passwords are ever sent over the network.

No user data is stored, logged, or tracked.

All hash comparisons are performed locally in the user's browser.

  Acknowledgments
Special thanks to the developers of zxcvbn and Troy Hunt (HIBP) for providing the infrastructure to make local security auditing possible for the average user.
