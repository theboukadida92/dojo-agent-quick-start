# DOJO Agent

![DOJO Agent Banner](./dajo-agent-banner.png)

**DOJO Agent** is an AI web automation tool that runs in your browser. A free alternative to OpenAI Operator with flexible LLM options and multi-agent system.

<div align="center">
<img src="Dojo-Agent-bitcoin.gif" width="900" alt="DOJO Agent Demo GIF" />
<p><em>DOJO Agent’s multi-agent system tracks Bitcoin real time price in Coingecko, with the Coordinator self-correcting obstacles and guiding the Operator to adapt instantly—all running seamlessly in your browser.</em></p>
</div>

## 🚀 Features

- **Browser-Based AI Automation**: Runs directly in your browser as a Chrome extension
- **Multi-LLM Support**: Compatible with OpenAI, Claude, Gemini, and OpenRouter
- **Multi-Agent System**: Coordinate multiple AI agents for complex tasks
- **Free Alternative**: Open-source alternative to expensive AI automation tools
- **Real-Time Web Interaction**: Automate web tasks with live data and dynamic responses
- **Flexible Configuration**: Easy setup with multiple AI provider options
- **Privacy-Focused**: Your data stays in your browser

## 📋 Prerequisites

- Google Chrome browser
- Node.js (v18 or higher)
- npm or pnpm package manager
- API key from at least one supported LLM provider:
  - OpenAI API Key
  - Anthropic Claude API Key
  - Google Gemini API Key
  - OpenRouter API Key

## 🛠️ Installation

### Option 1: Install from Chrome Web Store (Recommended)

1. Visit the [Chrome Web Store](https://chrome.google.com/webstore) (coming soon)
2. Search for "DOJO Agent"
3. Click "Add to Chrome"
4. Follow the setup instructions

### Option 2: Install from Source

1. **Clone the main repository**:
   ```bash
   git clone https://github.com/theboukadida92/dojo-agent.git
   cd dojo-agent
   ```

2. **Install dependencies**:
   ```bash
   npm install
   # or
   pnpm install
   ```

3. **Build the extension**:
   ```bash
   npm run build
   # or
   pnpm build
   ```

4. **Load the extension in Chrome**:
   - Open Chrome and go to `chrome://extensions/`
   - Enable "Developer mode" (top right)
   - Click "Load unpacked"
   - Select the `dist` folder from the project

## ⚡ Quick Start

### 1. Configure Your AI Provider

1. **Click the DOJO Agent extension icon** in your Chrome toolbar
2. **Open Settings** from the extension popup
3. **Add your API key** for your preferred LLM provider:
   - **OpenAI**: Enter your OpenAI API key
   - **Claude**: Enter your Anthropic API key
   - **Gemini**: Enter your Google API key
   - **OpenRouter**: Enter your OpenRouter API key

### 2. Start Automating

1. **Navigate to any website** you want to automate
2. **Open the DOJO Agent side panel** (click the extension icon)
3. **Describe your task** in natural language, for example:
   - "Fill out this contact form with my information"
   - "Find and click all the product links on this page"
   - "Extract all email addresses from this page"
   - "Navigate to the checkout and complete the purchase"

### 3. Monitor and Control

- **Real-time feedback**: Watch as DOJO Agent performs actions
- **Step-by-step execution**: See each action being performed
- **Error handling**: Automatic retry and error recovery
- **Manual override**: Take control at any time

## 🔧 Configuration

### Environment Variables

Create a `.env` file in your project root:

```env
# Choose your preferred LLM provider
OPENAI_API_KEY=your_openai_api_key_here
ANTHROPIC_API_KEY=your_claude_api_key_here
GOOGLE_API_KEY=your_gemini_api_key_here
OPEN_ROUTER_API_KEY=your_openrouter_api_key_here
```

### Advanced Settings

- **Model Selection**: Choose specific models for different tasks
- **Temperature Control**: Adjust AI creativity and randomness
- **Timeout Settings**: Configure how long to wait for responses
- **Logging Level**: Control debug information visibility

## 🎛️ Model Parameters

DOJO Agent uses advanced AI model parameters to control the behavior and output quality of its three specialized agents. Understanding these parameters helps you optimize performance for different tasks.

### Temperature (0.0 - 1.0)

**Temperature** controls the randomness and creativity of AI responses:

- **Lower values (0.0 - 0.3)**: More focused, deterministic, and consistent responses
- **Medium values (0.4 - 0.7)**: Balanced creativity and reliability
- **Higher values (0.8 - 1.0)**: More creative, diverse, but potentially less predictable responses

### Top P (0.0 - 1.0)

**Top P** (nucleus sampling) controls response diversity by limiting the AI's token selection:

- **Lower values (0.1 - 0.5)**: More focused responses, considers fewer word choices
- **Medium values (0.6 - 0.8)**: Balanced diversity and focus
- **Higher values (0.9 - 1.0)**: Maximum diversity, considers all possible word choices

### Recommended Settings by Agent

#### 🎯 Coordinator Agent
- **Temperature**: 0.3 - 0.5 (Strategic planning requires consistency)
- **Top P**: 0.7 - 0.8 (Moderate diversity for creative problem-solving)
- **Use Case**: Task planning, strategy formulation, high-level decision making

#### ⚡ Operator Agent
- **Temperature**: 0.1 - 0.3 (Precise execution requires low randomness)
- **Top P**: 0.5 - 0.7 (Focused responses for accurate actions)
- **Use Case**: Web interactions, form filling, clicking elements, data extraction

#### ✅ QA Reviewer Agent
- **Temperature**: 0.2 - 0.4 (Consistent validation and error detection)
- **Top P**: 0.6 - 0.8 (Thorough analysis with moderate diversity)
- **Use Case**: Quality assurance, error detection, result validation, testing

### Parameter Tuning Tips

- **Start with recommended settings** and adjust based on your specific use case
- **Lower temperature** for tasks requiring precision (forms, data entry)
- **Higher temperature** for creative tasks (content generation, brainstorming)
- **Monitor performance** and adjust parameters if responses are too rigid or too unpredictable
- **Test different combinations** to find optimal settings for your workflow

## 💡 Usage Examples

### E-commerce Automation
```
"Add 3 blue t-shirts size medium to cart and proceed to checkout"
```

### Data Extraction
```
"Extract all product names and prices from this page into a table"
```

### Form Filling
```
"Fill out this registration form with: Name: John Doe, Email: john@example.com, Phone: 555-0123"
```

### Navigation
```
"Go to the pricing page and find the enterprise plan details"
```

## 🔗 Links

- **Main Repository**: [https://github.com/theboukadida92/dojo-agent](https://github.com/theboukadida92/dojo-agent)
- **Documentation**: [Full Documentation](https://github.com/theboukadida92/dojo-agent/wiki)
- **Issues & Support**: [GitHub Issues](https://github.com/theboukadida92/dojo-agent/issues)
- **Discussions**: [GitHub Discussions](https://github.com/theboukadida92/dojo-agent/discussions)

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](https://github.com/theboukadida92/dojo-agent/blob/main/CONTRIBUTING.md) for details.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/theboukadida92/dojo-agent/blob/main/LICENSE) file for details.

## ⚠️ Disclaimer

DOJO Agent is designed for legitimate automation tasks. Please ensure you comply with website terms of service and applicable laws when using this tool.

---

**Ready to automate the web with AI?** [Get started now!](https://github.com/theboukadida92/dojo-agent)
