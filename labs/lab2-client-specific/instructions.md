# Lab 2: Bob vs Cursor - Head-to-Head Comparison

**Duration:** 40 minutes  
**Difficulty:** Intermediate  
**Focus:** Comprehensive comparison of Bob's key differentiators vs Cursor

## 🎯 Objectives

By the end of this lab, you will be able to:
- Experience all of Bob's key differentiators in action
- Understand when to use Bob vs Cursor for different scenarios
- Develop a complementary usage strategy
- Apply Bob's unique capabilities to real development tasks

## 📋 Prerequisites

- [ ] Completed Labs 1 and 2
- [ ] Understanding of Bob's agentic workflow model
- [ ] Familiarity with both Bob and Cursor (optional)
- [ ] Python 3.8+ and Node.js 16+ installed

## 🔨 Comparison Scenarios

### Scenario 1: Agentic Workflows - Autonomous Multi-Step Execution (15 minutes)

**The Challenge:** Implement a complete microservice with API, database, tests, and deployment configuration.

**Bob's Approach: Full Autonomous Execution**

**Task:**
Create a complete Python microservice from scratch with all components.

**Example Prompt for Bob:**
```
Create a complete Python microservice for a task management system:

1. Project Structure:
   - Create directories: src/, tests/, config/, deploy/
   - Create requirements.txt with Flask, SQLAlchemy, pytest, gunicorn

2. Database Layer (src/models/task.py):
   - Task model with id, title, description, status, created_at
   - SQLAlchemy ORM setup
   - Database initialization

3. API Layer (src/api/tasks.py):
   - GET /tasks - List all tasks
   - POST /tasks - Create new task
   - PUT /tasks/<id> - Update task
   - DELETE /tasks/<id> - Delete task
   - Proper error handling and validation

4. Tests (tests/test_tasks.py):
   - Unit tests for all endpoints
   - Test validation and error cases
   - Test database operations

5. Configuration (config/app.py):
   - Environment-based configuration
   - Database connection settings
   - Logging setup

6. Deployment (deploy/Dockerfile):
   - Multi-stage Docker build
   - Production-ready configuration

7. Documentation (README.md):
   - Setup instructions
   - API documentation
   - Deployment guide

8. Install all dependencies and run tests to verify everything works
```

**Cursor's Approach:**
With Cursor, you would need to:
1. Create each file manually
2. Copy code suggestions one by one
3. Manually install dependencies
4. Manually run tests
5. Manually create Docker configuration
6. Manually write documentation

**Expected Outcome:**
- Complete microservice created
- All files and directories in place
- Dependencies installed
- Tests written and passing
- Docker configuration ready
- Documentation complete
- Ready to deploy

**💡 Key Differentiator:**
Bob's agentic workflow executes the entire project setup autonomously. Cursor requires manual intervention at every single step.

---

### Scenario 2: Tool Integration - Direct System Access (10 minutes)

**The Challenge:** Set up a complete development environment with git, dependencies, and CI/CD.

**Bob's Approach: Direct Tool Access**

**Task:**
Initialize a project with version control, dependencies, and automated testing.

**Example Prompt for Bob:**
```
Set up a complete development environment:

1. Git Setup:
   - Initialize git repository
   - Create .gitignore for Python
   - Create initial commit
   - Create develop branch
   - Set up git hooks for pre-commit testing

2. Dependency Management:
   - Create requirements.txt with Flask, pytest, black, flake8
   - Create requirements-dev.txt with additional dev tools
   - Install all dependencies in virtual environment

3. Code Quality:
   - Set up black for code formatting
   - Configure flake8 for linting
   - Create .pre-commit-config.yaml

4. CI/CD (. github/workflows/test.yml):
   - GitHub Actions workflow
   - Run tests on push
   - Run linting and formatting checks
   - Generate coverage report

5. Run initial tests and show me the results
```

**Cursor's Limitation:**
Cursor cannot:
- Execute git commands
- Install packages
- Create git hooks
- Set up CI/CD
- Run tests
All of this must be done manually in the terminal.

**Expected Outcome:**
- Git repository initialized
- All dependencies installed
- Code quality tools configured
- CI/CD pipeline set up
- Tests running automatically
- All done through Bob

**💡 Key Differentiator:**
Bob has direct access to terminal, git, package managers, and file system. Cursor is limited to code suggestions within the editor.

---

### Scenario 3: Context Awareness - Full Codebase Understanding (10 minutes)

**The Challenge:** Refactor a feature that spans multiple files with complex dependencies.

**Bob's Approach: Full Project Context**

**Task:**
Refactor authentication system across multiple files while maintaining all dependencies.

**Example Prompt for Bob:**
```
I have an authentication system spread across these files:
- models/user.py (User model)
- services/auth_service.py (Authentication logic)
- api/auth_routes.py (API endpoints)
- middleware/auth_middleware.py (Request authentication)
- tests/test_auth.py (Test suite)

Refactor the authentication system to:
1. Change from session-based to JWT token authentication
2. Update User model to include token fields
3. Update AuthService to generate and validate JWTs
4. Update all API routes to use JWT authentication
5. Update middleware to validate JWT tokens
6. Update all tests to work with new JWT system
7. Ensure all cross-file dependencies are maintained

Analyze the impact across all files and make all necessary changes.
```

