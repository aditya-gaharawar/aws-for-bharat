# System Requirements Document  
CognitiveStack AI

---

# 1. Functional Requirements

## 1.1 User Management
- User registration & authentication
- Secure password storage
- JWT session management

## 1.2 Goal Management
- User can input learning goal
- User can specify time constraint
- System generates skill graph

## 1.3 Skill Graph Engine
- DAG-based skill modeling
- Dependency tracking
- Unlock logic

## 1.4 Learning Session
- Micro-lesson delivery
- One exercise per screen
- Deterministic answer validation
- Instant feedback

## 1.5 Mastery Engine
- Track accuracy
- Track response time
- Track retries
- Compute mastery score
- Persist mastery history

## 1.6 Adaptive Difficulty
- Increase complexity on high accuracy
- Decrease difficulty on repeated failure
- Change hint depth dynamically

## 1.7 AI Generation
- Structured exercise generation
- Strict JSON schema enforcement
- Multiple exercise types

## 1.8 Validation Layer
- Cross-model verification
- Retrieval grounding
- Confidence threshold enforcement

## 1.9 Analytics
- Session tracking
- Failure clustering
- Learning velocity
- Time-to-mastery estimation

---

# 2. Non-Functional Requirements

## 2.1 Performance
- Response time < 2 seconds
- AI generation < 1.5 seconds
- Validation < 1 second

## 2.2 Scalability
- Stateless services
- Auto-scaling backend
- Horizontal database scaling

## 2.3 Security
- JWT authentication
- Input validation
- Rate limiting
- Encryption at rest

## 2.4 Reliability
- 99% uptime (MVP target)
- Graceful AI fallback
- Logging & monitoring

## 2.5 Responsible AI
- No raw AI output without validation
- Transparent reasoning
- User data deletion option

---

# 3. Constraints

- Hackathon timeline
- Limited compute budget
- MVP scope
- Single domain focus initially

---

# 4. Assumptions

- Developers are primary users
- AI models available via AWS Bedrock
- Deterministic exercise formats only
