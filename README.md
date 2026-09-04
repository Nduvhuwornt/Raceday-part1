# RaceDay - PROG6212 PoE

## System Description
RaceDay is a full-stack web-based event management system for the South African road running,
walking, and cycling community. Event Organisers can create and manage events, categories, and
participant results. Participants can browse upcoming events, enter events, and track their personal
results history.

## Roles
- **Organiser** — creates, edits, and deletes events; manages event categories; captures participant
  results; views all enrolments for their events.
- **Participant** — creates an account; browses events; enrols in an event by selecting a category;
  views their own enrolments and results.

## Part 1 - System Planning and Database
All Part 1 planning artefacts are committed under `/docs`:
- `RaceDay_ERD.png` / `RaceDay_ERD.pdf` — Entity Relationship Diagram (6 entities: Roles, Users,
  Events, Categories, EventEnrolments, Results).
- `API_Endpoint_Plan.pdf` (also included as `API_Endpoint_Plan.md` for easy editing) — full endpoint
  plan covering Authentication, User Profile, Events, Categories, Event Enrolments, and Results.
- `RaceDay_Database.sql` — SQL Server script creating the schema and seeding sample data
  (2 Organisers, 2 Participants, 3 Events, categories per event, sample enrolments and a result).

### Running the SQL script
1. Open SQL Server Management Studio (SSMS) and connect to a local/clean SQL Server instance.
2. Open `docs/RaceDay_Database.sql`.
3. Execute the script (F5). It creates the `RaceDayDB` database, all tables with constraints, and
   seeds sample data.

## CI/CD
- `.github/workflows/validate-docs.yml` checks on every push that the `/docs` folder and required
  Part 1 files exist, and that a `README.md` is present at the repository root.
- [ ] Add screenshot of a successful green build here before submission.

## Video
- [ ] Add unlisted YouTube link here — walkthrough of the ERD, endpoint plan, and a live run of the
  SQL script in SSMS.
<img width="1917" height="912" alt="workflow" src="https://github.com/user-attachments/assets/5003bd13-90a8-4e47-8021-32e59184c27d" />


## AI Disclosure
- [ ] State briefly here which parts of this submission (if any) used AI assistance (e.g. planning,
  proofreading), per the assignment's AI disclosure instruction. Note: the API and MVC code you write
  in Parts 2 and 3 must be your own work with your own analysis, per the assignment brief — the
  planning documents in `/docs` are a starting scaffold for you to review, adjust, and understand, not
  a substitute for your own commit history or your own explanation in the video.
