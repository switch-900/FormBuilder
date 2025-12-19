# JSON Form Builder

A lightweight, browser-based tool for structured communication with AI assistants. Stop the back-and-forth—get all your questions answered in one clean form.

🔗 **[Live Demo](https://yourusername.github.io/json-form-builder/)**

## What is this?

JSON Form Builder transforms the way you communicate with AI assistants (ChatGPT, Claude, etc.) by using structured forms instead of endless back-and-forth messages.

### The Problem
- AI asks questions → You answer → AI asks more questions → Repeat 5+ times
- Information scattered across multiple messages
- Inefficient and time-consuming

### The Solution
1. AI provides a JSON schema with all questions upfront
2. You fill out a clean form with your answers
3. Export answers as JSON and paste back to AI
4. Work continues immediately—no more 20 questions

## Features

- ✅ **7 Field Types** - text, textarea, number, checkbox, checkboxes, radio, select
- 🔒 **100% Local** - Everything runs in your browser, no data sent anywhere
- 📋 **One-Click Copy** - Export answers JSON to clipboard instantly
- 🤖 **AI Prompt Generator** - Built-in prompt to teach AI assistants this workflow
- 🎨 **Clean UI** - Dark theme, responsive design, intuitive interface
- 💾 **No Dependencies** - Pure HTML/CSS/JavaScript, works anywhere

## Quick Start

### Option 1: Use GitHub Pages (Recommended)

1. Fork this repository
2. Go to Settings → Pages
3. Set Source to "main branch"
4. Visit `https://yourusername.github.io/json-form-builder/`

### Option 2: Download and Run Locally

1. Download `index.html` and `form-builder.html`
2. Open `index.html` in your browser
3. Click "Launch Form Builder"

### Option 3: Direct Form Builder

Just open `form-builder.html` directly in your browser—no server needed!

## How to Use

### For Users:

1. **Get the Schema** - Your AI assistant provides a JSON schema
2. **Build Form** - Paste schema into left panel, click "Build form"
3. **Fill It Out** - Answer all questions in the generated form
4. **Export** - Click "Copy answers JSON"
5. **Send to AI** - Paste the answers JSON back into your conversation

### For AI Assistants:

Use this schema format:

```json
{
  "version": "1.0",
  "title": "Your Form Title",
  "description": "Optional description",
  "fields": [
    {
      "id": "unique_key",
      "label": "Your question here",
      "type": "text|textarea|number|checkbox|checkboxes|radio|select",
      "required": true,
      "placeholder": "Optional hint",
      "help": "Optional help text",
      "options": [
        { "value": "opt1", "label": "Option 1" }
      ],
      "default": "optional default value"
    }
  ]
}
```

## Field Types

| Type | Description | Example Use |
|------|-------------|-------------|
| `text` | Single-line text input | Names, short answers |
| `textarea` | Multi-line text input | Long descriptions, URLs |
| `number` | Numeric input | Age, quantity, ratings |
| `checkbox` | Single yes/no toggle | Agreement, feature flags |
| `checkboxes` | Multiple selections | Features, preferences |
| `radio` | Single choice | Difficulty level, style |
| `select` | Dropdown menu | Categories, options |

## Example Schemas

### Website Design Questionnaire
```json
{
  "version": "1.0",
  "title": "Website Design Preferences",
  "fields": [
    {
      "id": "style",
      "label": "Choose design style",
      "type": "select",
      "required": true,
      "options": [
        { "value": "modern", "label": "Modern & minimal" },
        { "value": "bold", "label": "Bold & colorful" },
        { "value": "classic", "label": "Classic & elegant" }
      ]
    },
    {
      "id": "features",
      "label": "Required features",
      "type": "checkboxes",
      "options": [
        { "value": "mobile", "label": "Mobile responsive" },
        { "value": "dark_mode", "label": "Dark mode" },
        { "value": "animations", "label": "Animations" }
      ]
    }
  ]
}
```

### Project Requirements
```json
{
  "version": "1.0",
  "title": "Project Specifications",
  "fields": [
    {
      "id": "deadline",
      "label": "Project deadline",
      "type": "text",
      "placeholder": "e.g., 2 weeks, end of month"
    },
    {
      "id": "budget",
      "label": "Budget range",
      "type": "radio",
      "options": [
        { "value": "small", "label": "Small ($0-$1k)" },
        { "value": "medium", "label": "Medium ($1k-$5k)" },
        { "value": "large", "label": "Large ($5k+)" }
      ]
    },
    {
      "id": "details",
      "label": "Additional requirements",
      "type": "textarea",
      "placeholder": "Any other important details..."
    }
  ]
}
```

## Use Cases

- 🎨 **Creative Projects** - Lock in design direction and preferences
- 💻 **Development** - Specify tech requirements and constraints
- 📝 **Content Creation** - Define tone, audience, and structure
- 🎓 **Education** - Collect learning objectives and standards
- ⚙️ **Configuration** - Gather setup parameters and options

## Browser Compatibility

Works in all modern browsers:
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## Privacy

- **No data collection** - Everything runs locally in your browser
- **No analytics** - Zero tracking
- **No external requests** - Works completely offline after loading
- **No cookies** - Nothing stored unless you save schemas yourself

## Contributing

Pull requests welcome! Areas for improvement:
- Additional field types (date, time, color picker, etc.)
- Local storage for saving schemas
- Import/export functionality
- Template library
- Dark/light theme toggle

## License

MIT License - feel free to use this however you want!

## Credits

Created for efficient structured communication with AI assistants. Perfect for developers, designers, educators, and anyone who wants clearer AI conversations.

---

**[Launch Form Builder →](https://yourusername.github.io/json-form-builder/form-builder.html)**
