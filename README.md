# 🛍️ AI Ecommerce Copy Crafter
**with OpenAI SDK**


🌐 **See the Live Application**: [https://ai-ecommerce-copy-crafter.vercel.app/](https://ai-ecommerce-copy-crafter.vercel.app/)

> **Transform product ideas into high-converting ecommerce copy instantly. Generate SEO-optimized titles, descriptions, and A+ content with AI—then ship directly to Shopify.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-15.1-black.svg)](https://nextjs.org/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ Features

### 🎯 **Core Functionality**
- 🤖 **AI-Powered Copy Generation** - Create multiple variants with OpenAI GPT-4
- 🎨 **Brand Voice Learning** - Analyze samples to match your brand tone automatically
- 🔑 **Smart Keyword Suggestions** - AI recommends SEO keywords based on your product
- 📊 **SEO Scoring & Analysis** - Real-time keyword density, readability, and optimization tips
- 🎯 **Variant Comparison Mode** - Side-by-side comparison with word-level diff highlighting
- 🎤 **Voice-to-Text Input** - Speak your product details using Whisper API transcription
- 📦 **Batch Generation** - Upload CSV to generate copy for multiple products at once
- 🛒 **Shopify Integration** - Export directly to your Shopify store (optional)

### 🎨 **Beautiful UI/UX**
- ✨ **Modern 2025 Design** - Glassmorphism, gradients, smooth animations
- 🌙 **Dark Mode** - Full theme support with system preference detection
- 📱 **Fully Responsive** - Optimized for desktop, tablet, and mobile
- ♿ **Accessible** - WCAG AA compliant with keyboard navigation
- 🎬 **Video Background** - Cinematic hero section with parallax effects
- 🎯 **Intuitive Interface** - Single-page app with smooth transitions

### 📊 **Advanced Features**
- 🔄 **Real-Time Streaming** - Watch AI generate copy in real-time with SSE
- ⚡ **AI Quality Scoring** - Automatic evaluation of clarity, persuasiveness, SEO
- 🎚️ **Customizable Generation** - Configure tone, audience, keywords, variant count
- 💾 **Persistent History** - All generations saved to Supabase database
- 🔍 **SEO Metrics** - Keyword density, Flesch-Kincaid readability, length analysis
- 🎭 **Brand Voice Presets** - Save and reuse your brand voice across projects
- 📝 **Copy-to-Clipboard** - One-click copy for any variant
- 🔄 **Regeneration** - Refine and regenerate specific variants

### 🚀 **Developer Features**
- 📡 **FastAPI Backend** - Modern async Python web framework
- 🔌 **RESTful API** - Well-documented endpoints with OpenAPI/Swagger
- 💾 **Redis Job Queue** - Background processing with Upstash Redis
- 🗄️ **Supabase Database** - PostgreSQL with real-time capabilities
- 🎯 **TypeScript Frontend** - Type-safe React with Next.js 15
- 🧪 **Error Handling** - Graceful fallbacks and user-friendly error messages

---

## 🏗️ Tech Stack

### **Backend** 🐍
- **FastAPI** - Modern Python web framework with async support
- **OpenAI API** - GPT-4 for copy generation, analysis, and transcription
- **Whisper API** - Speech-to-text for voice input
- **Python 3.11+** - Latest features and performance optimizations

### **Frontend** ⚛️
- **Next.js 15.1** - React 19 with App Router and server components
- **Tailwind CSS** - Utility-first styling with custom design system
- **shadcn/ui** - Beautiful, accessible component library
- **Framer Motion** - Smooth animations and transitions
- **Lucide Icons** - Modern, consistent icon set

### **Database & Cache** 💾
- **Supabase** - PostgreSQL with real-time capabilities and RLS
- **Upstash Redis** - Serverless Redis for job queue, caching, and rate limiting

### **External APIs** 🔌
- **Shopify Admin API** - Product export and synchronization
- **OpenAI GPT-4** - Copy generation and scoring
- **OpenAI Whisper** - Audio transcription

### **Deployment** 🚀
- **Railway** - Automated monorepo deployment with `railway.toml`
- **Vercel** - Frontend deployment with edge functions
- **GitHub Actions** - CI/CD pipeline (optional)
---

## 📖 User Guide

### 🎮 Basic Usage

#### Step 1: Enter Product Details
1. Navigate to the generator panel
2. Enter your product title (or use voice input 🎤)
3. Add a product description
4. (Optional) Add keywords manually or let AI suggest them

#### Step 2: Configure Generation
- **Tone**: Professional, Casual, Enthusiastic, Luxury
- **Audience**: General, Tech-Savvy, Budget-Conscious, Premium
- **Brand Voice**: Select a saved brand voice or create new
- **Variants**: Choose how many versions to generate (1-5)

#### Step 3: Generate Copy
1. Click **"Generate Copy"**
2. Watch real-time streaming as AI creates variants
3. Automatic SEO scoring and quality analysis
4. Review all generated variants

#### Step 4: Review & Export
- **Compare**: Select 2 variants for side-by-side comparison
- **Copy**: Click to copy any variant to clipboard
- **Export**: Send to Shopify or download as JSON
- **Regenerate**: Refine and create new variants

---

### 🎭 Brand Voice Learning

#### Create Your Brand Voice
1. Click **"Learn My Brand Voice"** button
2. Paste 2-5 sample texts from your brand (website, previous product descriptions, emails)
3. Click **"Analyze Brand Voice"**
4. AI analyzes tone, style, vocabulary, and patterns
5. Save with a memorable name (e.g., "Premium Tech Brand")

#### Use Brand Voice
1. Select saved brand voice from dropdown
2. AI automatically matches your brand's tone and style
3. All generated copy maintains consistent voice
4. Edit or delete saved voices anytime

---

### 🔑 Smart Keyword Suggestions

#### How It Works
1. As you type your product title/description
2. AI automatically suggests relevant keywords
3. Keywords are debounced (waits 1.5s after typing)
4. Click suggested keywords to add them
5. Keywords influence SEO scoring and generation

#### Manual Keywords
- Type and press Enter to add custom keywords
- Click × to remove keywords
- Mix AI suggestions with manual keywords

---

### 📊 SEO Analysis

Each variant automatically shows:
- **Overall Score** (0-100) with letter grade (A+, A, B, etc.)
- **Keyword Density** - Target vs actual usage
- **Readability** - Flesch-Kincaid reading ease
- **Content Length** - Character count and optimal range
- **Suggestions** - Actionable tips to improve SEO

Click the score badge to expand full analysis and suggestions.

---

### 🔄 Variant Comparison Mode

#### Compare Two Variants
1. Click **"Compare"** on any variant
2. Select a second variant to compare
3. View side-by-side with word-level differences:
   - **Red highlight** = Words only in left variant
   - **Green highlight** = Words only in right variant
   - **No highlight** = Common words
4. Click **"Exit Comparison"** to return

Perfect for A/B testing and choosing the best copy!

---

### 🎤 Voice-to-Text Input

#### Using Voice Input
1. Click the microphone 🎤 icon next to product title
2. Allow browser microphone access
3. Click **"Start Recording"**
4. Speak clearly about your product
5. Click **"Stop Recording"** when done
6. AI transcribes and fills in the product title
7. Edit transcription if needed

Uses OpenAI Whisper for high-accuracy transcription in 50+ languages.

---

### 📦 Batch Generation

#### Process Multiple Products
1. Click **"Batch Upload"** button
2. Drag & drop CSV file or click to browse
3. CSV format:
   ```csv
   title,description,keywords
   "Product 1","Description 1","keyword1,keyword2"
   "Product 2","Description 2","keyword3,keyword4"
   ```
4. Review parsed products
5. Click **"Start Batch Generation"**
6. Watch progress in real-time
7. Download results as JSON when complete

Perfect for migrating catalogs or bulk content creation!

---



---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** - Clean, bright interface
- 🌙 **Dark Mode** - Easy on the eyes with modern gradients
- 🖥️ **System** - Automatically follows OS preference

Toggle theme using the sun/moon icon in top-right corner.

---

### Generation Options

#### Tone Presets
- **Professional** - Business-focused, authoritative
- **Casual** - Friendly, conversational
- **Enthusiastic** - Energetic, exciting
- **Luxury** - Premium, sophisticated

#### Audience Presets
- **General** - Broad appeal
- **Tech-Savvy** - Technical details, specs
- **Budget-Conscious** - Value-focused, cost-effective
- **Premium** - Quality-focused, high-end

#### Customization
All presets are starting points—AI adapts based on:
- Product description
- Keywords
- Brand voice (if selected)
- Context clues

---

### Brand Voice Customization

#### What AI Analyzes
- **Tone**: Formal/casual, friendly/authoritative, etc.
- **Style**: Sentence length, paragraph structure
- **Vocabulary**: Industry terms, brand-specific words
- **Patterns**: Common phrases, formatting preferences

#### Tips for Better Results
1. **Use diverse samples** - Website, emails, social media
2. **Include 2-5 samples** - More = better analysis
3. **Use representative text** - Actual brand content, not generic
4. **Update regularly** - As your brand evolves

---



---

## 📚 Additional Resources

### Documentation
- [FastAPI Docs](https://fastapi.tiangolo.com/)
- [Next.js Docs](https://nextjs.org/docs)
- [OpenAI API Docs](https://platform.openai.com/docs)
- [Supabase Docs](https://supabase.com/docs)
- [Upstash Redis Docs](https://docs.upstash.com/redis)
- [Shopify Admin API](https://shopify.dev/docs/api/admin-rest)

### Tutorials
- [OpenAI Cookbook](https://cookbook.openai.com/)
- [React 19 Features](https://react.dev/blog/2024/12/05/react-19)
- [Tailwind CSS Best Practices](https://tailwindcss.com/docs/utility-first)

### Community
- [GitHub Discussions](https://github.com/derril-tech/ai-ecommerce-copy-crafter/discussions)
- [GitHub Issues](https://github.com/derril-tech/ai-ecommerce-copy-crafter/issues)

---

## 👨‍💻 Creator

**Created by Derril Filemon**

- 💼 LinkedIn: [Derril Filemon](https://linkedin.com/in/derril-filemon)
- 🐙 GitHub: [@derril-tech](https://github.com/derril-tech)

---

## 🙏 Acknowledgments

Special thanks to:
- **OpenAI** - For GPT-4 and Whisper API
- **Supabase** - For database and authentication
- **Upstash** - For serverless Redis
- **Railway** - For seamless deployment
- **Vercel** - For Next.js and hosting
- **shadcn** - For beautiful UI components
- **Lucide** - For consistent icons
- **Framer** - For smooth animations
- **Tailwind Labs** - For utility-first CSS

---

## 📄 License

This project is licensed under the **MIT License**.

See [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Derril Filemon

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📞 Support

Need help? We're here for you:

- 📧 **Email**: support@ecomcopycrafter.com
- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/derril-tech/ai-ecommerce-copy-crafter/issues)
- 💬 **Questions**: [GitHub Discussions](https://github.com/derril-tech/ai-ecommerce-copy-crafter/discussions)
- 📖 **Documentation**: [API Docs](https://your-api.railway.app/docs)

---

## ⚠️ Important Notes

### API Keys & Security
- **Never commit** `.env` files to Git
- **Use environment variables** for all secrets
- **Rotate keys** regularly for production
- **Enable RLS** (Row Level Security) in Supabase

### Rate Limits
- **OpenAI**: Depends on your plan (check dashboard)
- **Supabase**: 500MB database, 2GB bandwidth (free tier)
- **Upstash Redis**: 10K commands/day (free tier)

### Costs
- **OpenAI API**: ~$0.01-0.03 per generation (GPT-4)
- **Whisper API**: ~$0.006 per minute of audio
- **Supabase**: Free tier available, Pro at $25/month
- **Upstash Redis**: Free tier available, Pro at $0.20/100K commands
- **Railway**: ~$5-20/month depending on usage

### Best Practices
- **Use caching** to reduce API costs (already implemented)
- **Implement rate limiting** for production
- **Monitor usage** in OpenAI dashboard
- **Set budget alerts** to avoid surprises
- **Use job queue** for batch operations (already implemented)

---

<div align="center">

**⭐ Star this repo if you find it useful!**

**Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)**

[🏠 Home](https://ai-ecommerce-copy-crafter.vercel.app/) • [📖 Docs](https://github.com/derril-tech/ai-ecommerce-copy-crafter#readme) • [🐛 Issues](https://github.com/derril-tech/ai-ecommerce-copy-crafter/issues) • [💬 Discussions](https://github.com/derril-tech/ai-ecommerce-copy-crafter/discussions)

---

### 🚀 Ready to craft amazing product copy?

[**Try it now →**](https://ai-ecommerce-copy-crafter.vercel.app/)

</div>
