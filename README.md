# Airline Operations & Booking Management System

**Expert Academic Software Engineering Project**  
**Architecture:** MVC + Service Layer Pattern  
**Stack:** HTML5, CSS3, JavaScript ES6+

---

## 👥 Team Members

| Name | ID | Role | Files |
|------|----|----|-------|
| **Abraham Amogne** | ETS 1848/17 | Core Infrastructure & Search | 22 |
| **Saron Anbesaw** | ETS 1309/17 | Passenger Booking Flow | 8 |
| **Seble Sisay** | ETS 1314/17 | Staff Flight Operations & Auth | 9 |
| **Senet Anbesaw** | ETS 1332/17 | Staff Crew & Schedule Analytics | 8 |
| **Shanbel Dires** | ETS 1336/17 | Passenger Check-In & Boarding Services | 6 |

---

## 📁 Project Structure

```
airline-operations-system/
├── index.html                              # Homepage
├── pages/
│   ├── passenger/                         # 10 pages
│   │   ├── search-flights.html
│   │   ├── flight-details.html
│   │   ├── booking-form.html
│   │   ├── booking-confirmation.html
│   │   ├── bookings-list.html
│   │   ├── booking-cancellation.html
│   │   ├── check-in.html
│   │   ├── boarding-pass.html
│   │   ├── flight-status.html
│   │   └── contact.html
│   └── staff/                             # 8 pages
│       ├── login.html
│       ├── dashboard.html
│       ├── flights-management.html
│       ├── crew-management.html
│       ├── crew-assignment.html
│       ├── schedule-view.html
│       └── reports-analytics.html
├── styles/
│   ├── core/                              # reset, variables, typography, layout
│   ├── components/                        # buttons, forms, cards, tables, modals, navigation
│   ├── modules/                           # passenger-portal, check-in, staff-portal, reports
│   └── utilities/                         # responsive
├── scripts/
│   ├── core/                              # app, config, constants
│   ├── utils/                             # validators, formatters, helpers, error-handler
│   ├── services/                          # storage-service, auth-service, data-service
│   ├── models/                            # flight-model, booking-model, crew-model, user-model, check-in-model
│   ├── controllers/
│   │   ├── passenger/                     # search-controller, booking-controller, check-in-controller
│   │   └── staff/                         # flights-controller, crew-controller, reports-controller
│   └── data/                              # seed-data
└── assets/
    ├── images/                            # logos, icons, backgrounds
    └── fonts/
```

**Total:** 53 files (18 HTML, 14 CSS, 20 JS, 1 data)

---

## 🎯 Features

### Passenger Portal
- Flight search with filters (price, time, stops, airline)
- Interactive seat selection with visual map
- Multi-passenger booking with validation
- Booking management (view, search, cancel)
- Real-time price calculation and refund
- Online check-in with seat confirmation and digital boarding pass generation
- Live flight status tracking and schedule lookup

### Staff Portal
- Role-based authentication and navigation security guards
- Flight CRUD operations with search/filter
- Crew CRUD operations with license tracking
- Intelligent crew assignment (prevents double-booking)
- Schedule visualization (calendar, timeline, table)
- Reports and analytics with export

---

## 📋 Member Assignments

### Abraham Amogne (ETS 1848/17) - 22 files
**HTML (3):** index.html, search-flights, flight-details  
**CSS (8):** Core (reset, variables, typography, layout), Components (buttons, cards, navigation), Utilities (responsive)  
**JS (11):** Core (app, config, constants), Utils (validators, formatters, helpers, error-handler), Services (storage, data), Controllers (search), Data (seed-data)  
**Testing:** Core infrastructure testing, utility validators unit testing, flight search validation

---

### Saron Anbesaw (ETS 1309/17) - 8 files
**HTML (4):** booking-form, booking-confirmation, bookings-list, booking-cancellation  
**CSS (2):** forms, modals  
**JS (2):** booking-model, booking-controller  
**Testing:** Booking lifecycle testing, seat selection logic, cancellation & refund calculations

---

### Seble Sisay (ETS 1314/17) - 9 files
**HTML (3):** login, dashboard, flights-management  
**CSS (2):** tables, staff-portal  
**JS (4):** flight-model, user-model, auth-service, flights-controller  
**Testing:** Authentication service validation, role access guards, flight CRUD operations

