# LAB-02 (Theory): Tracking vs Fingerprinting

## Overview
Tracking and fingerprinting are often used interchangeably, but they represent different identification mechanisms used by websites and online services.

Understanding this distinction is essential for cybersecurity and privacy analysis.

---

## Tracking

Tracking relies on **stored identifiers** that are saved on the user’s device.

Common tracking methods include:
- Cookies
- Local storage
- Session identifiers
- Account logins

### Characteristics
- Can often be cleared or reset
- Relies on client-side storage
- Widely used for analytics and personalization

---

## Fingerprinting

Fingerprinting identifies users by analyzing **environmental and behavioral characteristics** rather than stored data.

Common fingerprinting signals include:
- Browser version and configuration
- Operating system
- Screen resolution
- Timezone and locale
- JavaScript and rendering behavior
- Interaction timing patterns

### Characteristics
- Does not require cookies
- Persists across sessions
- Harder to avoid or reset

---

## Security Perspective

From a defensive standpoint:
- Tracking enables convenience and analytics
- Fingerprinting enables fraud detection and bot mitigation

Most modern systems use **both techniques together** to increase confidence in identification.

---

## Conclusion
Tracking is based on stored identifiers, while fingerprinting is based on observed characteristics. Understanding both is critical for analyzing modern web security and privacy risks.
