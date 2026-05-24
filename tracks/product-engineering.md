# 🏭 Product Engineering Building Cloud-Native Applications

> From idea to production. Frontend, backend, DevOps the full product lifecycle.

---

## 🎯 What This Covers

Building a real product end-to-end:
1. Design the system
2. Build the frontend
3. Build the backend
4. Set up CI/CD
5. Deploy to cloud
6. Monitor & iterate

---

## 🎨 Frontend Engineering

### Courses

| Course | Platform | Link |
|--------|----------|------|
| Full Stack Open (React + Node) | University of Helsinki (free) | [fullstackopen.com](https://fullstackopen.com/en/) |
| The Odin Project | Free Curriculum | [theodinproject.com](https://www.theodinproject.com/) |
| React Official Tutorial | React Docs | [react.dev/learn](https://react.dev/learn) |
| Next.js Learn | Vercel (free) | [nextjs.org/learn](https://nextjs.org/learn) |
| CSS for JS Developers (free parts) | Josh Comeau | [joshwcomeau.com](https://www.joshwcomeau.com/css/) |

### Key Skills

| Skill | Resource | Link |
|-------|----------|------|
| Component Architecture | Atomic Design | [atomicdesign.bradfrost.com](https://atomicdesign.bradfrost.com/) |
| State Management | Redux/Zustand docs | [redux.js.org](https://redux.js.org/) |
| Accessibility (a11y) | web.dev Learn Accessibility | [web.dev/learn/accessibility](https://web.dev/learn/accessibility) |
| Performance | Core Web Vitals | [web.dev/vitals](https://web.dev/vitals/) |
| Design Systems | Storybook | [storybook.js.org](https://storybook.js.org/) |
| Responsive Design | MDN | [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design) |

### UI Frameworks (Free/Open Source)

| Framework | Link |
|-----------|------|
| Tailwind CSS | [tailwindcss.com](https://tailwindcss.com/) |
| shadcn/ui | [ui.shadcn.com](https://ui.shadcn.com/) |
| Radix UI | [radix-ui.com](https://www.radix-ui.com/) |
| Material UI | [mui.com](https://mui.com/) |

---

## ⚙️ Backend Engineering

### Courses

| Course | Platform | Link |
|--------|----------|------|
| CS50 Web Programming (Django) | Harvard OCW | [cs50.harvard.edu/web](https://cs50.harvard.edu/web/) |
| Full Stack Open (Node.js) | Helsinki (free) | [fullstackopen.com](https://fullstackopen.com/en/) |
| Microservices with Node.js | YouTube (freeCodeCamp) | [YouTube](https://www.youtube.com/watch?v=XUSHH0E-7zk) |
| System Design for Backend | ByteByteGo | [youtube.com/@ByteByteGo](https://www.youtube.com/@ByteByteGo) |

### Architecture Patterns

| Pattern | When | Resource |
|---------|------|----------|
| Monolith | MVP, small team | Start here always |
| Microservices | Scale, team autonomy | [microservices.io](https://microservices.io/) |
| Event-Driven | Async workflows | [YouTube](https://www.youtube.com/results?search_query=event+driven+architecture) |
| CQRS | Read/write separation | [martinfowler.com/bliki/CQRS](https://martinfowler.com/bliki/CQRS.html) |
| Serverless | Event-triggered, low traffic | [serverless.com](https://www.serverless.com/) |

### Best Practices

| Practice | Resource | Link |
|----------|----------|------|
| 12-Factor App | Cloud-native principles | [12factor.net](https://12factor.net/) |
| API Design (Google) | REST/gRPC guidelines | [cloud.google.com/apis/design](https://cloud.google.com/apis/design) |
| Database Migrations | Flyway / Alembic | [flywaydb.org](https://flywaydb.org/) |
| Error Handling | Patterns | [YouTube](https://www.youtube.com/results?search_query=error+handling+best+practices+backend) |
| Authentication | OAuth2 / OIDC | [oauth.net/2](https://oauth.net/2/) |

---

## 🚀 DevOps & Deployment

→ *See [Cloud Track](cloud-devops.md) for full details*

### CI/CD Pipeline (Typical)

```
Code Push → Lint → Test → Build → Container → Deploy Staging → E2E Test → Deploy Prod
```

| Stage | Tool | Link |
|-------|------|------|
| CI | GitHub Actions | [docs.github.com/en/actions](https://docs.github.com/en/actions) |
| Containerize | Docker | [docs.docker.com](https://docs.docker.com/) |
| Orchestrate | Kubernetes | [kubernetes.io/docs](https://kubernetes.io/docs/) |
| IaC | Terraform | [developer.hashicorp.com/terraform](https://developer.hashicorp.com/terraform) |
| GitOps | ArgoCD | [argo-cd.readthedocs.io](https://argo-cd.readthedocs.io/) |
| Monitor | Prometheus + Grafana | [prometheus.io](https://prometheus.io/) |

### Deployment Strategies

| Strategy | Risk | Use When |
|----------|------|----------|
| Blue-Green | Low | Zero-downtime required |
| Canary | Low | Gradual rollout, catch regressions |
| Rolling | Medium | Default K8s strategy |
| Feature Flags | Lowest | Decouple deploy from release |

---

## 📐 Product Design & UX (for Engineers)

| Resource | Link |
|----------|------|
| Laws of UX | [lawsofux.com](https://lawsofux.com/) |
| Refactoring UI (free tips) | [refactoringui.com](https://www.refactoringui.com/) |
| Nielsen Norman Group (articles) | [nngroup.com/articles](https://www.nngroup.com/articles/) |
| Design for Developers (YouTube) | [YouTube](https://www.youtube.com/results?search_query=design+for+developers) |

---

## 📋 The Product Engineering Checklist

```
□ Requirements documented (PRD or RFC)
□ System design reviewed
□ API contract defined (OpenAPI spec)
□ Database schema designed
□ Auth strategy chosen (JWT/OAuth/Session)
□ Frontend scaffolded with design system
□ Backend with health checks, logging, metrics
□ CI/CD pipeline (lint → test → build → deploy)
□ Staging environment mirrors production
□ Monitoring & alerting configured
□ Error tracking (Sentry or equivalent)
□ Load testing done before launch
□ Security review (OWASP Top 10)
□ Documentation (README, API docs, runbook)
□ Feature flags for safe rollout
```

---

*Cross-references: [Cloud Track](cloud-devops.md) · [Web Track](web-development.md) · [System Design](interview-prep.md#-system-design) · [AI-Era Essentials](../subjects/ai-era-essentials.md)*
