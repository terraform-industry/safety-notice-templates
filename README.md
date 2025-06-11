# 🛡️ Terraform Industries Safety Notice Templates

> **Standardized safety communication templates for high-risk operations across all TI teams**

## 📋 Overview

This repository contains official safety notice templates used by Terraform Industries for communicating hazards, safety protocols, and operational restrictions during high-risk testing and processes. These templates ensure consistent, clear, and comprehensive safety communication across all teams and stakeholders.

## 🏗️ Repository Structure

```
safety-notice-templates/
├── company-wide/              # Templates for company-wide notices
├── infra-site-logistics/      # Infrastructure and site logistics notices
├── teams/                     # Team-specific safety notices
│   ├── DAC/                   # Direct Air Capture team
│   ├── Reactor/               # Reactor team
│   └── Electrolyzer/          # Electrolyzer team
└── README.md                  # This file
```

## 🚀 Quick Start: Creating a New Safety Notice

### 1. Choose the Right Template
Navigate to the appropriate directory based on the scope of your safety notice:
- **Company-wide**: Affects all TI personnel
- **Infra/Site**: Related to facilities, utilities, or site access
- **Team-specific**: Affects only your team's operations

### 2. Fill Out the Template
Templates use square brackets `[PLACEHOLDER]` for customizable fields:

```markdown
🚨 **[DEPARTMENT] | [PROCESS NAME] | [HAZARD TYPE] | Start: [DAY, DATE TIME] | End: [OPTIONAL END TIME]** 🚨
```

Example:
```markdown
🚨 **DAC Team | THOR SiC Testing | High Temperature | Start: Mon, June 5 11:00 PST | End: Until Further Notice** 🚨
```

### 3. Required Information
- **Department/Team**: Who is conducting the operation
- **Process Name**: What is being tested/performed
- **Hazard Type**: Primary hazard category
- **Start Time**: When operations begin
- **End Time**: When operations end (or "Until Further Notice")
- **Location**: Specific area where hazards exist
- **Safety Officer**: Primary safety contact
- **Operator**: Primary equipment operator

## 📧 Email Distribution Guidelines

When sending safety notices via email to `everyone@terraformindustries.com`:

### Email Template
```
Subject: 🚨 SAFETY NOTICE: [HAZARD TYPE] - [PROCESS NAME] - [START DATE]

Team,

Please be advised of the following safety notice for operations beginning [DATE/TIME].

[Paste the completed safety notice template here]

Please acknowledge receipt of this notice and direct any questions to the listed safety contacts.

Stay safe,
[Your Name]
[Your Role]
```

### Best Practices
- ✅ Send notices **at least 24 hours** in advance when possible
- ✅ Use the 🚨 emoji in subject lines for visibility
- ✅ Include "SAFETY NOTICE" in all caps in the subject
- ✅ Request read receipts for critical notices
- ✅ Follow up with a reminder 1 hour before operations begin

## 🌿 Git Workflow for New Notices

### Creating a New Notice

1. **Create a feature branch**
   ```bash
   git checkout -b safety-notice/[team]-[date]-[brief-description]
   # Example: git checkout -b safety-notice/dac-2025-06-11-thor-high-temp
   ```

2. **Copy and customize the appropriate template**
   ```bash
   cp teams/DAC/high-temp-template.md teams/DAC/2025-06-11-thor-testing.md
   # Edit the file with your specific details
   ```

3. **Commit your changes**
   ```bash
   git add teams/DAC/2025-06-11-thor-testing.md
   git commit -m "Add safety notice for DAC THOR high-temp testing June 11"
   ```

4. **Push to GitHub**
   ```bash
   git push -u origin safety-notice/dac-2025-06-11-thor-high-temp
   ```

5. **Create a Pull Request**
   ```bash
   gh pr create --title "Safety Notice: DAC THOR Testing June 11" \
                --body "Adding safety notice for high-temperature testing scheduled for June 11"
   ```

### Reviewing and Merging

1. **Review Requirements**
   - ✅ All required fields are filled
   - ✅ Contact information is current
   - ✅ Hazards are clearly described
   - ✅ Safety perimeter is appropriate

2. **Merge Process**
   ```bash
   # After PR approval
   git checkout main
   git pull origin main
   git merge --no-ff safety-notice/dac-2025-06-11-thor-high-temp
   git push origin main
   ```

3. **Clean up**
   ```bash
   git branch -d safety-notice/dac-2025-06-11-thor-high-temp
   git push origin --delete safety-notice/dac-2025-06-11-thor-high-temp
   ```

## 🎨 Template Categories

### High-Temperature Operations
- Furnace testing
- Combustion experiments
- Thermal stress testing

### Chemical Hazards
- Corrosive materials handling
- Toxic gas operations
- Chemical synthesis

### Electrical Hazards
- High-voltage testing
- Arc flash risks
- Power system work

### Mechanical Hazards
- High-pressure systems
- Moving machinery
- Structural testing

## 🔐 Safety First Culture

Remember: **No experiment or deadline is worth compromising safety**

- Always err on the side of caution
- If you see something, say something
- Safety notices are living documents - update them as conditions change
- When in doubt, consult the Safety Officer

## 📞 Key Contacts

**Company Safety Officer**: [Update with current contact]  
**Emergency**: 911  
**Site Security**: [Update with current contact]  

## 🤝 Contributing

1. Keep templates generic and reusable
2. Document any new hazard types
3. Share lessons learned in team retrospectives
4. Suggest improvements via pull requests

---

*For questions about this repository or safety procedures, contact the TI Safety Committee*