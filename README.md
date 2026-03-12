# Product Department KPI Dashboard

A professional, interactive dashboard for tracking Product Department KPIs and initiatives. Built for monthly updates and executive presentations.

**Live Dashboard:** https://teefrye.github.io/product-kpi-dashboard/

---

## 📊 Dashboard Features

- **3 Key Metrics:** Roadmap Health, Approved Change Requests, Backlog Health
- **Manual Color Controls:** Override automatic status colors (green/yellow/red)
- **Top 10 Initiatives Tracker:** Expandable cards with status and commentary
- **Auto-Change Calculation:** Tracks month-over-month changes
- **N/A Support:** Mark metrics as not applicable when needed
- **Responsive Design:** Works on desktop, tablet, and mobile

---

## 🚀 How to Use

### **Monthly Update Workflow (2 minutes)**

1. **Open the Dashboard**
   - Navigate to your GitHub Pages URL
   - Bookmark it for quick access

2. **Click "📊 Update Period"**
   - Saves current month as baseline
   - Enables automatic change calculation
   - Check "Skip change calculation" for first entry

3. **Click "✏️ Edit KPI Data"**
   - Update **Reporting Period** (e.g., "February 2026" or "Feb 1-15, 2026")
   - Enter current metric values
   - Adjust **Status Colors** using the colored buttons
   - Check **N/A** boxes for metrics without data

4. **Update Initiatives (Optional)**
   - Click any initiative card to expand
   - Edit name, status, or add commentary
   - Click card again to collapse

5. **Click "✓ Done Editing"**
   - Changes auto-save to browser
   - Dashboard updates immediately

6. **Take Screenshot**
   - Use for presentations or backup

---

## 💾 Data Storage

### **Current Setup (Phase 1):**
- **Data stored in:** Browser localStorage
- **Persists:** As long as you don't clear browser cache
- **Accessible from:** Same browser/device only
- **Backup method:** Screenshots or manual Excel copy

### **Important Notes:**
- Use the same browser/device each month for data persistence
- Clearing browser cache will delete your data
- Different browsers = different data (not synced)

---

## 🎨 Customizing Your Dashboard

### **Manual Status Colors**

Each metric has 3 color buttons (🟢 🟡 🔴) in the edit panel:
- **Green:** On track / Good status
- **Yellow:** Warning / Needs attention  
- **Red:** Off track / Critical

Click any color to override the automatic calculation.

### **Initiative Management**

**To Edit an Initiative:**
1. Click the initiative card to expand
2. Edit **Name**, **Status**, or **Commentary**
3. Changes save automatically

**Commentary Tips:**
- Add context, blockers, or updates
- First 60 characters show in collapsed view
- Full text visible when expanded

---

## 📋 Phase 2: Excel Integration (Future)

### **What This Enables:**
- Edit data in Excel (OneDrive)
- Dashboard reads from Excel automatically
- Access from any device
- Automatic backup via OneDrive
- Team collaboration on data entry

### **Setup Steps (30 minutes):**

1. **Create Excel File**
   ```
   Create file: kpi-data.xlsx in OneDrive
   
   Sheet 1: KPIs
   | Month      | Year | Roadmap_Current | Roadmap_Target | ... |
   |------------|------|-----------------|----------------|-----|
   | January    | 2026 | 18              | 26             | ... |
   ```

2. **Register Azure App**
   - Go to Azure Portal → App Registrations
   - Create new registration
   - Name: "Product KPI Dashboard"
   - Get Client ID
   - Set redirect URL: Your GitHub Pages URL

3. **Update Dashboard Code**
   - Add Microsoft Graph API integration
   - Configure authentication
   - Test connection

4. **Connect Dashboard**
   - One-time Microsoft 365 login
   - Grant read access to Excel file
   - Dashboard pulls data on refresh

### **Monthly Workflow After Phase 2:**
1. Open Excel file in OneDrive
2. Add new row with month's data
3. Open dashboard → auto-updates
4. Done! (~1 minute)

