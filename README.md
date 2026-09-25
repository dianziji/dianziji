# Shuo Yang

Full-stack engineer in New York — Next.js / TypeScript on the front, Python (FastAPI, Django) and PostgreSQL on the back. M.S. Computer Science, Tufts University.

I was an urban and landscape designer first. Three years on smart-city and headquarters projects taught me to think in systems, constraints, and the people who have to live inside what you build. I design software the same way.

**Open to work** — full-stack, backend, or AI-application roles · US work authorized, no sponsorship needed · [LinkedIn](https://www.linkedin.com/in/shuoyang89) · [shuo.yang@tufts.edu](mailto:shuo.yang@tufts.edu)

---

## Work

### [Prayer Walls](https://prayer-walls.com) — multi-tenant community platform
Organizations run a weekly prayer wall with roles, invitations, branding, and scoped analytics. Tenant isolation is enforced in Postgres with Supabase RLS; reads are pre-aggregated, per-user state is batched, and a k6 suite at 5–100 virtual users gates each release after a real Sunday outage. **100+ monthly active users across 10+ countries.**
`Next.js 15` `TypeScript` `Supabase` `PostgreSQL / PL/pgSQL` `TanStack Query` `Jest` `Playwright` `k6`
→ [architecture & incident write-up](https://github.com/dianziji/prayer-walls)

### [Bethel Renewal Center](https://bethelrc.org) — headless CMS rebuild
Migrated a legacy monolithic WordPress site to a headless architecture: Next.js frontend over WPGraphQL with typed query contracts, a normalization layer, ISR revalidation, and a ZH/EN bilingual pipeline with unified locale routing and field-level fallback. Defined the CPT/ACF schema and publishing SOP the editors now work from. GitHub Actions runs tests, lint, and build on every pull request and every push to main; a passing run on main triggers the Vercel deploy.
`Next.js` `TypeScript` `WPGraphQL` `GraphQL` `ISR` `WordPress` `GitHub Actions`
→ [source](https://github.com/dianziji/brc-web)

### [Bible Reference AI](https://github.com/dianziji/bible-reference-ai) — RAG scripture assistant
31,000+ KJV verses embedded into Pinecone; FastAPI service that moderates the question, retrieves with a score threshold, answers with GPT-4o constrained to the retrieved verses, and returns those verses as structured citations. Evaluated with Ragas on faithfulness and relevancy; Dockerized with Kubernetes manifests.
`FastAPI` `LangChain` `Pinecone` `OpenAI` `Ragas` `Next.js` `Docker` `Kubernetes`

### [MetaSpectra+ 3D Visualization](https://meta-imaging.qiguo.org/visualization) — scroll-driven WebGL paper walkthrough
Ten-scene React Three Fiber walkthrough of a hyperspectral camera paper for a Purdue research team. Scroll is the single source of truth; per-frame writes go straight to Three.js refs in ordered priority lanes, so animation costs zero React re-renders. Playwright visual regression made deterministic with SwiftShader. **Adopted as the paper's official visualization — CVPR 2026 Oral.**
`React` `Three.js` `React Three Fiber` `Zustand` `Vite` `Playwright`
→ [architecture write-up](https://github.com/dianziji/metaspectra-visualization)

### PosturePal — posture tracking and productivity app
Tufts M.S. capstone. Django REST backend for posture events, sessions, and longitudinal analytics; MediaPipe Pose inference pipeline for real-time feedback; guest vs. authenticated data scoping; frontend and backend containerized with Docker Compose.
`Django` `MediaPipe` `PostgreSQL` `Docker Compose`

### [SwiftUI Game of Life](https://github.com/dianziji/cs151Swift/tree/main/FinalProject) — iOS simulator
Interactive cellular-automaton simulator in SwiftUI, including a from-scratch SceneKit view that wraps the grid onto a 3D torus.
`Swift` `SwiftUI` `SceneKit`

---

## Stack

**Languages** TypeScript · JavaScript · Python · Swift · SQL · Java · C++
**Frontend** React · Next.js · Tailwind · React Three Fiber · SwiftUI
**Backend** FastAPI · Django REST Framework · Node.js · GraphQL · REST
**Data** PostgreSQL · Supabase · Pinecone · Redis · MongoDB
**Infra & tooling** Docker · Kubernetes · GitHub Actions · Vercel · Playwright · Jest · k6
**AI** OpenAI API · LangChain · RAG · Ragas
