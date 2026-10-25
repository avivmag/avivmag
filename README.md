### Hi, I'm Aviv 👋

Senior software engineer working in Go, distributed systems and AWS. Since 2019 I have designed and built, solo, the backend, infrastructure and clients of a real-time multiplayer social game platform (pre-launch). Before that I was at Google on account-security notifications, and I hold a B.Sc. in Software Engineering from Ben-Gurion University (highest honours, 3rd of 83).

**What I've built**

- **Go backend:** 18 microservices on AWS (~127k lines of production Go), with gRPC between services, SNS/SQS events, DynamoDB, a self-managed Elasticsearch cluster and X-Ray tracing.
- **Real-time gateway:** long-lived WebSocket and TCP connections routing 60+ Protocol Buffers message types to the backend services, with per-connection backpressure and updates pushed only to the clients viewing the changed data.
- **Sharding:** application-level sharding for stateful in-memory services: 240 logical shards, a versioned shard-to-instance map in DynamoDB and ownership checks on every call.
- **Infrastructure as code:** AWS CDK for staging and production (ECS, a Network Load Balancer, ~90 SNS topics fanned out to SQS, least-privilege IAM), plus a local environment that runs every service in one process against LocalStack.
- **Clients:** Android, iOS and web on one Kotlin Multiplatform core, with Compose Multiplatform and SwiftUI.
- **AI-directed engineering (2026):** a multi-agent pipeline in which Claude and Codex coding agents work in isolated git worktrees, read-only sessions review their changes, and a test, race-detector, static-analysis and secret-scanning gate decides what reaches my review.

That codebase is private. The public repositories here are a 2026 hackathon prototype and my university coursework (operating systems, compilers, concurrency).

**Stack:** Go · Kotlin · Swift · TypeScript · Java · gRPC · Protocol Buffers · WebSockets · DynamoDB · Elasticsearch · SNS/SQS · AWS (ECS, Lambda, Cloud Map, CloudFront, IAM) · AWS CDK · Docker · Claude Code · Codex

**Also:** websites for two family-run businesses, [lisa.org.il](https://lisa.org.il) and [magnezy.co.il](https://magnezy.co.il).

📍 Netanya, Israel, relocating to Cyprus in January 2027 · [LinkedIn](https://www.linkedin.com/in/aviv-magnezy)
