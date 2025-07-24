# Landed - Job Search Landing Page

A beautiful, animated landing page for the Landed job search platform built with React, Tailwind CSS, and Lucide icons.

## 🌐 **Connecting to landed.quest Domain**

### Option 1: GitHub Pages (Recommended - Free)

1. **Create a GitHub repository:**
   - Go to GitHub and create a new repository named `landed-website`
   - Make it public
   - Upload your `index.html` file

2. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Select "Deploy from a branch" → main branch → / (root)
   - Click Save

3. **Add custom domain:**
   - In Pages settings, add `landed.quest` as custom domain
   - This creates a CNAME file in your repo

4. **Configure DNS in Squarespace:**
   - Go to your Squarespace domain settings for landed.quest
   - Add these DNS records:
     ```
     Type: CNAME
     Host: www
     Points to: [your-username].github.io
     
     Type: A
     Host: @
     Points to: 185.199.108.153
     Points to: 185.199.109.153
     Points to: 185.199.110.153
     Points to: 185.199.111.153
     ```

### Option 2: Netlify (Also Free)

1. **Deploy to Netlify:**
   - Go to [netlify.com](https://netlify.com)
   - Drag and drop your `index.html` file
   - Get your Netlify URL

2. **Add custom domain:**
   - In Netlify dashboard: Domain settings → Add custom domain
   - Enter `landed.quest`

3. **Configure DNS:**
   - Point your domain to Netlify's DNS servers or add CNAME record

### Option 3: Squarespace (Paid but Integrated)

1. **Use Squarespace's built-in hosting**
2. **Create a Code Block page**
3. **Paste your HTML code**
4. **Domain automatically connects**

## 🛠️ **Current Features**

- **Supabase Integration**: Connected to user_signups database
- **7-Question Survey**: Captures user preferences and background
- **Fireworks Success Animation**: Celebration screen with beta messaging
- **Responsive Design**: Works on all devices
- **Real-time Validation**: Email verification and error handling

## 📧 **Database Structure**

Your signups are stored in Supabase with:
- `email` - User's email address
- `answers` - JSON object with survey responses  
- `signup_source` - Always 'landing_page'
- `created_at` / `updated_at` - Timestamps

## 🚀 **Next Steps**

1. Choose hosting option above
2. Set up domain connection
3. Test the live site
4. Monitor signups in your Supabase dashboard

---

**Need help?** The current setup is ready to go live - just needs hosting and domain connection! 