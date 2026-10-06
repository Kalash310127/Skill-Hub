# Skill-Hub

SkillHub is a full-stack skill-exchange platform built with Django REST and React. Users list skills they can teach, browse what others offer, and request to learn. They then join live video sessions, share materials, and review each other.
Core features
Listings: Each skill has a category, tags, level, experience, a fixed session time and a seat capacity.
Smart search: Results are ranked by TF-IDF cosine similarity with synonym expansion, so a query like "python for beginners" can find "Intro to Python scripting".
Request workflow: Requests move through pending, accepted, rejected, completed and cancelled. Requests over capacity are waitlisted, and a cancellation promotes the next learner automatically.
Live sessions: A unique Jitsi Meet room is generated when a request is accepted. It needs no API keys.
Materials and reminders: Teachers upload versioned zip files per lecture. A scheduled command sends a notification 30 minutes before each session.
Reviews and achievements: Learners leave one review per completed exchange. Completed skills appear on the learner's profile as achievements, kept separate from skills they teach. Teachers with consistently high ratings and positive reviews are flagged as "standout".
Profiles: Private and public profiles, a wishlist, notifications, a dark/light theme and a first-login tutorial.