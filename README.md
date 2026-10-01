## Sport Manager

Sport Manager is a full-stack platform for managing sports leagues, teams, and match scheduling. It connects players, coaches, venue owners, and administrators through role-based workflows, covering everything from league organization to venue reservations and live match results.

### Features
- User registration, login, and role-based access (player, coach, venue owner, administrator)
- League and team management, including team registration and coach assignment
- Match scheduling with conflict detection
- Live results entry with automatically updated standings and player/team statistics
- Venue availability management with reservation requests, an approval workflow, and a waitlist for fully booked slots
- Real-time notifications for reservations, match updates, and league activity
- Public, filterable views of schedules, results, and league tables
- PDF export of tables, schedules, and statistics
- AI-based predictions for match outcomes and final league standings

### Technologies

- **Frontend:** React
- **Backend:** Node.js, Express, Prisma
- **Database and cache:** PostgreSQL, Redis
- **Testing:** Jest, Vitest
- **DevOps:** Docker, GitHub Actions

### Architecture

The application follows a client-server architecture: a React frontend communicates with a Node.js/Express REST API, which uses PostgreSQL as the database and Redis for caching.

### Testing

- **Backend** – tests with Jest, run against a real PostgreSQL and Redis instance in Docker containers, so database queries and API behavior are tested without mocks
- **Frontend** – component tests with Vitest

Tests run automatically on every push and pull request with GitHub Actions.

### How to run tests

Frontend:

    cd Projekat/frontend
    npm install
    npm test

Backend tests need a running PostgreSQL and Redis instance (see `.github/workflows` for the configuration used in CI):

    cd Projekat/backend
    npm install
    npm test

## Scrum documentation

Each `SprintN` folder contains the documentation for that sprint, such as the sprint goal, backlog, sprint review and retrospective.
