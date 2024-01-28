### Denial-of-service (DoS)

A threat actor makes a target device\\resource unavailable by overloading it using a device

#### Example

*   A threat actor uses one device to overload XYZ LLC's website (This was common in the old days, but nowadays it often does not work )

* * *

### Distributed Denial of Service (DDoS)

A threat actor makes a target device\\resource unavailable by flooding using multiple devices

#### Example

*   A threat actor uses hundreds of infected devices to flood XYZ LLC's website

* * *

### Man in the Middle (MITM)

A threat actor intercepts and relays messages between 2 targets (This attack is a type of eavesdropping attack)

#### Types

*   Hijacking attack
    *   Session Hijacking
        *   A threat actor accesses the user's account using a stolen or leaked valid (existing) session identifier
*   Eavesdropping attack  
    *   Wi-Fi Eavesdropping (Evil Twin)
*   Spoofing attack
    *   ARP Spoofing
        *   A threat using the victim's MAC (This happens after ARP poisoning)
    *   DNS Spoofing
        *   When a victim gets directed to a malicious website (This happens after DNS poising)
    *   HTTPS Spoofing

#### Example

*   A threat actor inserts themself between a victim and a website; the victim is under the impression that the traffic is going directly to the website

* * *

### Buffer-Overflow

A threat actor attempts to write extra data to a fixed-size block of memory

Types

*   Heap-based overflow
    *   A threat actor injects a malicious payload on the target's heap, causing non-intended actions (a heap is a memory set used for dynamic allocation - data created create on the fly - Heap is a hierarchical data structure)
*   Stack-base overflow
    *   A threat actor injects a malicious payload on the target's stack, causing non-intended actions (a stack is a collection of components that work together to support the execution of the target - A stack is a linear data structure)
*   SEH Overflow
    *   A threat actor injects a malicious payload on the target's stack, causing non-intended actions by corrupting the Structured Exception Handler (SEH) and Next Structured Exception Handler (NSEH) records - Exception registration record (SEH) is a pointer to the current exception record, the following exception registration record is a pointer to the following exception record (NSEH)

Example

*   A threat actor sends the 123456MALICIOUS string to a vulnerable app that only handles 6 bytes strings; the rest of the string is written an area where it holds executable code, afterword MALICIOUS gets executed

* * *

### Cross-Site Scripting

A threat actor aims to execute malicious actions on the victim's website (It's a client-side code injection attack)

#### Types

*   Reflected Cross-Site Scripting
    *   A threat actor injects malicious content into web pages or web applications. The content will be reflected in the response and executed in the victim's browser
*   Dom-Based Cross-Site Scripting
    *   A threat actor injects malicious content into web pages or web applications. The content is not reflected in the response and is executed in the victim's browser
*   Stored Cross-Site Scripting
    *   A threat actor injects malicious content into a vulnerable server. The content is getting retrieved by users and then executed

* * *

### Cross-site request forgery

A threat actor may trick an authenticated or trusted victim into transmitting unauthorized actions on their behalf

#### Example

*   A threat actor crafts an exploit URL for a fund transfer and sends it to an authenticated user

* * *

### Privilege escalation

A threat actor gains privileges beyond what is entitled

#### Types

*   Horizontal Privilege Escalation
    *   A threat actor performs unauthorized functions belonging to another user with a similar privileges level
*   Vertical Privilege Escalation
    *    A threat actor performs unauthorized functions belonging to another user with a higher privileges level 

* * *

### Replay

A threat actor captures transmitted data and then repeats it (It's also called playback attack)

* * *

### Pass-the-Hash Attack

A threat actor captures a hashed user credential (Not the actual password) and reuses it (The threat actor is getting authenticated without using the password itself or cracking it)

#### Example

*   A threat actor requests access (Connection request), the server responds with an authentication challenge, the threat actor sends the username and the captured hash, the server checks the hash and grants access to resources