---

## 📈 Phase 3: Advanced Features (Future)

### **Potential Enhancements:**

**Export Features:**
- 📄 Export to PDF
- 📊 Export to PowerPoint
- 📥 Download as CSV

**Visualization Improvements:**
- 📉 Trend charts (last 6 months)
- 📊 Year-over-year comparison
- 🎯 Goal tracking progress bars

**Collaboration:**
- 👥 Multi-user access to shared Excel
- 💬 Comments on initiatives
- 📧 Email notifications for updates

**Automation:**
- ⚡ Auto-populate from Jira/Azure DevOps
- 🔄 Scheduled data refresh
- 📱 Mobile app version

---

## 🛠️ Making Changes

### **To Update Dashboard Design/Features:**

**Method 1: Edit on GitHub**
1. Click `index.html` in repository
2. Click pencil icon (Edit)
3. Make changes
4. Commit → Changes live in 2 minutes

**Method 2: Ask Claude**
1. Return to our chat conversation
2. Describe what you want changed
3. Claude provides updated `index.html`
4. Replace file on GitHub

### **Common Updates:**
- Add/remove metrics
- Change colors or fonts
- Adjust layout
- Add new features
- Fix bugs

---

## 🔐 Security & Privacy

### **What's Public:**
- Dashboard code (HTML/CSS/JavaScript)
- Design and layout
- Feature names

### **What's Private:**
- Your actual KPI numbers
- Initiative names and commentary
- All data entered in edit panel

**Data never leaves your browser** until you implement Phase 2 (Excel integration with your OneDrive).

---

## 📞 Support & Maintenance

### **For Help:**
- Return to the original Claude conversation
- Create new chat and reference this dashboard
- Check GitHub Issues tab (if enabled)

### **Common Issues:**

**Dashboard is blank:**
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Check browser console for errors
- Verify GitHub Pages is enabled

**Data disappeared:**
- Check if you're on the same browser/device
- Browser cache may have been cleared
- Restore from screenshot or manual backup

**Colors not updating:**
- Click "Done Editing" to save changes
- Hard refresh the page
- Check color buttons are selected

---

## 📁 File Structure

```
product-kpi-dashboard/
├── index.html          # Main dashboard file
├── README.md          # This file
└── (future files)
    ├── kpi-data.xlsx  # Phase 2: Excel database
    └── config.js      # Phase 2: API configuration
```

---

## 🗓️ Version History

**v1.0 - January 2026**
- Initial release
- 3 KPI metrics with manual color controls
- Top 10 initiatives with expandable cards
- localStorage persistence
- Monthly update workflow

**v2.0 - [Future]**
- Excel/OneDrive integration
- Multi-device sync
- Automatic data refresh

**v3.0 - [Future]**
- Trend visualization
- Export features
- Enhanced collaboration

---

## 💡 Tips & Best Practices

### **For Monthly Updates:**
1. **Consistency:** Update on the same day each month
2. **Backup:** Take screenshots before updating
3. **Documentation:** Add initiative commentary for context
4. **Review:** Check previous month's data before updating

### **For Presentations:**
1. **Screenshot:** Capture dashboard at right zoom level
2. **Annotation:** Add notes/arrows in PowerPoint if needed
3. **Print Mode:** Consider adding a print-friendly CSS (Phase 3)

### **For Data Integrity:**
1. **Single Source:** Keep one browser as "source of truth"
2. **Manual Backup:** Export to Excel monthly
3. **Validation:** Double-check numbers before finalizing

---

## 🎯 Goals for 2026

- ✅ Q1: Use dashboard for monthly EMT presentations
- ⬜ Q2: Implement Excel integration (Phase 2)
- ⬜ Q3: Add trend visualization
- ⬜ Q4: Full automation with system integration

---

## 📝 Notes

**Created:** December 2024  
**Last Updated:** December 2024  
**Maintained by:** Travis  
**Built with:** HTML, CSS, JavaScript  
**Hosted on:** GitHub Pages  
