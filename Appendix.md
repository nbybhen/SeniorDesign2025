# CS5002 Final Design Report - Appendix

## A. References and Citations

### Technologies & Frameworks
- **Next.js** - React framework for production applications
- **TypeScript** - Typed JavaScript for safer development
- **Supabase** - Open-source Firebase alternative with PostgreSQL backend
- **Docker** - Container platform for isolated code execution environments
- **WebSocket** - Real-time bidirectional communication protocol
- **AWS Lambda** - Serverless compute for matchmaking orchestration
- **Tailwind CSS** - Utility-first CSS framework for responsive UI

### Code Repositories
- **Main Repository:** https://github.com/nbybhen/CodeColosseum
- **Deployment & Infrastructure Code:** Contained in `/infra` directory
- **Execution Engine:** Contained in `/execution-engine` directory
- **Frontend Source:** Contained in `/src` directory

### External Tools & Services
- **GitHub** - Version control and collaboration
- **Supabase** - Database hosting and real-time APIs
- **AWS** - Cloud infrastructure (Lambda, S3, CloudWatch)
- **Vercel** - Frontend deployment platform

---

## B. Code Repository Links & Evidence

### Primary Repository
All source code is maintained in a single Git repository: **https://github.com/nbybhen/CodeColosseum**

**Key directories:**
- `/src/app` - Next.js application pages and API routes
- `/src/components` - Reusable React components
- `/src/lib` - Utility functions and service integrations
- `/execution-engine` - Docker-based isolated code execution
- `/infra/aws` - Infrastructure as Code (Lambda functions, scheduler scripts)
- `/supabase` - Database migrations and real-time configuration


## C. Meeting Notes & Project Timeline

### Project Phases & Milestones

#### Phase 1: Research & Tech Stack Selection (Aug 26 - Oct 10, 2025)
- **Aug 26-30**: Team formation, contract signing, meeting schedule established
- **Sep 1 - Oct 1**: Database & backend selection (PostgreSQL/Supabase)
- **Sep 1 - Oct 10**: Programming language support definition
- **Sep 16 - Oct 25**: Web IDE dependency research and evaluation
- **Oct 1 - Oct 31**: Docker containerization setup and configuration

#### Phase 2: Design & Prototyping (Oct 6 - Nov 30, 2025)
- **Oct 6 - Nov 30**: Project branding, logo design, landing page UX/UI
- **Oct 6 - Nov 30**: Multiplayer UI design and component library research

#### Phase 3: Implementation - Alpha Release (Nov 1 - Dec 30, 2025)
- **Nov 1 - Dec 15**: Database schema design and UML diagrams
- **Nov 1 - Dec 30**: Real-time WebSocket logic implementation
- **Nov 1 - Dec 30**: User authentication service integration
- **Nov 25 - Dec 30**: Functional 1v1 demo build completion

#### Phase 4: Post-Semester Development & Production Features (Jan - Apr 2026)
- **Jan 2026**: Competitive matchmaking system implementation (48 commits)
- **Feb 2026**: Competitive battle pages and results display (10+ commits)
- **Mar 2026**: 2v2 team-based competitive feature development (8+ commits)
- **Mar-Apr 2026**: Bug fixes, edge case handling, production stabilization (20+ commits)
- **Apr 2026**: AWS Lambda infrastructure and automated scheduling

---

## D. Evidence of Hours & Effort Justification

### Overall Team Effort Summary
- **Total project duration:** August 2025 - April 2026 (9 months)
- **Total commits by team:** 100+ commits in primary repository
- **Files modified:** 150+ unique files
- **Code lines contributed:** 5,000+ lines across all team members

### Ruduczo Mushunje (ruklee13) - 107 Hours
**Git Evidence:**
- Commits authored: 60+ commits (verified from export: Jan-Apr 2026)
- Files modified: 100+ files across API routes, infrastructure, and frontend
- Date range: Nov 2025 - Apr 2026
- Key contributions logged in: `/assignments/RukudzoTimeLine.md`

