NEXA Mortgage Pathfinder — Website Files (Redesigned)
Export date: October 16, 2026

Contents
- index.html: homepage with the compass navigator and one-question-at-a-time evaluation
- articles/: ten interview-style articles, shared styles, and audio/navigation script

What changed in this version
- New visual design across the whole site: a dark "navigator" palette, a precision
  compass instrument on the homepage, and Fraunces + Hanken Grotesk typography.
- All ten articles share one stylesheet (articles/styles.css), so the look is
  consistent site-wide. Article content and links are unchanged.
- The homepage survey logic, the provisional calendar, and every disclosure/compliance
  notice are unchanged from the previous export.

Use
Extract this ZIP and upload index.html and the articles folder together to a static web
host. No build step is required. Fonts load from Google Fonts. You can also open
index.html locally for a basic preview.

Still to do (unchanged from before)
- Audio players are placeholders until the cloned-voice MP3s are supplied
  (the script expects files at audio/<article-name>.mp3).
- The survey and provisional calendar are client-side only. This export does NOT include
  a backend to store submissions, send email/SMS, or reserve real calendar appointments.
  The completion screen still says information was "recorded" and a meeting "reserved" —
  that copy should be changed, or a backend added, before launch.
- Hosting account, domain, and DNS configuration are not included.