---

### Senet Anbesaw (ETS 1332/17) - 8 files
**HTML (4):** crew-management, crew-assignment, schedule-view, reports-analytics  
**CSS (1):** reports  
**JS (3):** crew-model, crew-controller, reports-controller  
**Testing:** Crew qualification checks, schedule conflict detection, reporting aggregations

---

### Shanbel Dires (ETS 1336/17) - 6 files
**HTML (3):** check-in, boarding-pass, flight-status  
**CSS (1):** check-in  
**JS (2):** check-in-model, check-in-controller  
**Testing:** Check-in validation, digital boarding pass verification, flight tracking, QA coordination

---

## 🚀 Development Phases

### Phase 1: HTML Structure (Week 1-2)
**All members:** Create HTML files for their assigned modules  
**Rules:** Semantic HTML5 only, NO CSS, NO JavaScript  
**Deliverable:** 18 validated HTML pages

### Phase 2: CSS Styling (Week 3-4)
**Day 1-2:** Abraham creates core CSS (layout, variables, reset)  
**Day 3-10:** All members create their module and component CSS files  
**Rules:** Responsive design, mobile-first, NO JavaScript  
**Deliverable:** 14 CSS files, fully responsive across mobile, tablet, and desktop

### Phase 3: JavaScript Functionality (Week 5-8)
**Week 5 Day 1-2:** Abraham initializes core contracts, data schema, and storage service  
**Week 5 Day 3+:** All members develop models and controllers in parallel using shared contracts  
**Week 6-7:** Full feature implementation and inter-module integration  
**Week 8:** Collaborative testing, edge case handling, and bug resolution  
**Deliverable:** 20 JS files, all features functioning seamlessly

### Integration & Testing (Week 9)
**All members:** End-to-end integration testing, UI Polish, presentation prep  
**Shared QA:** Every member validates their flow; Shanbel coordinates test records and documentation

---

## 🏗️ Architecture

**Pattern:** MVC (Model-View-Controller) + Service Layer

```
View Layer:       pages/**/*.html
Styling Layer:    styles/**/*.css
Controller Layer: scripts/controllers/**/*.js
Service Layer:    scripts/services/**/*.js
Model Layer:      scripts/models/**/*.js
Data Layer:       localStorage + scripts/data/seed-data.js
```

**Collaboration & Flow Model:**
```
Abraham (Core Services & Search)
     │
     ├──────────────────────┬──────────────────────┐
     ▼                      ▼                      ▼
Saron (Booking Flow)    Seble (Flights & Auth)   Shanbel (Check-In & Boarding)
     │                      │                      │
     └──────────────────────┼──────────────────────┘
                            ▼
                    Senet (Crew & Reports)
                            ▼
     Joint Testing & End-to-End Verification (All 5 Members)
```

---

## 📝 Naming Conventions

### Files
- HTML: `kebab-case.html` (e.g., `search-flights.html`)
- CSS: `kebab-case.css` (e.g., `passenger-portal.css`)
- JS: `entity-type.js` (e.g., `flight-model.js`, `storage-service.js`)

### Folders
- Lowercase, plural nouns: `scripts/`, `controllers/`, `services/`

### CSS Classes (BEM)
```css
.flight-card { }                    /* Block */
.flight-card__header { }            /* Element */
.flight-card--featured { }          /* Modifier */
.is-active { }                      /* State */
```

### JavaScript
```javascript
const MAX_PASSENGERS = 9;           // Constants: UPPER_SNAKE_CASE
let flightResults = [];             // Variables: camelCase
function searchFlights() {}         // Functions: camelCase
class FlightService {}              // Classes: PascalCase
```

---

## 📦 File Load Order

