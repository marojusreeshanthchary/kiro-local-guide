# The Local Guide - KIRO Prototype
## Visakhapatnam Local Guide AI

A hyperlocal AI assistant that understands Visakhapatnam's culture, slang, and local nuances.

---

## PROJECT STRUCTURE

```
kiro-local-guide/
├── index.html                 # Main interactive prototype
├── product.md                 # Knowledge base (Visakhapatnam)
├── README.md                  # Project documentation
├── /.kiro/                    # KIRO configuration directory
│   ├── system-prompt.txt      # KIRO system instructions
│   ├── slang-map.json         # Local slang dictionary
│   ├── context-vizag.json     # Visakhapatnam knowledge base
│   └── intent-patterns.json   # Intent detection patterns
├── /docs/
│   ├── SETUP.md               # Setup instructions
│   ├── ARCHITECTURE.md        # Technical design
│   └── BLOG_POST_TEMPLATE.md  # AWS Builder Center blog outline
└── package.json               # Project metadata (optional)
```

---

## QUICK START

### 1. **Extract ZIP file**
```bash
unzip kiro-local-guide.zip
cd kiro-local-guide
```

### 2. **Open in browser**
```bash
# Simply open index.html in any browser
open index.html
```

Or run a local server:
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server
```

Then visit: `http://localhost:8000`

---

## WHAT'S INSIDE

### **index.html** (Interactive Prototype)
- Live chatbot interface
- Slang translator
- Food recommender
- Traffic estimator
- Hangout spot guide
- Conversation history

**Features:**
✅ Understands Telugu-English mix  
✅ Detects local slang automatically  
✅ Recommends based on time/budget  
✅ Shows reasoning from product.md  
✅ Mobile responsive  
✅ No backend required (client-side only)  

### **product.md** (Knowledge Base)
Complete Visakhapatnam local information:
- 🗣️ Slang & phrases
- 🍛 Street food with prices
- 🏖️ Hangout spots & vibes
- 🚌 Transport options
- ⏰ Best times for activities
- 💰 Budget breakdowns
- 🎯 Local behavior etiquette

### **/.kiro/ directory**
Configuration files for KIRO:
- `system-prompt.txt` - Role & behavior definition
- `slang-map.json` - Slang to meaning mapping
- `context-vizag.json` - Structured knowledge base
- `intent-patterns.json` - Intent detection rules

---

## HOW IT WORKS

### Intent Detection Flow
```
User Input
    ↓
Slang Detection (Match against slang-map.json)
    ↓
Intent Classification (Food? Travel? Hangout? Slang?)
    ↓
Context Lookup (Query product.md knowledge base)
    ↓
Response Generation (Formatted in local tone)
    ↓
Display with Reasoning
```

### Example Interaction

**User:** "Anna, light ga emaina night time lo thinali?"

**Detection:**
- Slang: "Anna" (respectful address)
- Slang: "light ga" (light food)
- Time: "night time" (after 8 PM)

**Response:**
"Seri, thammudu! Night lo light food ki, Maggi + Chai (₹30-50) or Samosa (₹10-20) best option. Old City lo 24-hour stalls unte. RTC lo madathey—bus cheppi vellipovu."

---

## CUSTOMIZATION

### For Other Cities

1. **Rename product.md** to your city's context
2. **Update slang-map.json** with local slang
3. **Update context-vizag.json** with local data
4. **Modify system-prompt.txt** for city-specific behavior

### For Enhanced Features

- Add voice input (Web Speech API)
- Add Google Maps integration
- Add real-time transit data
- Add user preferences saving (localStorage)
- Connect to actual food delivery APIs

---

## FOR HACKATHON SUBMISSION

### GitHub Setup
1. Create repo: `kiro-local-guide`
2. Push all files
3. Ensure `/.kiro` is NOT in .gitignore
4. Add comprehensive README
5. Include SETUP.md for judges

### AWS Builder Center Blog
Structure:
- **Problem:** Why hyperlocal AI matters
- **Solution:** How KIRO works
- **Implementation:** Code snippets from index.html
- **Demo:** Screenshots or video recording
- **Results:** What you learned
- **Code snippets:** Focus on slang detection, intent classification
- **Visuals:** Show Kiro UI, local slang in action

### Dashboard Submission
- GitHub repo link
- Blog post link (Published on AWS Builder Center)
- Brief description of your implementation

---

## TECHNICAL STACK

- **Frontend:** HTML5 + CSS3 + Vanilla JavaScript (ES6+)
- **Storage:** JSON (embedded in HTML)
- **No Dependencies:** Runs anywhere, no npm required
- **Responsive:** Mobile-first design
- **Accessibility:** WCAG 2.1 compliant

---

## KEY FILES EXPLAINED

| File | Purpose |
|------|---------|
| index.html | Full interactive prototype with embedded logic |
| product.md | Knowledge base for Visakhapatnam |
| /.kiro/system-prompt.txt | KIRO's role & instructions |
| /.kiro/slang-map.json | Slang dictionary |
| /.kiro/context-vizag.json | Structured local knowledge |
| /.kiro/intent-patterns.json | Intent detection patterns |
| README.md | Project overview |
| /docs/SETUP.md | Setup & deployment instructions |
| /docs/ARCHITECTURE.md | Technical design document |
| /docs/BLOG_POST_TEMPLATE.md | AWS blog outline |

---

## TESTING

### Test Queries
Try these to see KIRO in action:

**Slang:**
- "Enti ra, eppatlo vasthava?"
- "Light ga emaina thinali"
- "Heavy ga unbaya?"

**Food:**
- "Breakfast lo emaina bagundi?"
- "Night time lo kharchu etuvanti?"
- "Beach side food emundi?"

**Travel:**
- "RK Beach ki eppatlo time peduthey?"
- "Old City ki auto etuvanti?"

**Hangouts:**
- "Chill spot cheppu, night time lo"
- "Budget lo hangout spot?"

---

## SUPPORT

For issues or questions:
1. Check SETUP.md
2. Review product.md structure
3. Verify /.kiro/ files are present
4. Test in Chrome/Firefox (latest versions)

---

## LICENSE

Open source for hackathon & learning purposes.

---

**Built with ❤️ for AI for Bharat Challenge**  
**Last Updated:** December 2025