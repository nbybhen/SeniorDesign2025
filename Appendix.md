# CS5002 Final Design Report - Appendix

Current site: https://dev.d2vzwbwt56tp2j.amplifyapp.com/

## A. References and Citations

### Technologies & Frameworks
- Next.js
- TypeScript
- Supabase
- Docker
- WebSocket
- Tailwind CSS
- GitHub
- AWS-related deployment tooling

### Code Repositories
- Main repository: https://github.com/nbybhen/CodeColosseum
- Current site: https://dev.d2vzwbwt56tp2j.amplifyapp.com/

### Key Directories
- `/src` - Application pages, routes, and components
- `/execution-engine` - Code execution service files
- `/supabase` - Database migrations and configuration
- `/infra` - Deployment and automation scripts

---

## B. Meeting Notes & Project Timeline

### Project Phases & Milestones

#### Phase 1: Research & Setup (Aug 26 - Oct 10, 2025)
- Team formation and meeting schedule
- Database and backend evaluation
- Supported language definition
- Web IDE and UI library research
- Containerization planning

#### Phase 2: Design & Prototyping (Oct 6 - Nov 30, 2025)
- Branding, logo, and landing page work
- Multiplayer UI design
- UX flow and component refinement

#### Phase 3: Implementation - Alpha Release (Nov 1 - Dec 30, 2025)
- Database schema and UML design
- Real-time communication logic
- User authentication integration
- Functional demo build

#### Phase 4: Post-Semester Development & Stabilization (Jan - Apr 2026)
- Competitive mode implementation
- Ranking and achievements updates
- 2v2 feature development
- Bug fixes and stability improvements
- Deployment and release updates

---

## C. Evidence of Hours & Effort Justification

### Aidan Sommer - 45 Hours
The export shows repeated work on authentication cleanup, rank updates, achievements, UI cleanup, and execution-engine package maintenance. His contribution level supports a 45-hour allocation because the work spans design polish, bug fixes, and release stabilization rather than a single narrow feature.

### Henock Dinberu - 45 Hours
The export shows work across homepage setup, friends and social features, practice-page updates, login fixes, execution-engine work, Dockerfile changes, custom room logic, and build/debug fixes. Those commits justify a 45-hour allocation across research, UI, and infrastructure maintenance.

### Rukudzo Mushunje - 45 Hours
The export shows concentrated work on competitive pages, match results, matchmaking route fixes, 2v2 logic, queue handling, and production bug fixes. This is the highest-density implementation area in the repo and supports a 45-hour allocation for backend and feature integration work.

---

## D. Individual Contributions - Detailed File Evidence

### Rukudzo Mushunje
- `src/app/api/matchmaking/join-queue/route.ts`
- `src/app/api/matchmaking/accept/route.ts`
- `src/app/api/matchmaking/decline/route.ts`
- `src/app/api/match/[sessionId]/route.ts`
- `src/app/api/match/[sessionId]/submit/route.ts`
- `src/app/api/match/[sessionId]/results/route.ts`
- `src/app/competitive/page.tsx`
- `src/app/competitive/battle/[sessionId]/page.tsx`
- `src/app/competitive/results/[sessionId]/page.tsx`
- `src/lib/matchmakingCore.ts`

### Aidan Sommer
- `src/app/auth/callback/route.ts`
- `src/app/competitive/page.tsx`
- `src/app/profile/*`
- `src/app/practice/*`
- `src/components/*` for UI polish and rank/achievement updates
- `execution-engine/package.json`
- `execution-engine/server.js`

### Henock Dinberu
- `src/app/page.tsx` and homepage-related updates
- `src/components/FriendsSidebar.tsx`
- `src/components/LoginWithGithub.tsx`
- `src/app/practice/[id]/page.tsx`
- `src/app/practice/page.tsx`
- `execution-engine/Dockerfile`
- `src/components/*` for shared UI and integration work

---

## E. Git Commit Statistics (Jan-Apr 2026)

### Exported Activity
- Aidan Sommer: 44 commits
- Henock Dinberu / nbybhen: 43 commits combined
- Rukudzo Mushunje / RKO: 42 commits combined
- Total tracked author activity in the export: 129 commits

### Representative Commit Themes
- Authentication redirect fixes and login cleanup
- Ranking, achievements, and profile updates
- Competitive mode and 2v2 matchmaking work
- Practice-page UI and execution-engine fixes
- Build cleanup and repo maintenance

---

## F. Testing & Quality Assurance Evidence

### Test Plan Documentation
- File: `/assignments/TestPlan.pdf`
- Covers unit testing, integration testing, and user acceptance testing

### QA Focus Areas
1. Execution engine behavior and runtime handling
2. Authentication and user profile flows
3. Competitive mode and queue logic
4. Results and ranking behavior
5. UI cleanup and production readiness

---

## G. Deployment & Infrastructure

### Current Deployment
- Frontend and live preview: https://dev.d2vzwbwt56tp2j.amplifyapp.com/
- Repository source: https://github.com/nbybhen/CodeColosseum
- Database and backend support: Supabase and Next.js API routes

### Project Notes
- Do not cite unimplemented matchmaking Lambda functionality as part of the final deliverable.
- Keep deployment language limited to what is visible in the repo and exported history.

---

## H. Professional Biographies

All team member biographies are included in the `/biographies` directory:
- Aidan Sommer - `Aidan-BIO.md`
- Henock Dinberu - `Henock-BIO.md`
- Rukudzo Mushunje - `Rukudzo-BIO.md`

---

## I. Project Launch & Results

### Completed Features
- User authentication via GitHub OAuth
- Practice mode with isolated code execution
- Competitive mode and matchmaking flows
- 2v2 team-based competitive mode
- Ranking and achievements updates
- User profiles and history views
- Responsive UI work and cleanup

### Production Status
- Current site: https://dev.d2vzwbwt56tp2j.amplifyapp.com/
- Active repository: https://github.com/nbybhen/CodeColosseum

---

## J. Video/Presentation Evidence

### Spring Final PPT Presentation
- File: `/assignments/SpingFinalPPT`

### Expo Poster
- File: `/assignments/Poster.pdf`

---

## K. Session History & Work Logs

### Documented Time Tracking
- Aidan Sommer: `/assignments/AidanTimeLine.md`
- Rukudzo Mushunje: `/assignments/RukudzoTimeLine.md`
- Henock Dinberu: hours justified in this appendix from the exported commit history

### Evidence Sources
1. Git commit export in `/exports/changes_all-authors_2026-01-01_to_2026-04-10.csv`
2. Export summary in `/exports/changes_all-authors_2026-01-01_to_2026-04-10.md`
3. Individual timeline files
4. Self-assessment documents
5. Repository file history and merge activity

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