### CSS (in <head>)
```html
<!-- 1. Core -->
<link href="styles/core/reset.css" rel="stylesheet">
<link href="styles/core/variables.css" rel="stylesheet">
<link href="styles/core/typography.css" rel="stylesheet">
<link href="styles/core/layout.css" rel="stylesheet">

<!-- 2. Components -->
<link href="styles/components/buttons.css" rel="stylesheet">
<link href="styles/components/forms.css" rel="stylesheet">
<link href="styles/components/cards.css" rel="stylesheet">
<link href="styles/components/tables.css" rel="stylesheet">
<link href="styles/components/modals.css" rel="stylesheet">
<link href="styles/components/navigation.css" rel="stylesheet">

<!-- 3. Modules (page-specific) -->
<link href="styles/modules/passenger-portal.css" rel="stylesheet">

<!-- 4. Utilities -->
<link href="styles/utilities/responsive.css" rel="stylesheet">
```

### JavaScript (before </body>)
```html
<!-- 1. Core -->
<script src="scripts/core/constants.js"></script>
<script src="scripts/core/config.js"></script>
<script src="scripts/core/app.js"></script>

<!-- 2. Utilities -->
<script src="scripts/utils/error-handler.js"></script>
<script src="scripts/utils/validators.js"></script>
<script src="scripts/utils/formatters.js"></script>
<script src="scripts/utils/helpers.js"></script>

<!-- 3. Services -->
<script src="scripts/services/storage-service.js"></script>
<script src="scripts/services/data-service.js"></script>
<script src="scripts/services/auth-service.js"></script>

<!-- 4. Models -->
<script src="scripts/models/flight-model.js"></script>
<script src="scripts/models/booking-model.js"></script>
<script src="scripts/models/crew-model.js"></script>
<script src="scripts/models/user-model.js"></script>

<!-- 5. Data -->
<script src="scripts/data/seed-data.js"></script>

<!-- 6. Controllers (page-specific) -->
<script src="scripts/controllers/passenger/search-controller.js"></script>
```

---

## 💻 Code Standards

### JavaScript Module Pattern
```javascript
/**
 * Search Controller Module
 * Handles flight search and filtering
 */
const SearchController = (function() {
  'use strict';
  
  // Private variables
  let currentResults = [];
  
  // Public methods
  function searchFlights(criteria) {
    // Implementation
  }
  
  function applyFilters(filters) {
    // Implementation
  }
  
  // Return public API
  return {
    searchFlights,
    applyFilters
  };
})();
```

### JSDoc Comments
```javascript
/**
 * Search for flights based on criteria
 * @param {Object} criteria - Search parameters
 * @param {string} criteria.origin - Origin airport code
 * @param {string} criteria.destination - Destination airport code
 * @param {string} criteria.date - Departure date (YYYY-MM-DD)
 * @param {number} criteria.passengers - Number of passengers
 * @returns {Promise<Array<Object>>} Array of matching flights
 * @throws {Error} If criteria is invalid
 */
async function searchFlights(criteria) {
  // Implementation
}
```

---

## ✅ Quality Checklist

### HTML
- [ ] Valid HTML5 (W3C validated)
- [ ] Semantic elements used
- [ ] All images have alt text
- [ ] All forms have labels
- [ ] Proper heading hierarchy (h1 → h2 → h3)
- [ ] ARIA attributes where needed

### CSS
- [ ] Valid CSS3 (W3C validated)
- [ ] Mobile-first responsive design
- [ ] BEM naming convention
- [ ] No !important (unless necessary)
- [ ] WCAG AA color contrast
- [ ] Cross-browser compatible

### JavaScript
- [ ] ES6+ syntax (const, let, arrow functions)
- [ ] JSDoc comments for functions
- [ ] Error handling (try-catch)
- [ ] Input validation
- [ ] No console.log in production
- [ ] Module pattern used
- [ ] No global variables pollution

---

## 🧪 Testing Requirements (Shared Across All Team Members)

Testing is a shared responsibility across the entire team to ensure high code quality and reliability.

### 1. Component & Module Testing (Every Member)
- **HTML Validation:** Each member validates their markup against W3C HTML5 standards.
- **Form & Input Validation:** Members verify all input boundary checks and validation logic in their controllers.
- **Model Integrity:** Unit testing for data models (e.g. calculation of booking totals, flight seat decrements, crew qualification validity).

### 2. Browser & Device Compatibility (Every Member)
- **Browsers:** Chrome, Firefox, Safari, Edge
- **Devices:** Mobile (320px - 767px), Tablet (768px - 1023px), Desktop (1024px+)
- **Responsive Layout:** Verify mobile-first media queries and touch-friendly interactions.