**Breakdown of hours by phase:**
1. Research & Backend Selection (5 hrs) - Initial tech stack evaluation
2. Language Support Definition (6 hrs) - Programming language compatibility analysis
3. Docker Infrastructure (7 hrs) - Container setup and deployment configuration
4. Frontend Design & UI (8 hrs) - Landing page and dashboard prototyping
5. Frontend Implementation (6 hrs) - UI component development
6. Integration & Testing (5 hrs) - API integration debugging
7. QA & Testing (4 hrs) - Test case development and validation
8. Competitive Matchmaking P.1 (12 hrs) - Core queue management and match initialization
9. Competitive Implementation P.2 (10 hrs) - Battle pages and results endpoints
10. 2v2 Feature Development (11 hrs) - Team-based match orchestration
11. Bug Fixes & Production Stabilization (15 hrs) - Edge case resolution and performance optimization
12. AWS Infrastructure & Automation (8 hrs) - Lambda setup and scheduled jobs

**Evidence sources:** Git commit history, file change logs, project documentation

### Aidan Sommer (SommAid) - 45 Hours
**Contributions (from README & project structure):**
- Database schema design and optimization
- UML diagram creation
- Frontend component rendering and state management
- QA/Testing execution and test report generation
- Network debugging and WebSocket optimization
- Multiplayer patch releases
- DevOps and cloud deployment configuration
- Key contributions logged in: `/assignments/AidanTimeLine.md`

**Work focused on:** Backend architecture, testing infrastructure, deployment pipelines

### Henock Dinberu (nbybhen) - 45+ Hours
**Contributions (from README & project structure):**
- Web IDE dependency research and evaluation (Sep 16 - Oct 25)
- UI component and icon library research (Sep 15 - Oct 15)
- Docker container setup partnership with Rukudzo (Oct 1 - Oct 31)
- Real-time WebSocket logic implementation (Nov 1 - Dec 30)
- Project branding and logo design (Oct 6 - Nov 30)
- Repository maintenance and pull request coordination
- Execution engine server configuration and optimization
- Key evidence: Initial project structure setup and repository administration

**Work focused on:** Infrastructure, WebSocket implementation, real-time features, project management

---

## E. Individual Contributions - Detailed File Evidence

### Rukudzo Mushunje - Key Modified Files
- `src/app/api/matchmaking/*` - All matchmaking routes (accept, decline, join-queue, leave-queue, worker)
- `src/app/competitive/page.tsx` - Competitive mode navigation
- `src/app/competitive/battle/[sessionId]/page.tsx` - Live battle interface
- `src/app/competitive/results/[sessionId]/page.tsx` - Match results display
- `src/lib/matchmakingCore.ts` - Core matchmaking logic
- `supabase/migrations/001_competitive_matchmaking.sql` - Database schema for matchmaking
- `infra/aws/matchmaking-worker-lambda.mjs` - AWS Lambda worker function
- `infra/aws/setup-matchmaking-scheduler.sh` - Infrastructure setup script
- `docs/COMPETITIVE_FEATURE.md` - Feature documentation

### Aidan Sommer - Key Modified Files
- `src/app/api/users/*` - User profile and sync endpoints
- `src/app/practice/[id]/page.tsx` - Practice mode interface
- `src/app/profile/*` - User profile pages and history
- Database migration files for schema optimization
- Frontend component rendering and state management
- Theme integration and UI polish

### Henock Dinberu - Key Modified Files
- Initial repository structure and setup
- `.gitignore` and configuration files
- `execution-engine/` directory files
- `execution-engine/Dockerfile` - Code execution containerization
- `src/components/` - Shared component library
- WebSocket integration and real-time logic

---

## F. Git Commit Statistics (Jan-Apr 2026)

### Rukudzo Mushunje Commits Sample
- **2026-04-09 01:55:01** - cron 2 (AWS scheduler updates)
- **2026-04-09 01:50:57** - cron job (matchmaking worker implementation)
- **2026-04-09 01:38:59** - fix #3 (competitive page bug)
- **2026-04-08 22:03:03** - fixed match making requeue bug
- **2026-04-06 20:36:12** - added notifications and fixed queue bugs
- **2026-03-29 20:04:50** - 2v2 functionality implementation
- **2026-02-15 22:31:33** - Competitive feature full implementation
- **2026-02-01 21:44:29** - added ui pages (login, practice, competitive)

**Total commits in sample:** 60+ with cumulative changes across 100+ files

---

