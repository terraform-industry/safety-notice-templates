# Reactor Team Safety Notices

This directory contains safety notice templates specific to Reactor team operations.

## Quick Reference

For detailed instructions, see the [main repository README](../../README.md).

## Reactor-Specific Hazards

Common hazards in Reactor operations include:
- High temperatures and pressures
- Chemical reactions and catalysts
- Thermal runaway risks
- Toxic gas generation
- Equipment overpressure scenarios

## Creating a New Notice - Command Line

```bash
# 1. Navigate to the repository
cd /path/to/safety-notice-templates

# 2. Create a new branch
git checkout -b safety-notice/reactor-[date]-[description]
# Example: git checkout -b safety-notice/reactor-2025-06-15-catalyst-testing

# 3. Copy a template or create new file
cp teams/Reactor/template.md teams/Reactor/2025-06-15-catalyst-test.md
# Or create from scratch
vim teams/Reactor/2025-06-15-catalyst-test.md

# 4. Stage and commit
git add teams/Reactor/2025-06-15-catalyst-test.md
git commit -m "Add safety notice for Reactor catalyst testing June 15"

# 5. Push to GitHub
git push -u origin safety-notice/reactor-2025-06-15-catalyst-testing

# 6. Create pull request
gh pr create --title "Safety Notice: Reactor Catalyst Testing June 15" \
             --body "Safety notice for scheduled catalyst performance testing"
```

## Creating a New Notice - GitHub Web Interface

1. **Navigate to this directory** on GitHub:
   - Go to `https://github.com/terraform-industry/safety-notice-templates`
   - Click into `teams` → `Reactor`

2. **Create a new file**:
   - Click "Add file" → "Create new file"
   - Name it with the pattern: `YYYY-MM-DD-brief-description.md`
   - Example: `2025-06-15-catalyst-testing.md`

3. **Use a template**:
   - Copy content from an existing template
   - Fill in all `[PLACEHOLDER]` fields
   - Preview using the "Preview" tab

4. **Commit the file**:
   - At the bottom, select "Create a new branch for this commit"
   - Name the branch: `safety-notice/reactor-[date]-[description]`
   - Click "Propose new file"

5. **Create Pull Request**:
   - Review your changes
   - Add any additional context in the PR description
   - Click "Create pull request"
   - Tag relevant team members for review

## Template Checklist

Before submitting your safety notice, ensure:
- [ ] All placeholder fields are filled
- [ ] Emergency contacts are current
- [ ] Hazard descriptions are specific to your process
- [ ] Safety perimeter is clearly defined
- [ ] PPE requirements match the hazards
- [ ] Start/end times are accurate

## Reactor Team Contacts

**Reactor Safety Lead**: [Update with current contact]  
**Reactor Operations Manager**: [Update with current contact]  
**24/7 Reactor Hotline**: [Update with number]

---

*For Reactor-specific safety questions, contact the Reactor Safety Lead*