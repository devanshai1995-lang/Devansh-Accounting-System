# Contributing to Devansh Accounting System

Thank you for your interest in contributing! We welcome developers, accountants, and domain experts to help build a world-class accounting solution for Indian industries.

## Code of Conduct

- Be respectful and inclusive
- Help others and provide constructive feedback
- Report issues professionally
- No harassment or discrimination

## How to Contribute

### 1. **Reporting Bugs**

If you find a bug, please create an issue with:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Environment details (OS, browser, etc.)

### 2. **Suggesting Features**

Feature requests should include:
- Clear use case and problem statement
- Why this feature is needed
- How it aligns with project goals
- Proposed implementation approach (if any)

### 3. **Code Contributions**

#### Setup Development Environment

```bash
# Fork the repository
git clone https://github.com/YOUR_USERNAME/Devansh-Accounting-System.git
cd Devansh-Accounting-System

# Create a feature branch
git checkout -b feature/your-feature-name

# Install dependencies
npm install  # or pip install -r requirements.txt

# Create .env file
cp .env.example .env
```

#### Development Workflow

1. **Create a feature branch** from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes**:
   - Follow the project's code style
   - Write clean, readable code
   - Add comments for complex logic
   - Update documentation if needed

3. **Write/Update Tests**:
   ```bash
   npm test  # Run tests
   ```

4. **Commit your changes**:
   ```bash
   git commit -m "Add: Clear description of changes"
   ```
   
   Commit message format:
   - `Add:` - New features
   - `Fix:` - Bug fixes
   - `Docs:` - Documentation updates
   - `Refactor:` - Code refactoring
   - `Test:` - Test additions/updates
   - `Style:` - Code style changes

5. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create a Pull Request**:
   - Clear title describing the change
   - Reference related issues using `#issue_number`
   - Describe what was changed and why
   - Include any testing notes

## Coding Standards

### JavaScript/Node.js
```javascript
// Use const/let (no var)
const maxRetries = 3;

// Arrow functions preferred
const calculate = (a, b) => a + b;

// Descriptive variable names
const customerInvoiceTotal = 5000;

// Comments for complex logic
// Calculate GST at 18% for service category
const gstAmount = total * 0.18;
```

### File Naming
- Components: `PascalCase` (e.g., `InvoiceForm.js`)
- Utilities: `camelCase` (e.g., `gstCalculator.js`)
- Tests: `filename.test.js`

### Documentation
- Add JSDoc comments for functions
- Include parameter types and return values
- Document edge cases

```javascript
/**
 * Calculate GST amount for a given value
 * @param {number} value - The base amount
 * @param {number} rate - GST rate (e.g., 5, 12, 18)
 * @returns {number} GST amount
 */
const calculateGST = (value, rate) => (value * rate) / 100;
```

## Testing Requirements

- Write unit tests for business logic
- Maintain >70% code coverage for core modules
- Test edge cases and error scenarios
- Run tests before submitting PR

```bash
npm test                    # Run all tests
npm test -- --coverage     # With coverage report
npm test -- --watch       # Watch mode
```

## Documentation Updates

When contributing, please update relevant documentation:
- `README.md` - If adding major features
- `docs/` folder - Detailed feature documentation
- Code comments - Inline documentation
- API documentation - If adding endpoints

## Review Process

1. **Automated Checks**:
   - Tests must pass
   - Code coverage requirements met
   - Linting passes (ESLint)

2. **Code Review**:
   - At least one maintainer review required
   - Constructive feedback provided
   - Request changes if needed

3. **Approval & Merge**:
   - All reviews approved
   - No conflicts with `main`
   - Feature branch deleted after merge

## Areas We're Looking For Help

### High Priority
- [ ] Core accounting module development
- [ ] GST compliance features
- [ ] Database schema optimization
- [ ] API endpoint development

### Medium Priority
- [ ] UI/UX improvements
- [ ] Integration features
- [ ] Documentation
- [ ] Testing & QA

### Community Contributions
- [ ] Bug reports and fixes
- [ ] Feature suggestions
- [ ] Documentation improvements
- [ ] Translation/localization
- [ ] Performance optimization

## Getting Help

- Check existing [Issues](https://github.com/devanshai1995-lang/Devansh-Accounting-System/issues)
- Read [Documentation](https://github.com/devanshai1995-lang/Devansh-Accounting-System/tree/main/docs)
- Open a [Discussion](https://github.com/devanshai1995-lang/Devansh-Accounting-System/discussions)
- Contact maintainers via issues

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

## Recognition

Contributors will be recognized in:
- Project README
- Release notes
- Contributors page

---

Thank you for making Devansh Accounting System better! 🙌
