# Email Writer Project

An AI-powered email writing assistant that generates professional emails in multiple communication styles with proper file management and revision control.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Communication Styles](#communication-styles)
- [Getting Started](#getting-started)
- [Important: Referencing Instruction Files](#important-referencing-instruction-files)
- [Customizing Email Formats](#customizing-email-formats)
- [File Management](#file-management)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)

## Overview

This project provides AI-powered email writing assistance that helps you craft effective emails for different audiences and purposes. The system automatically applies appropriate communication styles, saves emails with proper naming conventions, and maintains revision history for all generated content.

## Features

- **AI-Powered Email Generation**: Intelligent email composition using advanced language models
- **Multiple Communication Styles**: Seven distinct email styles for different contexts and audiences
- **Customizable Email Formats**: Modify instruction files to tailor email styles to your organization's needs
- **Automatic File Management**: Proper naming conventions and revision control
- **Plain Text Storage**: Clean, markdown-free email storage for maximum compatibility
- **Style Guidelines Integration**: Built-in adherence to professional communication standards
- **Revision Tracking**: Maintain complete history of email iterations

## Communication Styles

The system supports seven distinct communication styles, each with detailed guidelines:

### 1. **Technical-to-General** (`technical-to-general`)
- **Purpose**: Translate complex technical concepts for non-technical audiences
- **Key Features**: Uses analogies, avoids jargon, focuses on benefits over features
- **Best For**: Explaining technical issues to stakeholders, status updates to management

### 2. **Professional Business** (`professional-business`)
- **Purpose**: Formal business communications
- **Key Features**: Formal tone, proper hierarchy, structured format
- **Best For**: Executive communications, legal matters, official announcements

### 3. **Casual Friendly** (`casual-friendly`)
- **Purpose**: Warm, approachable team communications
- **Key Features**: Conversational tone, personal touches, relationship building
- **Best For**: Team updates, internal communications, networking

### 4. **Urgent Crisis** (`urgent-crisis`)
- **Purpose**: Time-sensitive crisis communications
- **Key Features**: Clear urgency indicators, immediate action focus, direct language
- **Best For**: System outages, security incidents, critical issues

### 5. **Customer Support** (`customer-support`)
- **Purpose**: Empathetic customer service communications
- **Key Features**: Understanding tone, solution-focused, helpful approach
- **Best For**: Issue resolution, customer inquiries, support tickets

### 6. **Marketing Sales** (`marketing-sales`)
- **Purpose**: Engaging prospects and driving conversions
- **Key Features**: Value-focused, compelling CTAs, relationship building
- **Best For**: Lead generation, product announcements, sales outreach

### 7. **Executive Communication** (`executive-communication`)
- **Purpose**: Strategic leadership communications
- **Key Features**: Bottom-line-up-front, decision-oriented, business impact focus
- **Best For**: Board updates, strategic decisions, executive briefings

## Getting Started

### Prerequisites
- VS Code with Copilot or compatible AI assistant
- Access to the email writing guidelines in `.github/instructions/`

### Basic Usage
1. **Request Email Generation**: Specify the communication style and context, referencing the instruction files
2. **AI Processing**: The system applies appropriate guidelines and generates content
3. **Automatic Storage**: Email is saved with proper naming convention in plain text format
4. **Review and Revise**: Make changes and save as new revisions as needed

### Example Request
```
"Write a technical-to-general email explaining a database performance issue to stakeholders. 
Use the technical-to-general.instructions.md guidelines."
```

The system will:
- Load and apply the technical-to-general communication guidelines from the instruction file
- Generate appropriate content with analogies and simple language
- Save as `2025-07-11_database-performance-issue_v1.txt`
- Store in plain text format without markdown

### Proper Request Format
When requesting emails, always include:
- **Style specification**: Reference the exact instruction file (e.g., `professional-business.instructions.md`)
- **Context**: What the email is about and who it's for
- **Special requirements**: Any specific details or customizations needed

**Format:**
```
"Write a [style-name] email about [topic] for [audience]. 
Use the [style-name].instructions.md guidelines."
```

## Important: Referencing Instruction Files

**Critical for Proper Email Generation**: Always include the specific instruction file name in your email requests to ensure the AI applies the correct communication style and formatting guidelines.

### Why This Matters
- **Consistency**: Ensures emails follow your organization's specific guidelines
- **Customization**: Applies any modifications you've made to the instruction files
- **Quality**: Guarantees the AI uses the complete style framework rather than generic formatting
- **Predictability**: Produces consistent results based on your defined standards

### Correct Request Format
```
"Write a [communication style] email about [topic] for [audience]. 
Use the [style-name].instructions.md guidelines."
```

### Available Instruction Files
- `technical-to-general.instructions.md` - For translating technical concepts
- `professional-business.instructions.md` - For formal business communications  
- `casual-friendly.instructions.md` - For warm, approachable communications
- `urgent-crisis.instructions.md` - For time-sensitive crisis communications
- `customer-support.instructions.md` - For empathetic customer service
- `marketing-sales.instructions.md` - For prospect engagement and conversions
- `executive-communication.instructions.md` - For strategic leadership communications

### What Happens Without Instruction File Reference
If you don't specify an instruction file, the AI may:
- Use generic email formatting
- Miss your organization's specific requirements
- Apply inconsistent styling
- Ignore customizations you've made to the instruction files

**Always include the instruction file reference for best results!**

## File Management

### Naming Convention
All emails use this standardized naming pattern:
```
YYYY-MM-DD_subject-keywords_revision.txt
```

**Components:**
- **Date**: ISO format (YYYY-MM-DD)
- **Subject Keywords**: 2-4 key words from email subject, hyphen-separated
- **Revision**: Version number (v1, v2, v3, etc.)
- **Extension**: Always `.txt` for plain text storage

### Examples
- `2025-07-11_project-update-meeting_v1.txt`
- `2025-07-11_server-downtime-alert_v1.txt`
- `2025-07-11_customer-support-refund_v2.txt`

### Directory Structure
```
/emails/
  /2025/
    /07/
      2025-07-11_project-update-meeting_v1.txt
      2025-07-11_server-downtime-alert_v1.txt
      2025-07-11_customer-support-refund_v1.txt
      2025-07-11_customer-support-refund_v2.txt
```

### Content Format
- **Plain Text Only**: No markdown formatting
- **Standard Email Structure**: To, From, Subject, Body
- **Clean Formatting**: Simple line breaks and spacing
- **No Markup**: No bold, italics, or other formatting syntax

## Usage Examples

### Team Communication Email
```
User: "Write an email to my team about the migration of the website.org webserver on aug 2nd. 
Use the casual-friendly.instructions.md guidelines."

AI Response: I'll write a team communication email about the website.org webserver migration on August 2nd. 
Since this is an internal team update, I'll use the casual-friendly style to maintain a warm, 
approachable tone while providing the necessary technical information.

Generated File: 2025-07-example-webserver-migration_v1.txt
Content Highlights:
- Warm greeting: "Hi team! Hope everyone's having a great week!"
- Clear migration details with friendly explanations
- Specific action items in conversational tone
- Supportive closing: "Thanks for being such an awesome team"
```

### Professional Business Communication
```
User: "Write a professional business email requesting a meeting with the board about Q3 results. 
Use the professional-business.instructions.md guidelines."

AI Response: I'll create a formal business email for your board meeting request using 
professional business communication standards.

Generated File: 2025-07-11_board-meeting-q3-results_v1.txt
Content Highlights:
- Formal salutation: "Dear Board Members"
- Clear purpose statement in opening paragraph
- Structured agenda and meeting details
- Professional closing: "Best regards"
```

### Technical Issue Explanation
```
User: "Explain the API rate limiting issue to the marketing team. 
Use the technical-to-general.instructions.md guidelines."

AI Response: I'll translate the technical API issue into terms the marketing team can 
easily understand, using analogies and focusing on business impact.

Generated File: 2025-07-11_api-rate-limiting-issue_v1.txt
Content Highlights:
- Highway toll booth analogy for rate limiting
- Focus on user impact rather than technical details
- Clear next steps for marketing team
- No technical jargon or complex terminology
```

### Customer Support Response
```
User: "Write a customer support email about a refund request for a cancelled order. 
Use the customer-support.instructions.md guidelines."

AI Response: I'll create an empathetic customer support response that acknowledges 
their frustration and provides a clear resolution path.

Generated File: 2025-07-11_customer-refund-request_v1.txt
Content Highlights:
- Empathetic opening: "I understand how frustrating this must be"
- Clear explanation of refund process
- Specific timeline and next steps
- Offer for additional assistance
```

### Crisis Communication
```
User: "Write an urgent email about the database server outage affecting our main application. 
Use the urgent-crisis.instructions.md guidelines."

AI Response: I'll create an urgent crisis communication with clear urgency indicators 
and immediate action focus.

Generated File: 2025-07-11_database-server-outage_v1.txt
Content Highlights:
- Subject: [URGENT] Database Server Outage - Immediate Action Required
- Immediate issue statement and impact assessment
- Current status and resolution timeline
- Clear escalation path and contact information
```

## Contributing

We welcome contributions to improve the email writing assistant! Here's how you can help:

### Ways to Contribute
- **New Communication Styles**: Add specialized styles for specific industries or contexts
- **Enhanced Guidelines**: Improve existing style instructions with better examples
- **Template Library**: Create reusable email templates for common scenarios
- **Bug Fixes**: Report and fix issues with file naming or content generation
- **Documentation**: Improve this README or add usage examples

### Contributing Guidelines
1. **Fork the Repository**: Create your own copy to work on
2. **Create Feature Branch**: Use descriptive branch names
3. **Follow Style Guidelines**: Maintain consistency with existing patterns
4. **Test Examples**: Verify email generation works correctly
5. **Submit Pull Request**: Include clear description of changes

### File Structure Guidelines
When adding new instruction files:
- Place in `.github/instructions/` directory
- Use descriptive filename ending in `.instructions.md`
- Follow the established YAML frontmatter format
- Include comprehensive examples and guidelines

### Testing Your Changes
- Generate sample emails using your new styles
- Verify proper file naming and storage
- Test with different scenarios and recipients
- Ensure plain text output format

## Customizing Email Formats

One of the key features of this email writing assistant is the ability to **modify and customize email formats** by editing the instruction files. Each communication style is defined by a detailed instruction file that you can customize to match your organization's specific needs.

### How Instruction Files Work

Each communication style has its own instruction file in `.github/instructions/` that defines:
- **Language guidelines** - Tone, vocabulary, and phrasing
- **Structure requirements** - Email organization and format
- **Content principles** - What to emphasize or avoid
- **Examples and templates** - Real-world usage patterns

### Modifying Email Formats

To customize how emails are generated for any style:

1. **Navigate to** `.github/instructions/` directory
2. **Open** the relevant `.instructions.md` file for your target style
3. **Edit** the guidelines to match your preferences:
   - Change tone requirements
   - Modify structure templates
   - Add company-specific language
   - Update examples and best practices
4. **Save** your changes - the AI will immediately use your updated guidelines
5. **Test** by requesting emails that specifically reference your modified instruction file

### Example Request After Customization
```
"Write a professional business email about the quarterly review meeting. 
Use the professional-business.instructions.md guidelines."
```

The AI will apply your customized guidelines from the instruction file, ensuring consistent formatting according to your organization's standards.

### Example: Customizing Professional Business Style

**Default Professional Business Format:**
```markdown
## Structure Requirements
1. **Subject line**: Specific, action-oriented, professional
2. **Salutation**: "Dear [Title] [Last Name]" or "Good morning/afternoon [Name]"
3. **Opening**: State purpose clearly in first paragraph
4. **Body**: Organized paragraphs with logical flow
5. **Call to action**: Clear next steps or requests
6. **Professional closing**: "Best regards," "Sincerely," "Kind regards"
```

**Your Custom Format** (edit `professional-business.instructions.md`):
```markdown
## Structure Requirements
1. **Subject line**: Include [COMPANY] prefix for internal emails
2. **Salutation**: Always use "Good morning/afternoon [First Name]" for colleagues
3. **Opening**: Include project code reference in first line
4. **Body**: Use bullet points for action items, numbered lists for processes
5. **Call to action**: Include specific deadlines and responsible parties
6. **Company closing**: "Best regards," followed by department signature
```

### Common Customizations

#### **Company Branding**
- Add company-specific terminology
- Include standard disclaimers or signatures
- Modify greeting and closing conventions

#### **Industry Standards**
- Adapt to regulatory requirements
- Include required compliance language
- Adjust formality levels for your sector

#### **Team Preferences**
- Change tone from formal to conversational
- Add emoji guidelines for casual communications
- Modify urgency indicators and escalation paths

#### **Cultural Adaptations**
- Adjust for different time zones and regions
- Include cultural sensitivity guidelines
- Modify holiday and greeting references

### Creating New Communication Styles

You can create entirely new communication styles by:

1. **Copy** an existing instruction file as a template
2. **Rename** it with your new style name (e.g., `legal-compliance.instructions.md`)
3. **Modify** all sections to match your new style requirements
4. **Test** by requesting emails that reference your new instruction file:
   ```
   "Write a legal compliance email about data retention policies. 
   Use the legal-compliance.instructions.md guidelines."
   ```

### Advanced Customization Examples

#### **Sales Team Customization**
```markdown
# Marketing/Sales Email Writing Guidelines - Enterprise B2B Focus

## Core Principles
- **ROI-focused**: Always include quantifiable business benefits
- **Enterprise language**: Use "solution," "partnership," "strategic value"
- **Compliance aware**: Include required legal disclaimers
- **Relationship building**: Reference previous interactions and mutual connections

## Structure Requirements
1. **Subject line**: Include company name and specific value proposition
2. **Opening**: Reference mutual connection or previous conversation
3. **Value section**: Lead with ROI metrics and case studies
4. **Social proof**: Include customer logos and testimonials
5. **CTA**: Schedule specific meeting types (demo, ROI analysis, etc.)
6. **Signature**: Include multiple contact methods and calendar link
```

#### **Technical Documentation Style**
```markdown
# Technical Documentation Email Guidelines

## Language Guidelines
- Use precise technical terminology with definitions
- Include relevant error codes and system specifications
- Reference specific documentation versions and links
- Provide step-by-step troubleshooting procedures

## Structure Requirements
1. **Subject**: Include system name, issue type, and severity level
2. **Environment details**: OS, software versions, configuration
3. **Problem description**: Steps to reproduce, expected vs actual behavior
4. **Diagnostic information**: Logs, screenshots, error messages
5. **Solution steps**: Numbered procedures with verification steps
6. **Follow-up**: Testing timeline and escalation contacts
```

### Testing Your Customizations

After modifying instruction files:

1. **Generate test emails** using your customized style by specifically referencing the instruction file:
   ```
   "Write a customer support email about a refund request. 
   Use the customer-support.instructions.md guidelines."
   ```
2. **Review output** to ensure changes are applied correctly
3. **Iterate** on your instructions for better results
4. **Share with team** for feedback and consistency

### Best Practices for Customization

- **Start small**: Make incremental changes rather than complete rewrites
- **Test thoroughly**: Generate multiple email types to verify consistency
- **Always reference instruction files**: Include the `.instructions.md` file name in your requests
- **Document changes**: Keep notes on what modifications you made and why
- **Version control**: Consider backing up original instruction files
- **Team alignment**: Ensure all team members understand the customized formats and how to reference them



---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Effective communication is the bridge between confusion and clarity. Choose the right style, and your message will always reach its destination.*