### 3. Accessibility & Usability (Every Member)
- Keyboard navigation (tab indices, focus rings)
- Screen reader compatibility (semantic landmarks, alt texts, ARIA labels)
- Color contrast meets WCAG 2.1 AA standards

### 4. Joint Integration & End-to-End Testing (Full Team)
- **Collaborative Flow:** Full team executes end-to-end integration journeys across modules (Flight Creation → Crew Assignment → Flight Search → Seat Reservation → Passenger Check-in → Operational Reporting).
- **QA Documentation:** Shanbel coordinates unified test execution matrices, bug tracking logs, and verification reports with contributions from all members.

---

## 📅 Weekly Schedule

| Week | Phase | Focus | Responsibility |
|------|-------|-------|----------------|
| 1-2 | Phase 1 | HTML structure | All |
| 3-4 | Phase 2 | CSS styling | All (Core styles initialized first) |
| 5 | Phase 3 | Core JS setup | Abraham (Core services & contracts) |
| 6-7 | Phase 3 | Full development | All |
| 8 | Phase 3 | Testing & debugging | All |
| 9 | Integration | Integration & presentation | All |

---

## 🎯 Success Criteria

### Functional
- ✅ All features work correctly
- ✅ No console errors
- ✅ Data persists (localStorage)
- ✅ Smooth user flows

### Technical
- ✅ Valid HTML5, CSS3, JavaScript
- ✅ Responsive design works
- ✅ Cross-browser compatible
- ✅ Accessible (WCAG AA)
- ✅ Code well-documented

### Team
- ✅ Equal contributions
- ✅ Regular communication
- ✅ Code reviews done
- ✅ Git commits consistent

---

## 🚦 Getting Started

### 1. Setup Environment
```bash
# Clone/navigate to project folder
cd Airline-Operations-and-Booking-Management-system_project

# View structure
ls -R

# Create your feature branch
git checkout -b feature/your-name-module
```

### 2. Start Phase 1 (Week 1-2)
- Create your assigned HTML files
- Use semantic HTML5 elements
- Add accessibility attributes
- NO CSS or JavaScript yet!

### 3. Communication
- **Daily:** Brief update in team chat
- **Weekly:** Team meeting (1 hour)
- **Git:** Commit regularly with clear messages

---

## 📚 Resources

- **HTML:** [MDN HTML Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **CSS:** [MDN CSS Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS)
- **JavaScript:** [MDN JavaScript Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- **Validator:** [W3C Markup Validator](https://validator.w3.org/)
- **Accessibility:** [WAVE Tool](https://wave.webaim.org/)

---

## 🎓 Grade Breakdown

| Category | Weight | Requirements |
|----------|--------|-------------|
| **Functionality** | 40% | All features work, no errors |
| **Code Quality** | 25% | Clean, documented, follows standards |
| **Design** | 20% | Professional, responsive, accessible |
| **Teamwork** | 10% | Equal contributions, collaboration |
| **Documentation** | 5% | Complete, clear, helpful |

**Target Grade:** A (Excellent)

---

## 📞 Team Communication

**Daily Standups:** 15 min (What done? What next? Blockers?)  
**Weekly Meetings:** 1 hour (Progress review, demos, planning)  
**Git Repository:** [Add URL]  
**Team Chat:** [Add platform/group]

---

## ⚠️ Critical Rules

1. **Phase discipline:** Complete HTML before CSS, CSS before JavaScript
2. **Core setup priority:** Initialize core layout styles and data contracts early to enable parallel development
3. **Daily communication:** Update team on progress
4. **Test frequently:** Don't wait until the end; test each module continuously
5. **Git discipline:** Clear commits, pull before push
6. **Code review:** Review before merging
7. **Ask early:** Don't struggle alone

---

## 🏆 Project Status

**Architecture:** ✅ Expert academic level  
**Team:** ✅ 5 members assigned  
**Structure:** ✅ 53 files ready  
**Documentation:** ✅ Complete  
**Status:** 🟢 **READY TO START**

---

**Let's build something amazing!** 🚀✈️

**Project Start Date:** [Date]  
**Expected Completion:** [Date + 9 weeks]  
**Version:** 1.0
