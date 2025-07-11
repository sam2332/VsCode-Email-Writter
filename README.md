# Email Writer Project

An AI-powered email writing assistant that generates professional emails in multiple communication styles with proper file management and revision control.


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

### Fluid Workflow (Recommended)
This is the natural, conversational workflow that works best for quick email generation:

1. **Make a simple request**: Just tell the AI what you need in plain language
   ```
   "tell them that the web server is low on cpu speed and we need to buy a second one"
   ```

2. **Answer clarifying questions**: The AI will ask for key details using numbered questions:
   ```
   1. Who is the intended recipient?
   2. What's the urgency level?
   3. What's the current impact?
   4. Do you have any specific details?
   5. What's your preferred communication style?
   6. What timeline are you looking for?
   ```

3. **Provide quick answers**: Respond with numbered answers matching the questions:
   ```
   1. it manager
   2. moderate
   3. slow website performance, customer complaints, system crashes
   4. 89% constant cpu, 100% disk and 90% ram
   5. executive
   6. months?
   ```

4. **Get your email**: The AI automatically:
   - Selects the appropriate communication style
   - Applies the relevant instruction guidelines
   - Generates professional content
   - Saves with proper naming convention
   - Stores as plain text format

**Why this workflow is effective:**
- **Fast**: No need to research style names or instruction files
- **Natural**: Just describe what you need in your own words
- **Guided**: The AI asks the right questions to get all necessary context
- **Automatic**: Style selection and file management happen seamlessly
- **Professional**: Always produces polished, appropriate emails

### Traditional Usage (Alternative)
For users who prefer explicit control:
1. **Request Email Generation**: Specify the communication style and context, referencing the instruction files
2. **AI Processing**: The system applies appropriate guidelines and generates content
3. **Automatic Storage**: Email is saved with proper naming convention in plain text format
4. **Review and Revise**: Make changes and save as new revisions as needed


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


### Content Format
- **Plain Text Only**: No markdown formatting
- **Standard Email Structure**: To, From, Subject, Body
- **Clean Formatting**: Simple line breaks and spacing
- **No Markup**: No bold, italics, or other formatting syntax




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


---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Effective communication is the bridge between confusion and clarity. Choose the right style, and your message will always reach its destination.*
