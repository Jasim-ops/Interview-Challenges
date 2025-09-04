# Interview-Challenges (MD JASIMUDDIN KHAN)
This is the interview challenges i hope like this code structure and code 
# Offline Task Management API

This backend project powers a personal task management app with offline support and sync capabilities.

## Features

- RESTful API for tasks
- SQLite database
- Sync support for offline operations
- Conflict resolution using "last-write-wins"
- Batch sync support
- Built with Express + Prisma + TypeScript

## API Endpoints

### Tasks

- `GET /api/tasks` - List all tasks
- `GET /api/tasks/:id` - Get a specific task
- `POST /api/tasks` - Create a task
- `PUT /api/tasks/:id` - Update a task
- `DELETE /api/tasks/:id` - Soft-delete a task

### Sync

- `POST /api/sync` - Sync local changes (create/update/delete)

## Setup

```bash
npm install
npx prisma migrate dev --name init
npm run dev

