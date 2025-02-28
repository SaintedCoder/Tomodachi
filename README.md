# Tomodachi
Replacement for Skype

Features: 
Voice calls, 
video calls, 
group calls (30+ users), 
file sharing, 
user accounts.

Security: 
End-to-end encryption, 
anti-hacking measures against skilled attackers.

Beginner-Friendly: 
Simple tools, 
lots of guidance, 
and pre-built pieces where practical.

Group Size: 
Over 30 means we’ll need a server-based approach (SFU) instead of mesh for group calls.
Simplified Tech Stack
Frontend
React: Web-based to start (easier for beginners than mobile). We’ll use Create React App.
Why: You can see results in your browser fast, and it’s beginner-friendly.
Backend
Node.js + Express: Easy to learn, tons of tutorials.
MongoDB: Free tier on MongoDB Atlas—simple setup, no server management yet.
Why: Keeps server-side code approachable.
Real-Time Communication
WebRTC: For voice/video, guided with a library like simple-peer.
SFU (Selective Forwarding Unit): Use mediasoup—a Node.js library for group calls. Pros won’t guess it easily.
Why: simple-peer simplifies WebRTC, and mediasoup handles 30+ users without choking.
Encryption
Libsodium: High-grade encryption, but we’ll use a simple wrapper (sodium-plus).
E2EE: Calls and files encrypted so only users can decrypt—not the server.
Why: Secure yet beginner-accessible with examples.
File Sharing
WebRTC Data Channels: For small files, E2EE.
Server Fallback: Encrypted uploads for big files.
Why: Balances ease and security.
