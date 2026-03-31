## Session 1

### Exercise 1: Local API Setup and Audit

#### Step 1: Launch the API locally (15 min)
1. Fork the provided API repository
2. Install dependencies
3. Start the API server locally: http://localhost:8000/api/v1/stations/
4. Test basic endpoints with curl or Postman

#### Step 2: System Audit (25 min)
1. Create an audit checklist with these categories:
   - Code quality
   - Testing
   - Deployment process
   - Monitoring
   - Security
   - Documentation

2. For each category, identify:
   - What's missing
   - What's manual vs automated
   - Potential failure points

#### Step 3: Improvement Plan (15 min)
1. Prioritize the top 5 issues found
2. For each issue, propose:
   - Short-term fix
   - Long-term solution
   - Tools/technologies to implement

**Deliverable**: Markdown file with audit findings and improvement plan

## Session 2: Advanced Git

### Exercise 1: Git Workflow Setup (30 min)
1. Use first repo 
2. Set up branch protection for `main` branch:
   - Require PR reviews
   - Require status checks to pass
   - Require signed commits
3. Add a PR template with sections:
   - Description
   - Related issues
   - Testing done
   - Checklist

### Exercise 2: Conflict Simulation (25 min)
1. Create a feature branch from main
2. Have another team member create a conflicting change on main
3. Attempt to merge and resolve conflicts
4. Document the resolution process

**Deliverable**: Repository with protected branches and documented conflict resolution process : https://github.com/jadechy/14_ValorisationDonneeMeteo

## Session 3: CI/CD

### Exercise 1: Basic Pipeline Creation (40 min)
1. Create `.github/workflows/ci.yml` or `.gitlab-ci.yml`
2. Add stages:
   - Install dependencies
   - Run tests
   - Run linter
   - Run security scan
   - Build Docker image
   - Push to registry (on main branch only)

### Exercise 2: Pipeline Testing (15 min)
1. Intentionally break a test to verify CI catches it
2. Fix the test and verify pipeline passes
3. Add a CI badge to your README

**Deliverable**: Functional CI/CD pipeline with badge in README
- Docker image
- test report
- scan code report
- trivy report
- fichier vex