## G. Testing & Quality Assurance Evidence

### Test Plan Documentation
- File: `/assignments/TestPlan.pdf`
- Covers: Unit tests, integration tests, user acceptance testing
- Includes: Test results, pass/fail metrics, bug tracking

### QA Phases
1. **Execution Engine Testing** - Timeout handling, output evaluation, error management
2. **Database Testing** - Schema optimization, query performance, data relationships
3. **MultiPlayer Testing** - WebSocket synchronization, match state consistency
4. **Competitive Mode Testing** - Matchmaking edge cases, queue logic, results calculation
5. **Production Testing** - Load testing, performance optimization, stability verification

---

## H. Deployment & Infrastructure

### Cloud Deployment
- **Frontend:** Deployed on Vercel
- **Backend API:** Next.js API routes on Vercel
- **Database:** Supabase (PostgreSQL instance)
- **Execution Engine:** Docker containers in AWS


## I. Professional Biographies

All team member biographies are included in the `/biographies` directory:
- **Aidan Sommer** - `Aidan-BIO.md` (frontend/web development focus)
- **Henock Dinberu** - `Henock-BIO.md` (infrastructure/DevOps focus)
- **Rukudzo Mushunje** - `Rukudzo-BIO.md` (backend/infrastructure focus)

---

## J. Project Launch & Results

### Completed Features
✓ User authentication via GitHub OAuth
✓ Practice mode with isolated code execution
✓ 1v1 competitive matchmaking
✓ 2v2 team-based competitive mode
✓ Real-time match updates via WebSocket
✓ User profiles and match history
✓ Ranking system and achievements
✓ Responsive UI across devices

### Production Status
- **Project Repository:** Live at https://github.com/nbybhen/CodeColosseum
- **Latest commits:** April 9, 2026
- **Active development:** Ongoing post-semester
- **Team:** Successfully transitioned from semester project to live platform

---

## K. Video/Presentation Evidence

### Spring Final PPT Presentation
- File: `/assignments/SpingFinalPPT`
- Includes: Project overview, technical architecture, live demo
- Presented: Spring 2026

### Expo Poster
- File: `/assignments/Poster.pdf`
- Includes: Project summary, key features, team information
- Format: Professional expo-ready poster

---

## L. Session History & Work Logs

### Documented Time Tracking
Each team member has maintained detailed hour logs with justifications:
- **Rukudzo Mushunje:** `/assignments/RukudzoTimeLine.md` (107 hours documented)
- **Aidan Sommer:** `/assignments/AidanTimeLine.md` (45 hours documented)
- **Henock Dinberu:** (Timeline pending - estimated 45+ hours)

### Evidence Sources
1. Git commit history with timestamps
2. File modification logs showing incrementally added features
3. Hours documented in individual timeline files
4. Pull request reviews and merge dates
5. Self-assessment documents with reflection on contributions

---

## M. Contact & Collaboration Information

### Team Members
- **Henock Dinberu** (Project Lead/DevOps):
  - GitHub: [@nbybhen](https://github.com/nbybhen)
  - Email: henockdinberu11@gmail.com
  
- **Aidan Sommer** (Frontend/QA):
  - GitHub: [@SommAid](https://github.com/SommAid)
  - Email: aidansommeriii@gmail.com
  
- **Rukudzo Mushunje** (Backend/Infrastructure):
  - GitHub: [@Ruklee13](https://github.com/Ruklee13)
  - Email: rukudzomushunje@gmail.com

### Project Advisor
- **Professor Giovanni** - UC Department of Computer Science

---

## N. Additional Resources

### Documentation Files
- User Manual: `/assignments/UserManual.md`
- Project Description: `/assignments/project-description.pdf`
- Test Plan: `/assignments/TestPlan.pdf`
- User Stories & Design: `/assignments/user-stories-and-design.pdf`
- ABET Concerns: `/assignments/ABET-concerns.pdf`

### Source Code Documentation
- Competitive Feature Docs: `/docs/COMPETITIVE_FEATURE.md`
- Database Migrations: `/supabase/migrations/`
- Infrastructure Setup: `/infra/aws/`

---

**Report Generated:** April 10, 2026
**Project Duration:** August 2025 - April 2026 (9 months)
**Status:** Final Design Report Complete
