# Full Stack JavaScript Interview Preparation Checklist
### For 3+ Years Experience | React • Node.js • MongoDB • System Design

---

## Table of Contents
- [JavaScript Deep Dive](#javascript-deep-dive)
- [React In-Depth](#react-in-depth)
- [Node.js Mastery](#nodejs-mastery)
- [MongoDB & Database Design](#mongodb--database-design)
- [System Design - Frontend](#system-design---frontend)
- [System Design - Backend](#system-design---backend)
- [Common Interview Questions](#common-interview-questions)

---

## JavaScript Deep Dive

### ✅ Core Concepts (How Things Work Internally)

#### **Execution Context & Call Stack**
- [ ] Global Execution Context
- [ ] Function Execution Context
- [ ] Execution Context phases (Creation & Execution)
- [ ] Call Stack mechanism
- [ ] Stack Overflow scenarios

#### **Hoisting**
- [ ] Variable hoisting (var, let, const)
- [ ] Function hoisting
- [ ] Temporal Dead Zone (TDZ)
- [ ] Interview Question: Predict output of hoisting scenarios

#### **Scope & Scope Chain**
- [ ] Global Scope
- [ ] Function Scope
- [ ] Block Scope
- [ ] Lexical Scope
- [ ] Scope Chain lookup mechanism
- [ ] Interview Question: Nested function scope resolution

#### **Closures** ⭐
- [ ] What is a closure and how it works
- [ ] Closure use cases (data privacy, currying, memoization)
- [ ] Module pattern using closures
- [ ] Common pitfalls (loop + closure with var)
- [ ] Memory implications of closures
- [ ] Interview Question: Create a counter using closures
- [ ] Interview Question: setTimeout in loop problem

#### **Prototype & Prototypal Inheritance** ⭐
- [ ] `__proto__` vs `prototype`
- [ ] Prototype chain mechanism
- [ ] Constructor functions
- [ ] Object.create() for inheritance
- [ ] ES6 Classes (syntactic sugar over prototypes)
- [ ] Inheritance patterns (Prototypal, Classical, Functional)
- [ ] hasOwnProperty vs in operator
- [ ] Interview Question: Implement custom inheritance
- [ ] Interview Question: Difference between `__proto__` and `prototype`

#### **this Keyword** ⭐
- [ ] Default binding
- [ ] Implicit binding
- [ ] Explicit binding (call, apply, bind)
- [ ] new binding
- [ ] Arrow functions and this
- [ ] this in different contexts (global, object method, class)
- [ ] Interview Question: Predict this value in various scenarios

#### **Event Loop & Asynchronous JavaScript** ⭐
- [ ] Call Stack
- [ ] Web APIs / Browser APIs
- [ ] Callback Queue (Task Queue)
- [ ] Microtask Queue (Job Queue)
- [ ] Event Loop mechanism
- [ ] Macro tasks vs Micro tasks
- [ ] Promise execution order
- [ ] async/await internal working
- [ ] Interview Question: Predict output of setTimeout, Promise, async/await mix

#### **Promises** ⭐
- [ ] Promise states (pending, fulfilled, rejected)
- [ ] Promise chaining
- [ ] Error handling (catch, try/catch)
- [ ] Promise.all(), Promise.race(), Promise.allSettled(), Promise.any()
- [ ] Creating custom Promises
- [ ] Interview Question: Implement Promise.all()
- [ ] Interview Question: Sequential vs Parallel execution

#### **async/await**
- [ ] How async/await works internally
- [ ] Error handling with try/catch
- [ ] async/await vs Promises
- [ ] Top-level await
- [ ] Interview Question: Convert Promise chain to async/await

### ✅ Advanced Concepts

#### **Currying**
- [ ] What is currying
- [ ] Implementing curry function
- [ ] Partial application
- [ ] Use cases in real applications

#### **Debouncing & Throttling** ⭐
- [ ] Debounce implementation
- [ ] Throttle implementation
- [ ] Use cases and differences
- [ ] Interview Question: Implement custom debounce/throttle

#### **Memoization**
- [ ] Concept and use cases
- [ ] Implementing memoization function
- [ ] React.memo, useMemo relation

#### **Function Composition & Pipe**
- [ ] compose() implementation
- [ ] pipe() implementation
- [ ] Functional programming basics

#### **Deep Copy vs Shallow Copy**
- [ ] Spread operator limitations
- [ ] Object.assign() limitations
- [ ] structuredClone()
- [ ] JSON.parse/stringify method
- [ ] Custom deep clone implementation
- [ ] Interview Question: Deep clone an object with circular references

#### **Polyfills** ⭐
- [ ] map() polyfill
- [ ] filter() polyfill
- [ ] reduce() polyfill
- [ ] bind() polyfill
- [ ] call() & apply() polyfill
- [ ] Promise polyfill (basic)
- [ ] Interview Question: Write polyfill for Array methods

#### **Memory Management**
- [ ] Garbage Collection
- [ ] Memory Leaks (common causes)
- [ ] WeakMap and WeakSet
- [ ] Reference counting

#### **Design Patterns**
- [ ] Singleton Pattern
- [ ] Factory Pattern
- [ ] Observer Pattern (Pub-Sub)
- [ ] Module Pattern
- [ ] Revealing Module Pattern
- [ ] Prototype Pattern

#### **ES6+ Features**
- [ ] Destructuring (array, object)
- [ ] Spread & Rest operators
- [ ] Template literals
- [ ] Arrow functions
- [ ] Default parameters
- [ ] Enhanced object literals
- [ ] Symbols
- [ ] Iterators & Generators
- [ ] Map, Set, WeakMap, WeakSet
- [ ] Proxy & Reflect
- [ ] Optional Chaining (?.)
- [ ] Nullish Coalescing (??)

#### **Error Handling**
- [ ] try/catch/finally
- [ ] Custom Error classes
- [ ] Error propagation
- [ ] Global error handlers

---

## React In-Depth

### ✅ Core Concepts (How React Works Internally)

#### **Virtual DOM & Reconciliation** ⭐
- [ ] What is Virtual DOM
- [ ] Diffing Algorithm
- [ ] Reconciliation process
- [ ] Fiber Architecture (React 16+)
- [ ] Keys in lists (why keys matter)
- [ ] Interview Question: Explain Virtual DOM vs Real DOM

#### **Component Lifecycle** ⭐
- [ ] Class component lifecycle methods
  - [ ] Mounting: constructor, render, componentDidMount
  - [ ] Updating: shouldComponentUpdate, render, componentDidUpdate
  - [ ] Unmounting: componentWillUnmount
- [ ] getDerivedStateFromProps
- [ ] componentDidCatch (Error Boundaries)
- [ ] Lifecycle in functional components (hooks)

#### **React Hooks** ⭐⭐
- [ ] **useState**
  - [ ] How state updates work (batching)
  - [ ] Functional updates
  - [ ] Lazy initialization
- [ ] **useEffect**
  - [ ] How useEffect works internally
  - [ ] Dependency array
  - [ ] Cleanup function
  - [ ] useEffect vs useLayoutEffect
- [ ] **useContext**
  - [ ] Creating and consuming context
  - [ ] Context performance issues
- [ ] **useReducer**
  - [ ] When to use vs useState
  - [ ] Implementing complex state logic
- [ ] **useCallback**
  - [ ] Memoizing functions
  - [ ] Dependency array
- [ ] **useMemo**
  - [ ] Memoizing expensive computations
  - [ ] When to use
- [ ] **useRef**
  - [ ] Accessing DOM elements
  - [ ] Storing mutable values
  - [ ] useRef vs useState
- [ ] **useLayoutEffect**
  - [ ] Difference from useEffect
  - [ ] Use cases (measuring DOM, preventing flicker)
- [ ] **useImperativeHandle**
- [ ] **Custom Hooks**
  - [ ] Creating reusable hooks
  - [ ] Best practices
  - [ ] Interview Question: Build custom hooks (useDebounce, useFetch, useLocalStorage)

#### **State Management** ⭐
- [ ] Lifting state up
- [ ] Prop drilling problem
- [ ] Context API (when to use, limitations)
- [ ] Redux
  - [ ] Store, Actions, Reducers
  - [ ] Middleware (redux-thunk, redux-saga)
  - [ ] Redux Toolkit
- [ ] Zustand / Recoil / Jotai (alternative solutions)
- [ ] Interview Question: When to use Context vs Redux

#### **Performance Optimization** ⭐
- [ ] React.memo()
- [ ] useMemo vs useCallback
- [ ] Code splitting (React.lazy, Suspense)
- [ ] Virtualization (react-window, react-virtualized)
- [ ] Avoiding unnecessary re-renders
- [ ] Profiler API
- [ ] Bundle size optimization
- [ ] Interview Question: Debug performance issues

#### **Rendering Behavior**
- [ ] Render phase vs Commit phase
- [ ] Batching updates
- [ ] Concurrent Rendering (React 18)
- [ ] Automatic batching
- [ ] useTransition
- [ ] useDeferredValue

#### **React Patterns**
- [ ] Higher Order Components (HOC)
- [ ] Render Props
- [ ] Compound Components
- [ ] Controlled vs Uncontrolled Components
- [ ] Container/Presentational Pattern

#### **Error Handling**
- [ ] Error Boundaries
- [ ] Implementing error boundaries
- [ ] Fallback UI

#### **React Router**
- [ ] BrowserRouter vs HashRouter
- [ ] Route matching and rendering
- [ ] Nested routes
- [ ] Protected routes
- [ ] Programmatic navigation
- [ ] useParams, useNavigate, useLocation

#### **Forms & Validation**
- [ ] Controlled components
- [ ] Uncontrolled components (useRef)
- [ ] Form libraries (Formik, React Hook Form)
- [ ] Validation strategies

#### **Server-Side Rendering (SSR)**
- [ ] Next.js basics
- [ ] getServerSideProps, getStaticProps
- [ ] Hydration
- [ ] SEO benefits

#### **Testing**
- [ ] Jest basics
- [ ] React Testing Library
- [ ] Testing hooks
- [ ] Mocking in tests

---

## Node.js Mastery

### ✅ Core Concepts (How Node.js Works Internally)

#### **Event Loop** ⭐⭐
- [ ] How Node.js event loop works
- [ ] Phases of event loop:
  - [ ] Timers
  - [ ] Pending callbacks
  - [ ] Idle, prepare
  - [ ] Poll
  - [ ] Check
  - [ ] Close callbacks
- [ ] process.nextTick()
- [ ] setImmediate() vs setTimeout()
- [ ] Microtasks vs Macrotasks in Node
- [ ] Interview Question: Predict execution order

#### **Streams** ⭐
- [ ] Types: Readable, Writable, Duplex, Transform
- [ ] Stream events
- [ ] Backpressure handling
- [ ] Piping streams
- [ ] Use cases (file processing, large data)
- [ ] Interview Question: Process large files using streams

#### **Buffer**
- [ ] What is Buffer
- [ ] Creating buffers
- [ ] Buffer vs String
- [ ] Buffer operations

#### **Cluster & Child Processes** ⭐
- [ ] Cluster module for multi-core utilization
- [ ] Worker threads
- [ ] child_process (fork, spawn, exec)
- [ ] PM2 for process management
- [ ] Interview Question: Scale Node.js application

#### **Event Emitters**
- [ ] Creating custom event emitters
- [ ] on(), once(), emit()
- [ ] removeListener()
- [ ] Use cases

#### **Middleware** ⭐
- [ ] How middleware works in Express
- [ ] Creating custom middleware
- [ ] Error handling middleware
- [ ] Order of middleware execution

#### **Authentication & Authorization** ⭐
- [ ] JWT (JSON Web Tokens)
  - [ ] Creating and verifying JWT
  - [ ] Token storage (httpOnly cookies)
  - [ ] Refresh tokens
- [ ] Session-based auth
- [ ] OAuth 2.0 / Social login
- [ ] Role-based access control (RBAC)
- [ ] Interview Question: Implement JWT auth

#### **Security Best Practices** ⭐
- [ ] CORS
- [ ] Helmet.js
- [ ] Rate limiting
- [ ] Input validation & sanitization
- [ ] SQL Injection prevention
- [ ] XSS prevention
- [ ] CSRF protection
- [ ] Environment variables (.env)
- [ ] Secrets management

#### **RESTful API Design** ⭐
- [ ] REST principles
- [ ] HTTP methods (GET, POST, PUT, PATCH, DELETE)
- [ ] Status codes (2xx, 3xx, 4xx, 5xx)
- [ ] API versioning
- [ ] Pagination
- [ ] Filtering, sorting
- [ ] HATEOAS

#### **GraphQL**
- [ ] GraphQL vs REST
- [ ] Schema definition
- [ ] Resolvers
- [ ] Queries and Mutations
- [ ] Apollo Server

#### **WebSockets**
- [ ] Socket.io basics
- [ ] Real-time communication
- [ ] Rooms and namespaces
- [ ] Scaling WebSocket servers

#### **Caching** ⭐
- [ ] In-memory caching
- [ ] Redis integration
- [ ] Cache invalidation strategies
- [ ] CDN caching

#### **Testing**
- [ ] Jest / Mocha / Chai
- [ ] Supertest for API testing
- [ ] Unit tests
- [ ] Integration tests
- [ ] Mocking dependencies

#### **Error Handling** ⭐
- [ ] Try/catch in async/await
- [ ] Centralized error handling
- [ ] Custom error classes
- [ ] Logging (Winston, Morgan)
- [ ] Error monitoring (Sentry)

#### **Performance Optimization**
- [ ] Profiling Node.js apps
- [ ] Memory leak detection
- [ ] CPU profiling
- [ ] Optimizing V8 garbage collection

#### **Package Management**
- [ ] npm vs yarn vs pnpm
- [ ] package.json vs package-lock.json
- [ ] Semantic versioning
- [ ] Creating npm packages

---

## MongoDB & Database Design

### ✅ MongoDB Deep Dive

#### **Core Concepts**
- [ ] Documents and Collections
- [ ] BSON format
- [ ] ObjectId generation

#### **CRUD Operations** ⭐
- [ ] insertOne, insertMany
- [ ] find, findOne
- [ ] updateOne, updateMany, replaceOne
- [ ] deleteOne, deleteMany
- [ ] Bulk operations

#### **Querying** ⭐
- [ ] Query operators ($eq, $gt, $gte, $in, $nin, etc.)
- [ ] Logical operators ($and, $or, $not, $nor)
- [ ] Element operators ($exists, $type)
- [ ] Array operators ($all, $elemMatch, $size)
- [ ] Projection
- [ ] Sorting and limiting

#### **Indexing** ⭐⭐
- [ ] What are indexes and why they matter
- [ ] Single field indexes
- [ ] Compound indexes
- [ ] Multikey indexes
- [ ] Text indexes
- [ ] Geospatial indexes
- [ ] Index properties (unique, sparse, TTL)
- [ ] explain() for query analysis
- [ ] Interview Question: When to use indexes, trade-offs

#### **Aggregation Pipeline** ⭐⭐
- [ ] $match
- [ ] $group
- [ ] $project
- [ ] $sort, $limit, $skip
- [ ] $lookup (joins)
- [ ] $unwind
- [ ] $addFields
- [ ] $bucket
- [ ] Pipeline optimization
- [ ] Interview Question: Complex aggregation queries

#### **Data Modeling** ⭐
- [ ] Embedded documents vs References
- [ ] One-to-One relationships
- [ ] One-to-Many relationships
- [ ] Many-to-Many relationships
- [ ] Denormalization strategies
- [ ] Schema design patterns
- [ ] Interview Question: Design schema for e-commerce app

#### **Transactions**
- [ ] ACID properties in MongoDB
- [ ] Multi-document transactions
- [ ] Session management
- [ ] Read/Write concerns

#### **Replication** ⭐
- [ ] Replica sets
- [ ] Primary and Secondary nodes
- [ ] Election process
- [ ] Oplog
- [ ] Read preference

#### **Sharding**
- [ ] Horizontal scaling
- [ ] Shard keys
- [ ] Chunk distribution
- [ ] Zone sharding

#### **Performance Optimization** ⭐
- [ ] Query optimization
- [ ] Index strategies
- [ ] Monitoring with mongostat, mongotop
- [ ] Profiler
- [ ] Connection pooling

#### **Mongoose (ODM)** ⭐
- [ ] Schema definition
- [ ] Models
- [ ] Validation
- [ ] Middleware (pre, post hooks)
- [ ] Population (references)
- [ ] Virtual properties
- [ ] Query helpers

---

## System Design - Frontend

### ✅ Architecture Patterns

#### **Component Architecture**
- [ ] Atomic Design (Atoms, Molecules, Organisms)
- [ ] Feature-based folder structure
- [ ] Reusable component design

#### **State Management Architecture** ⭐
- [ ] Local vs Global state
- [ ] State normalization
- [ ] State machines (XState)
- [ ] Server state vs Client state

#### **Routing Architecture**
- [ ] Client-side routing
- [ ] Code splitting by routes
- [ ] Protected routes pattern
- [ ] Deep linking

#### **API Layer Design** ⭐
- [ ] API client abstraction
- [ ] Request/Response interceptors
- [ ] Error handling layer
- [ ] Retry mechanisms
- [ ] API caching strategies

### ✅ Performance Optimization

#### **Loading Performance** ⭐⭐
- [ ] Code splitting
- [ ] Lazy loading components
- [ ] Tree shaking
- [ ] Bundle analysis
- [ ] Critical CSS
- [ ] Resource hints (preload, prefetch, preconnect)
- [ ] Service Workers & PWA

#### **Runtime Performance**
- [ ] Minimize re-renders
- [ ] Virtualization for long lists
- [ ] Image optimization (lazy loading, WebP, responsive images)
- [ ] Debouncing/Throttling user inputs
- [ ] Web Workers for heavy computations

#### **Metrics** ⭐
- [ ] Core Web Vitals (LCP, FID, CLS)
- [ ] Lighthouse score
- [ ] Performance monitoring tools

### ✅ Design System Questions (Common in Interviews)

#### **Build Complex Components** ⭐⭐
- [ ] Infinite scroll implementation
- [ ] Autocomplete/Typeahead
- [ ] Carousel/Slider
- [ ] Modal/Dialog system
- [ ] Toast/Notification system
- [ ] Virtualized list (windowing)
- [ ] File uploader with preview
- [ ] Multi-step form
- [ ] Data table with sorting, filtering, pagination

#### **Design System Scenarios**
- [ ] Design Instagram feed
- [ ] Design Twitter timeline
- [ ] Design Netflix homepage
- [ ] Design Google search autocomplete
- [ ] Design a commenting system

### ✅ Browser & Web Technologies

#### **How Browsers Work**
- [ ] Critical rendering path
- [ ] HTML parsing → DOM tree
- [ ] CSS parsing → CSSOM tree
- [ ] Render tree construction
- [ ] Layout (reflow)
- [ ] Paint (repaint)
- [ ] Compositing

#### **Security**
- [ ] XSS (Cross-Site Scripting)
- [ ] CSRF (Cross-Site Request Forgery)
- [ ] Content Security Policy (CSP)
- [ ] CORS (Cross-Origin Resource Sharing)
- [ ] Same-Origin Policy

#### **Storage**
- [ ] localStorage vs sessionStorage
- [ ] IndexedDB
- [ ] Cookies (httpOnly, secure, SameSite)

#### **Network**
- [ ] HTTP/1.1 vs HTTP/2 vs HTTP/3
- [ ] HTTPS and TLS
- [ ] HTTP caching (Cache-Control, ETag)
- [ ] Service Workers for offline support

---

## System Design - Backend

### ✅ High-Level Design (HLD)

#### **System Design Fundamentals** ⭐⭐
- [ ] Requirements gathering (Functional & Non-functional)
- [ ] Capacity estimation (Storage, Bandwidth, QPS)
- [ ] Traffic estimation
- [ ] Back-of-envelope calculations

#### **Scalability** ⭐⭐
- [ ] Vertical vs Horizontal scaling
- [ ] Load Balancing
  - [ ] Round Robin
  - [ ] Least Connections
  - [ ] IP Hash
  - [ ] Layer 4 vs Layer 7 load balancers
- [ ] Stateless vs Stateful services
- [ ] Database scaling (Read replicas, Sharding)

#### **Caching** ⭐⭐
- [ ] Caching strategies
  - [ ] Cache-Aside (Lazy loading)
  - [ ] Write-Through
  - [ ] Write-Behind
  - [ ] Refresh-Ahead
- [ ] Cache eviction policies (LRU, LFU, FIFO)
- [ ] Distributed caching (Redis, Memcached)
- [ ] CDN caching

#### **Databases** ⭐⭐
- [ ] SQL vs NoSQL (When to use what)
- [ ] CAP Theorem
- [ ] ACID vs BASE
- [ ] Database Sharding
- [ ] Database Replication (Master-Slave, Master-Master)
- [ ] Consistent Hashing
- [ ] Database Indexing strategies

#### **Message Queues & Async Processing** ⭐
- [ ] Message Queue pattern
- [ ] RabbitMQ / Kafka basics
- [ ] Pub-Sub pattern
- [ ] Event-driven architecture
- [ ] Task queues (Bull, Bee-Queue)

#### **Microservices** ⭐
- [ ] Monolith vs Microservices
- [ ] Service discovery
- [ ] API Gateway
- [ ] Inter-service communication (REST, gRPC)
- [ ] Distributed transactions (Saga pattern)
- [ ] Circuit Breaker pattern

#### **API Design** ⭐
- [ ] REST API best practices
- [ ] API Rate limiting
- [ ] API versioning
- [ ] Idempotency
- [ ] Pagination strategies (Offset, Cursor)
- [ ] GraphQL vs REST trade-offs

#### **Security** ⭐
- [ ] Authentication (JWT, OAuth, Session)
- [ ] Authorization (RBAC, ABAC)
- [ ] API Security (API keys, rate limiting)
- [ ] Data encryption (at rest, in transit)
- [ ] HTTPS/TLS

#### **Monitoring & Logging** ⭐
- [ ] Application logging (Winston, Bunyan)
- [ ] Distributed tracing
- [ ] Metrics collection (Prometheus, Grafana)
- [ ] Error tracking (Sentry)
- [ ] Health checks
- [ ] Alerting

#### **Reliability**
- [ ] Fault tolerance
- [ ] Retry mechanisms (Exponential backoff)
- [ ] Circuit Breaker
- [ ] Bulkhead pattern
- [ ] Graceful degradation
- [ ] Disaster recovery

### ✅ Common System Design Interview Questions ⭐⭐

#### **Design Questions (Practice These)**
- [ ] Design URL Shortener (like bit.ly)
- [ ] Design Twitter
- [ ] Design Instagram
- [ ] Design WhatsApp/Chat application
- [ ] Design YouTube/Netflix
- [ ] Design Uber/Ola
- [ ] Design E-commerce system (Amazon)
- [ ] Design Rate Limiter
- [ ] Design Web Crawler
- [ ] Design Notification Service
- [ ] Design Payment System
- [ ] Design API Gateway
- [ ] Design Real-time leaderboard
- [ ] Design Food delivery app (Swiggy/Zomato)

#### **Low-Level Design (LLD)**
- [ ] Design Parking Lot
- [ ] Design Library Management System
- [ ] Design Elevator System
- [ ] Design Tic-Tac-Toe
- [ ] Design Chess Game
- [ ] Design Vending Machine

---

## Common Interview Questions

### ✅ JavaScript Tricky Questions
- [ ] Predict output: hoisting scenarios
- [ ] Predict output: closure in loops
- [ ] Predict output: event loop (setTimeout, Promise, async/await)
- [ ] Predict output: this keyword scenarios
- [ ] Implement: debounce function
- [ ] Implement: throttle function
- [ ] Implement: deep clone
- [ ] Implement: flatten nested array
- [ ] Implement: Promise.all()
- [ ] Implement: Function.prototype.bind()
- [ ] Implement: Event Emitter
- [ ] Implement: LRU Cache

### ✅ React Coding Questions
- [ ] Build infinite scroll
- [ ] Build autocomplete with debounce
- [ ] Build custom hooks (useFetch, useDebounce, useLocalStorage)
- [ ] Optimize component with many re-renders
- [ ] Build todo app with local storage
- [ ] Build modal component
- [ ] Build pagination component
- [ ] Implement context-based theme switcher

### ✅ Node.js Questions
- [ ] How does Node.js handle concurrency?
- [ ] Explain event loop with example
- [ ] What are streams? When to use them?
- [ ] Difference between fork() and spawn()
- [ ] How to handle file uploads?
- [ ] Implement JWT authentication
- [ ] Implement rate limiting middleware
- [ ] How to handle errors in async/await?

### ✅ MongoDB Questions
- [ ] When to use MongoDB vs SQL?
- [ ] Explain indexing with example
- [ ] Write aggregation query for complex scenario
- [ ] How to model relationships in MongoDB?
- [ ] What is sharding and when to use it?
- [ ] Explain replica sets

### ✅ System Design Approach
1. **Clarify requirements** (5 min)
   - Functional requirements
   - Non-functional requirements
   - Scale (users, requests/sec, data size)
2. **High-level design** (10 min)
   - Draw basic architecture
   - Identify core components
3. **Deep dive** (15-20 min)
   - Database design
   - API design
   - Scalability
   - Caching strategy
4. **Trade-offs & Bottlenecks** (5-10 min)

---

## Interview Preparation Tips

### Study Plan (8-12 Weeks)
- **Week 1-2**: JavaScript deep dive (closures, prototypes, async)
- **Week 3-4**: React internals and hooks
- **Week 5-6**: Node.js, Express, authentication
- **Week 7-8**: MongoDB, databases, aggregation
- **Week 9-10**: System design fundamentals
- **Week 11-12**: Practice coding questions and mock interviews

### Resources
- **JavaScript**: javascript.info, You Don't Know JS (book series)
- **React**: Official docs, Kent C. Dodds blog
- **Node.js**: Official docs, Node.js Design Patterns (book)
- **System Design**: System Design Primer (GitHub), Designing Data-Intensive Applications (book)
- **Practice**: LeetCode, HackerRank, AlgoExpert

### Before Interview
- [ ] Review this checklist
- [ ] Practice whiteboard coding
- [ ] Prepare STAR format stories for behavioral questions
- [ ] Prepare questions to ask interviewer
- [ ] Review recent projects in depth

---

## 🎯 Priority Topics for 3+ Years Experience

**Must Know (Asked in 90% interviews):**
- Closures, Prototypes, Event Loop, Promises
- React Hooks, Virtual DOM, Performance optimization
- Node.js Event Loop, Streams, Middleware
- MongoDB Indexing, Aggregation
- REST API design, JWT Authentication
- System Design: Scalability, Caching, Load Balancing

**Good to Know (Asked in 50-70% interviews):**
- Polyfills, Design patterns
- React Fiber, Concurrent mode
- Cluster, Child processes
- MongoDB Sharding, Replication
- Microservices, Message Queues

**Nice to Have (Differentiator):**
- Advanced system design patterns
- Performance profiling tools
- GraphQL
- CI/CD, Docker basics

---

**Good luck with your interviews! 🚀**

*Check off each item as you master it. Focus on understanding "how things work" rather than just memorizing.*
