# Electrolyzer Team Safety Notices

This directory contains safety notice templates specific to Electrolyzer team operations.

## Quick Reference

For detailed instructions, see the [main repository README](../../README.md).

## Electrolyzer-Specific Hazards

Common hazards in Electrolyzer operations include:
- High-voltage electrical systems
- Hydrogen gas generation and accumulation
- Oxygen-enriched environments
- Caustic electrolyte solutions
- Arc flash and electrocution risks
- Explosive gas mixtures

## Creating a New Notice - Command Line

```bash
# 1. Navigate to the repository
cd /path/to/safety-notice-templates

# 2. Create a new branch
git checkout -b safety-notice/electrolyzer-[date]-[description]
# Example: git checkout -b safety-notice/electrolyzer-2025-06-20-stack-testing

# 3. Copy a template or create new file
cp teams/Electrolyzer/template.md teams/Electrolyzer/2025-06-20-stack-test.md
# Or create from scratch
vim teams/Electrolyzer/2025-06-20-stack-test.md

# 4. Stage and commit
git add teams/Electrolyzer/2025-06-20-stack-test.md
git commit -m "Add safety notice for Electrolyzer stack testing June 20"

# 5. Push to GitHub
git push -u origin safety-notice/electrolyzer-2025-06-20-stack-testing

# 6. Create pull request
gh pr create --title "Safety Notice: Electrolyzer Stack Testing June 20" \
             --body "Safety notice for high-voltage stack performance testing"
```

## Creating a New Notice - GitHub Web Interface

1. **Navigate to this directory** on GitHub:
   - Go to `https://github.com/terraform-industry/safety-notice-templates`
   - Click into `teams` → `Electrolyzer`

2. **Create a new file**:
   - Click "Add file" → "Create new file"
   - Name it with the pattern: `YYYY-MM-DD-brief-description.md`
   - Example: `2025-06-20-stack-testing.md`

3. **Use a template**:
   - Copy content from an existing template
   - Fill in all `[PLACEHOLDER]` fields
   - Pay special attention to electrical safety requirements
   - Preview using the "Preview" tab

4. **Commit the file**:
   - At the bottom, select "Create a new branch for this commit"
   - Name the branch: `safety-notice/electrolyzer-[date]-[description]`
   - Click "Propose new file"

5. **Create Pull Request**:
   - Review your changes
   - Add any additional context in the PR description
   - Click "Create pull request"
   - Tag relevant team members for review

## Template Checklist

Before submitting your safety notice, ensure:
- [ ] All placeholder fields are filled
- [ ] Electrical hazard warnings are prominent
- [ ] Gas monitoring requirements are specified
- [ ] Ventilation requirements are clear
- [ ] Lock-out/tag-out procedures referenced
- [ ] Arc flash boundaries defined (where applicable)
- [ ] Emergency shower/eyewash locations noted

## Special Considerations

⚡ **Electrical Safety**: All Electrolyzer operations require qualified electrical personnel
🔥 **Hydrogen Safety**: Ensure proper ventilation and gas detection systems are active
🧪 **Chemical Safety**: Have spill kits and neutralizing agents readily available

## Electrolyzer Team Contacts

**Electrolyzer Safety Lead**: [Update with current contact]  
**Electrical Safety Officer**: [Update with current contact]  
**Electrolyzer Operations Manager**: [Update with current contact]  
**Emergency Electrical Hotline**: [Update with number]

---

*For Electrolyzer-specific safety questions, contact the Electrolyzer Safety Lead*