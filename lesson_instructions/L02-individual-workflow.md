# Meeting 2 — Capstone introduction, preparation review and first requirements specification

## Course capstone: event photographer platform
A photographer manages events and photographs. Clients access their event gallery and select images or services. This lesson introduces the product *at a high level only*. Lesson 3 covers deeper repository archaeology and code tracing.

## Preparation assignment — bring your questions
You were asked to choose a task you had received and write **one question for each** of: functional requirements, non-functional requirements, actors/users, use cases, constraints, assumptions, acceptance criteria, ambiguity, missing information, and scope.

In class: share two questions with a partner. Discuss what the answer would change and whether the question embeds an unverified assumption. Reuse the ten lenses later for the event-title change request.

## GitHub and first run
1. Open the public GitHub repository URL provided by the instructor. Click **Fork** into your own GitHub account.
2. Clone **your fork** locally using `git clone <YOUR_FORK_URL>`; a downloaded ZIP is not a fork.
3. Read `README.md`. Check `node --version` and `npm --version`.
4. Run `npm install`, `npm test`, `npm run typecheck`, and `npm run dev`.
5. Check `http://localhost:3000/health`; if runtime fails, document the error and mark execution unverified.

## First discovery — not deep archaeology
Find the README, `src/domain/types.ts`, `src/data/memory-store.ts`, `src/services/event-service.ts`, `src/http/app.ts`, and `tests/event-api.test.ts`. Record **three verified observations** (file/function/line or actual HTTP output). Your job is to find where an event title exists and whether the client gallery returns it. Do **not** comprehensively trace flows or change code; that is for the next lessons.

### AI checkpoint 1: understanding
Only after reading the README and at least one relevant source file: ask AI to explain a function you provide and suggest *one* other file worth checking. Check its claims against the repository.

## Feature request (no implementation)
> “I entered the wrong event name. I want to change the name displayed in my client's gallery.”

First, independently write at least five questions. Then use **all ten analysis terms** from the prep assignment as lenses: which questions are essential, which have no known answer, and which requirements are only assumptions?

### AI checkpoint 2: questioning
Ask AI to suggest essential/deferrable questions and unsupported assumptions **from the request and the repository facts you provide**. Compare against your own questions. Do not let AI invent decisions, architecture, code facts, or requirements.

## Specification
Copy `docs/requirements-event-title.template.md` to `docs/requirements-event-title.md`. Record original wording, verified behavior, actors, use cases, scope, functional and non-functional requirements, constraints, ambiguity, assumptions, missing information, and acceptance criteria. Mark undecided items as **open**, not decided.

### AI checkpoint 3: spec review
Ask AI to review *your draft* for unsupported assumptions, inconsistencies and untestable acceptance criteria. Classify suggestions as adopted / rejected / open with a reason. No feature implementation or Pull Request is required.
