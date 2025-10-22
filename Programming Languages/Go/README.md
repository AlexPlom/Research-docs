# Go Fast-Track Guide

Goal: reach comfortable productivity in Go within four focused weeks by combining hands-on coding with targeted theory.

## Prerequisites
- Basic command line familiarity.
- Working Git install (for cloning examples).
- Latest Go toolchain: download from [https://go.dev/dl/](https://go.dev/dl/) and verify with `go version`.

## Learning Roadmap
1. **Week 1 — Core Syntax & Tooling**
   - Work through [A Tour of Go](https://go.dev/tour/) (complete every exercise).
   - Read chapters 1–3 of *The Go Programming Language* (Kernighan & Donovan).
   - Practice: implement CLI utilities (`wordfreq`, `jsonfmt`) using `go run`.
2. **Week 2 — Concurrency Foundations**
   - Study goroutines and channels (Tour sections + Go doc guides).
   - Build a worker pool that fetches URLs concurrently and aggregates results.
   - Experiment with `context.Context` cancellation and timeouts.
3. **Week 3 — Building Services**
   - Follow the [Go Web Examples](https://gowebexamples.com/) tutorial.
   - Create a REST API using `net/http` with JSON handlers, middleware, and tests.
   - Add persistence via `database/sql` with SQLite or PostgreSQL.
4. **Week 4 — Testing & Deployment**
   - Deep dive into `testing` package, table-driven tests, benchmarks.
   - Integrate `golangci-lint` and `go test ./...` into a Makefile or task runner.
   - Containerize the Week 3 API with a multi-stage Dockerfile and run it locally.

## Daily Practice Template (45–90 min)
- 10 min: revisit notes / flashcards (key syntax, idioms).
- 20–40 min: implement or extend a micro-project feature.
- 10–20 min: read stdlib documentation relevant to today's work.
- 5 min: summarize what you learned in your personal log.

## Essential Commands
- `go fmt ./...` — format code consistently (run before commits).
- `go test ./... -run . -count=1` — execute all tests without caching.
- `go build ./cmd/<app>` — compile binaries; useful for smoke checking dependencies.
- `go doc <package>` — view local documentation quickly.

## Starter Projects
- `cmd/todo-cli` — terminal task tracker persisting to a JSON file.
- `cmd/feed-aggregator` — fetch multiple RSS feeds concurrently, expose combined JSON.
- `internal/pkg/validation` — write reusable validation helpers with unit tests.

## Reference & Community
- Official docs: [https://pkg.go.dev/std](https://pkg.go.dev/std)
- Style guide: [Go Code Review Comments](https://go.dev/wiki/CodeReviewComments)
- Exercises: [Exercism Go Track](https://exercism.org/tracks/go), [LeetCode Go tag](https://leetcode.com/problemset/?topicSlugs=golang)
- Talks/Playlists: JustForFunc (YouTube), GopherCon playlists.

## Next Steps After the Roadmap
- Contribute to a small open-source Go project (review issues labeled `good first issue`).
- Explore advanced topics: generics patterns, profiling (`pprof`), go modules in monorepos.
- Prepare for interviews: implement classic data structures and concurrency problems in Go.
