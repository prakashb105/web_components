---
type: "pages/prompts"
title: "AI Prompts"
url: "/pages/prompts/"
prompts:
  - category: "HTML & Accessibility"
    items:
      - title: "Semantic HTML Review"
        prompt: "Review the following HTML and refactor it to use proper semantic elements (header, nav, main, section, article, aside, footer). Ensure all images have descriptive alt text, all form inputs have associated labels, and ARIA attributes are used where necessary."
      - title: "Accessibility Audit"
        prompt: "Audit this webpage code for WCAG 2.1 AA compliance. Check for color contrast issues, missing alt text, keyboard navigation problems, missing ARIA roles/labels, and focus management. Provide a prioritized list of fixes."
      - title: "Meta Tags & SEO"
        prompt: "Generate a complete set of meta tags for a webpage about [TOPIC]. Include Open Graph tags, Twitter Card tags, canonical URL, description, viewport, charset, and any structured data (JSON-LD) that would be appropriate."

  - category: "CSS & Styling"
    items:
      - title: "Responsive Layout"
        prompt: "Create a responsive CSS Grid layout for a dashboard with a sidebar, header, main content area, and footer. It should collapse to a single column on mobile (<768px), show a collapsible sidebar on tablet (768px–1024px), and the full layout on desktop. Use CSS custom properties for spacing and colors."
      - title: "Dark Mode Toggle"
        prompt: "Implement a CSS dark mode system using CSS custom properties and prefers-color-scheme media query. Include a toggle button that saves the user's preference to localStorage and respects their OS-level setting as the default."
      - title: "Animation & Transitions"
        prompt: "Create a smooth page transition animation using CSS @keyframes for a single-page app feel. Include enter/exit animations for route changes, a loading skeleton screen, and staggered list item animations. Keep animations under 300ms and respect prefers-reduced-motion."
      - title: "CSS Architecture"
        prompt: "Refactor this CSS file using BEM naming convention. Identify repeated values and extract them into CSS custom properties. Remove any unused selectors, reduce specificity issues, and organize rules by component."

  - category: "JS"
    items:
      - title: "Debounce & Throttle"
        prompt: "Write a production-ready debounce and throttle utility in vanilla JS with TypeScript types. Include options for leading/trailing edge execution, cancel method, and flush method. Add JSDoc comments and unit test cases."
      - title: "Fetch Wrapper"
        prompt: "Create a reusable fetch API wrapper that handles: automatic JSON parsing, request/response interceptors, timeout support, retry logic with exponential backoff, abort controller integration, and typed error handling. Use TypeScript."
      - title: "Form Validation"
        prompt: "Build a lightweight form validation library in vanilla JS that supports: required fields, email/URL/phone patterns, min/max length, custom regex, async validation (e.g., checking username availability), and real-time inline error messages with proper ARIA attributes."
      - title: "LocalStorage Manager"
        prompt: "Create a type-safe localStorage utility that handles: JSON serialization/deserialization, expiry/TTL support, storage quota detection, cross-tab synchronization via storage events, and a fallback to in-memory storage when localStorage is unavailable."

  - category: "React & Frameworks"
    items:
      - title: "Custom Hook"
        prompt: "Create a custom React hook called useAsync that handles async operations with loading, error, and data states. Include support for: automatic execution on mount, manual trigger, cancellation on unmount, retry logic, and TypeScript generics for the return type."
      - title: "Component Architecture"
        prompt: "I have a large monolithic React component (pasted below). Refactor it by extracting logical pieces into smaller, reusable components. Apply the single responsibility principle, use composition over prop drilling, and suggest where to use context or custom hooks."
      - title: "Performance Optimization"
        prompt: "Analyze this React component for performance issues. Check for: unnecessary re-renders, missing memoization (useMemo/useCallback), large bundle imports that should be lazy-loaded, unoptimized images, and missing key props in lists. Provide before/after code."

  - category: "Testing"
    items:
      - title: "Unit Test Generation"
        prompt: "Generate comprehensive unit tests for the following function/component. Cover: happy path, edge cases (empty input, null, undefined, boundary values), error cases, and async behavior. Use [Jest/Vitest] with descriptive test names following the 'should... when...' pattern."
      - title: "E2E Test Scenario"
        prompt: "Write Playwright end-to-end tests for a user login flow. Cover: successful login, invalid credentials, empty form submission, remember me functionality, redirect after login, and session expiry. Use Page Object Model pattern."

  - category: "Code Review & Refactoring"
    items:
      - title: "Code Review Checklist"
        prompt: "Review this code for: security vulnerabilities (XSS, injection, CSRF), performance bottlenecks, memory leaks, error handling gaps, naming conventions, DRY violations, and adherence to SOLID principles. Rate severity (critical/major/minor) for each finding."
      - title: "Legacy Code Refactor"
        prompt: "Refactor this legacy JavaScript code to modern ES2024+ standards. Replace var with const/let, convert callbacks to async/await, use optional chaining and nullish coalescing, replace lodash utilities with native methods where possible, and add TypeScript types."
      - title: "Regex Generator"
        prompt: "Write a well-commented regular expression that matches [PATTERN DESCRIPTION]. Include: the regex with named capture groups, a plain-English explanation of each part, 5 examples of strings that match, 5 examples that don't match, and edge cases to be aware of."

  - category: "MR & Code Review"
    items:
      - title: "MR Description"
        prompt: "Generate a clear and concise Merge Request (MR) description for the changes in @[file_path]. The output should include a short, technical title followed by a brief summary explaining what was changed and why (limit this to 3–4 sentences). Then describe the key modifications in a focused way, including small, relevant code snippets only where necessary to clarify non-trivial logic. Clearly mention any breaking changes, dependency updates, or impacts on performance, accessibility, or mobile usability. Conclude with how the changes were tested and any important edge cases that were validated. Keep the tone direct and technical, and avoid unnecessary detail or filler."
---