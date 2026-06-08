# PADME Chatbot Test Site
 
A dummy website for testing the PADME (Penicillin Allergy Decision & Mobile Empowerment) chatbot integration with Microsoft Copilot Studio.
 
## 📋 Overview
 
This is a simple test environment to validate:
- Chatbot functionality
- User interactions
- Survey flow logic
- Boundary language responses
- Mobile responsiveness
- Copilot Studio integration
## 🚀 Quick Start
 
### Option 1: Open Locally (No Server Needed)
1. Download `padme-test-site.html`
2. Double-click the file to open in your browser
3. Chat bubble appears in bottom-right corner
### Option 2: Run on Local Server
```bash
# Using Python 3
python -m http.server 8000
 
# Using Python 2
python -m SimpleHTTPServer 8000
 
# Using Node.js (with http-server)
npx http-server
```
 
Then visit: `http://localhost:8000/padme-test-site.html`
 
## 🔗 Copilot Studio Integration
 
### Step 1: Get Your Bot Credentials
 
1. Go to **Copilot Studio** → Find your chatbot
2. Click **Publish** or **Share**
3. Look for **Web** or **Embed** options
4. You should see:
   - **Bot ID**
   - **Tenant ID** (sometimes called "Environment ID")
   - A webChat code snippet (optional)
### Step 2: Add Credentials to HTML
 
Open `padme-test-site.html` and find this section:
 
```javascript
const BOT_CONFIG = {
    botId: 'YOUR_BOT_ID_HERE',
    tenantId: 'YOUR_TENANT_ID_HERE',
    channelId: 'webchat',
    conversationId: ''
};
```
 
Replace with your actual credentials:
 
```javascript
const BOT_CONFIG = {
    botId: 'a1b2c3d4-e5f6-7890-abcd-ef1234567890',
    tenantId: 'xyz789-tenant-id-here',
    channelId: 'webchat',
    conversationId: ''
};
```
 
### Step 3: Test the Integration
 
1. Open `padme-test-site.html` in your browser
2. Click the blue chat bubble in the bottom-right corner
3. The chatbot should load
4. Try test scenarios:
   - "Walk me through the survey"
   - "What does hives mean?"
   - "Help with question 5"
   - "Can you diagnose my allergy?" (should get boundary response)
   - "I'm having trouble breathing right now" (should get emergency response)
## 📝 What's Included
 
- **Clean Admin Interface**: Simple dashboard for testing
- **Chat Bubble**: Bottom-right corner, ready for Copilot Studio integration
- **Test Scenarios**: Pre-written test cases to validate chatbot responses
- **Responsive Design**: Works on desktop and mobile
- **Easy to Customize**: Simple HTML/CSS/JS - modify as needed
## 🎨 Customization
 
### Change Colors
Find this in the CSS:
```css
header {
    border-bottom: 3px solid #0066cc; /* Change this color */
}
```
 
### Change Chat Bubble Position
```css
.chat-bubble-container {
    bottom: 20px;  /* Distance from bottom */
    right: 20px;   /* Distance from right */
}
```
 
### Add More Test Content
Add new sections in the HTML:
```html
<div class="section">
    <h2>Your Section Title</h2>
    <p>Your content here</p>
</div>
```
 
### Change the Title/Branding
```html
<h1>🧬 PADME Chatbot Testing</h1>
<p>Your custom description</p>
```
 
## 🧪 Testing Checklist
 
- [ ] Chat bubble appears in bottom right
- [ ] Click opens chatbot (or shows setup instructions)
- [ ] Can send messages to chatbot
- [ ] Chatbot responds with appropriate answers
- [ ] Boundary language works (refuses medical advice)
- [ ] Emergency detection works
- [ ] Definitions and glossary terms work
- [ ] Mobile responsive (test on phone)
- [ ] No console errors
## 📱 Mobile Testing
 
The site is responsive and works on mobile. To test:
- Open on your phone browser, OR
- Use Chrome DevTools: Right-click → Inspect → Toggle device toolbar (Ctrl+Shift+M)
## 🔧 Troubleshooting
 
### Chat bubble doesn't open
- Make sure bot credentials are added to the JavaScript
- Check browser console for errors (F12)
- Verify Bot ID and Tenant ID are correct
### Chatbot loads but doesn't respond
- Check that the Copilot Studio bot is published
- Verify credentials in the HTML file
- Check browser console for API errors
### Need help?
- Ask Tim or Andy from AI Acceleration
- Check Copilot Studio documentation
- Review Copilot Studio embedding guide
## 📂 File Structure
 
```
padme-test-site/
├── README.md                    (you are here)
├── padme-test-site.html        (main test website)
└── .gitignore                  (optional)
```
 
## 🎯 Next Steps
 
1. **Add real bot credentials** (see Copilot Studio Integration section)
2. **Test with actual survey** - embed the PADME survey if needed
3. **Invite team to test** - share link with Dr. Kwan and team
4. **Collect feedback** - what works? what needs improvement?
5. **Iterate** - adjust design, content, functionality based on feedback
6. **Deploy** - once ready, can be hosted on GitHub Pages, Netlify, etc.
## 📊 Version History
 
- **v1.0** (May 2026): Initial dummy test site with chat bubble integration
## 👥 Team
 
- **Sanjana Chaudhary** - Lead Developer
- **Manasi Chaudhary** - Co-Developer
- **Dr. Mildred Kwan** - Project Lead
## 📧 Questions?
 
Create an issue in this repo or reach out to the team!
 