**Cursor's Limitation:**
Cursor would require you to:
1. Manually identify all affected files
2. Update each file individually
3. Manually track dependencies
4. Risk missing some references
5. Manually verify consistency

**Expected Outcome:**
- All files updated consistently
- JWT authentication implemented
- All dependencies maintained
- Tests updated and passing
- No broken references
- Complete refactoring in one workflow

**💡 Key Differentiator:**
Bob understands your entire codebase structure and automatically updates all dependent files. Cursor focuses on current file, requiring manual cross-file updates.

---

### Scenario 4: Mode Specialization - Right Tool for the Job (5 minutes)

**The Challenge:** Plan, implement, and debug a complex feature.

**Bob's Approach: Specialized Modes**

**Task:**
Use different Bob modes for different phases of development.

**Example Workflow:**

**Phase 1: Planning (Ask Mode)**
```
[Switch to Ask Mode]
"Explain the trade-offs between microservices and monolithic architecture for a task management system. What are the key considerations?"
```

**Phase 2: Architecture (Plan Mode)**
```
[Switch to Plan Mode]
"Create a detailed implementation plan for adding real-time notifications to our task management system using WebSockets. Break it down into steps with dependencies."
```

**Phase 3: Implementation (Code Mode)**
```
[Switch to Code Mode]
"Implement step 1 of the plan: Set up WebSocket server with Flask-SocketIO."
```

**Phase 4: Debugging (Debug Mode - if available)**
```
[Switch to Debug Mode]
"The WebSocket connection is dropping after 30 seconds. Help me debug this issue."
```

**Cursor's Limitation:**
Cursor has a single chat interface for all tasks. No specialized modes for different types of work.

**Expected Outcome:**
- Clear understanding from Ask mode
- Detailed plan from Plan mode
- Working implementation from Code mode
- Issues resolved in Debug mode
- Optimal tool for each phase

**💡 Key Differentiator:**
Bob's mode specialization provides the right tool for each phase of development. Cursor uses one interface for everything.

---

## 🎓 Complementary Usage Strategy

### When to Use Bob

✅ **Complex Multi-Step Tasks**
- Feature implementation across multiple files
- System setup and configuration
- Refactoring with dependencies
- Automated testing and CI/CD

✅ **System Operations**
- Git operations (commit, branch, merge)
- Package management (install, update)
- File system operations
- Command execution

✅ **Architecture and Planning**
- System design and planning
- Breaking down complex tasks
- Impact analysis
- Technical decision-making

✅ **Autonomous Workflows**
- End-to-end feature development
- Automated deployments
- Database migrations
- Documentation generation

### When to Use Cursor

✅ **Quick Edits**
- Single-line changes
- Fast autocomplete
- Inline suggestions
- Rapid prototyping in one file

✅ **Learning and Exploration**
- Asking questions about code
- Getting code snippets
- Exploring new concepts
- Quick experiments

### Optimal Daily Workflow

**Morning: Feature Development**
1. **Bob (Plan Mode)**: Plan the day's work
2. **Bob (Code Mode)**: Implement core functionality
3. **Cursor**: Quick inline edits and refinements
4. **Bob**: Run tests and commit changes

**Midday: Bug Fixing**
1. **Bob**: Run tests to identify failures
2. **Bob**: Search codebase for root cause
3. **Cursor**: Quick fixes in individual files
4. **Bob**: Verify fixes and commit

**Afternoon: Code Review**
1. **Bob**: Analyze code for issues
2. **Cursor**: Make suggested improvements
3. **Bob**: Update tests and documentation
4. **Bob**: Final verification and push

---

## ✅ Completion Checklist

- [ ] Completed Scenario 1: Agentic Workflows
- [ ] Completed Scenario 2: Tool Integration
- [ ] Completed Scenario 3: Context Awareness
- [ ] Completed Scenario 4: Mode Specialization
- [ ] Understand all of Bob's key differentiators
- [ ] Know when to use Bob vs Cursor
- [ ] Have a complementary usage strategy
- [ ] Ready to apply Bob to real projects

---

## 📚 Additional Resources

- **Bob Differentiators**: See [`resources/bob-differentiators.md`](../../resources/bob-differentiators.md)
- **Bob Productivity Gains**: See [`resources/bob-productivity-gains-client-zero.md`](../../resources/bob-productivity-gains-client-zero.md)
- **Cheat Sheet**: See [`resources/cheat-sheet.md`](../../resources/cheat-sheet.md)
- **Troubleshooting**: See [`resources/troubleshooting.md`](../../resources/troubleshooting.md)

---

## 🎉 Congratulations!

You've completed the Bob vs Cursor comparison workshop! You now understand:
- Bob's unique agentic workflow model
- When to use Bob vs Cursor
- How to leverage both tools effectively
- Bob's key differentiators and business value

**Remember:** Bob and Cursor are complementary tools. Use Bob for complex, multi-step tasks and system operations. Use Cursor for quick edits and inline suggestions. Together, they provide a powerful development experience.

---

**Need Help?** Ask your facilitator or use the dedicated support channel!

**Feedback:** Please share your workshop experience to help us improve future sessions.
