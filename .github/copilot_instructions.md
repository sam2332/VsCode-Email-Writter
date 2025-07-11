# Email Writer Project - Copilot Instructions

## Project Overview
This project provides AI-powered email writing assistance with multiple communication styles and proper file management for generated emails.

## Email Writing Guidelines
When generating emails, follow these core principles:

1. **Style Selection**: Choose the appropriate email style based on context:
   - `technical-to-general` - For translating technical concepts to general audiences
   - `professional-business` - For formal business communications
   - `casual-friendly` - For warm, approachable communications
   - `urgent-crisis` - For time-sensitive crisis communications
   - `customer-support` - For empathetic customer service
   - `marketing-sales` - For prospect engagement and conversions
   - `executive-communication` - For strategic leadership communications

2. **Apply Style Instructions**: Reference the appropriate `.instructions.md` file in the `.github/instructions/` directory for detailed guidelines on language, tone, structure, and best practices.

## File Storage Requirements

### Email File Naming Convention
All generated emails MUST be stored using this exact naming pattern:
```
YYYY-MM-DD_subject-keywords_revision.txt
```

**Format Rules:**
- Date: Use ISO format (YYYY-MM-DD)
- Subject: Extract 2-4 key words from email subject, separated by hyphens
- Revision: Start with "v1", increment for each revision (v2, v3, etc.)
- Extension: Always use `.txt` (never `.md` or other formats)

**Examples:**
- `2025-07-11_project-update-meeting_v1.txt`
- `2025-07-11_server-downtime-alert_v1.txt`
- `2025-07-11_customer-support-refund_v2.txt`

### Content Format Requirements
- **No Markdown**: Store emails as plain text only
- **No formatting syntax**: No bold (**text**), italics (*text*), or other markdown
- **Basic text only**: Use simple line breaks and spacing for structure
- **Preserve email structure**: Keep standard email elements (To, From, Subject, Body)

### File Organization
- Store all emails in a dedicated `/emails/` directory
- Organize by year/month subdirectories if volume is high
- Example structure:
  ```
  /emails/
    /2025/
      /07/
        2025-07-11_project-update-meeting_v1.txt
        2025-07-11_server-downtime-alert_v1.txt
  ```

## Workflow Instructions

### When Creating New Emails:
1. Determine the appropriate communication style
2. Apply the relevant instruction guidelines
3. Generate the email content in plain text format
4. Save with proper naming convention
5. Confirm file is stored as `.txt` with no markdown formatting

### When Revising Emails:
1. Load the existing email file
2. Make requested changes following style guidelines
3. Save as new revision (increment version number)
4. Keep previous versions for reference

### Quality Checklist:
- [ ] Appropriate style guidelines followed
- [ ] File saved with correct naming convention
- [ ] Content is plain text only (no markdown)
- [ ] Email structure is clear and professional
- [ ] Revision number is accurate

## Important Notes
- Always prioritize clarity and appropriate tone for the intended audience
- When down-teching (technical-to-general), focus on benefits over features
- Maintain consistency within email threads and revisions
- Store ALL email variations, even minor edits, as separate revision files