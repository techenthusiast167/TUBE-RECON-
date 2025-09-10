# TUBE-RECON

The YouTube OSINT Reconnaissance Tool is a powerful Python-based open source intelligence gathering utility designed to extract valuable information from YouTube channels, videos, and search results. This tool enables cybersecurity professionals, researchers, and investigators to conduct comprehensive digital footprint analysis through YouTube's platform.

- - - 

# YouTube OSINT Reconnaissance Tool

**Table of Contents**

- Overview
               
- Features

- Importance in OSINT & Cybersecurity

- Installation

- Usage Guide

- API Setup

- Output Examples

- Contributing

- Disclaimer

---

# FEATURES

**Video Analysis**:

- Extract comprehensive video metadata (title, description, statistics)

- Retrieve and analyze video comments

- Calculate engagement metrics and performance analytics

- Identify related videos and content recommendations

- Extract social media handles from video descriptions

- - - 

**Channel Analysis**:

- Gather complete channel metadata and statistics

- Analyze subscriber growth and engagement patterns

- Extract uploaded videos and playlists

- Scan channel descriptions for contact information

- Identify social media connections and website links

- - -

**Search Functionality**:

- Search across YouTube videos, channels, and playlists

- Extract intelligence from multiple sources simultaneously

- Aggregate social media findings from search results

- Export comprehensive data for further analysis

- - - 

**Profile Analysis (Digital Footprint)**:

- Profile Image Extraction: Download high-quality YouTube profile pictures

- Google Dorking Automation: Generate targeted search queries across platforms

- Cross-Platform Discovery: Find targets on Twitter, Instagram, Facebook, LinkedIn, TikTok

- Document Intelligence: Search for PDFs, DOCs, and other files related to target

- Email & Phone Extraction: Discover contact information from descriptions

- - - 

**Social Media Intelligence**:

- **Twitter**: Extract @handles and profile links

- **Instagram**: Identify Instagram accounts and links

- **Facebook**: Discover Facebook pages and profiles

- **TikTok**: Find TikTok usernames and profiles

- **Discord**: Extract server invites and community links

- **Telegram**: Identify Telegram channels and groups

- **Websites**: Capture all mentioned websites and domains

- **Email Addresses**: Extract email contacts

- **Phone Numbers**: Discover phone numbers from content

- - - 

**Data Export Capabilities**:

- JSON exports for complete data preservation

- CSV files for spreadsheet analysis

- Organized social media handle extraction

- Automated report generation

- Structured output folder organization

- Profile image downloads

- - - 

# Importance in OSINT & Cybersecurity

^^Digital Footprint Analysis**:

YouTube has become a critical platform for digital presence, making it an essential source for:

- Person of Interest Investigations:

- Track individuals' online activities

- Brand Monitoring: Protect organizational reputation

- Threat Intelligence: Identify potential security threats

- Social Engineering Defense: Understand public information exposure

- - - 

**Cybersecurity Applications**:

- **Attack Surface Mapping**: Identify publicly available information

- **Social Media Intelligence (SOCMINT)**: Gather platform-specific intelligence

- Incident Response: Investigate digital evidence during security incidents

- **Background Checks**: Verify individual claims and credentials

- **Threat Actor Profiling**: Build comprehensive profiles of malicious actors

- - - 
**Law Enforcement & Research**:

 
- **Evidence Collection**: Gather digital evidence from public sources

- **Trend Analysis**: Monitor emerging topics and communities

- **Network Mapping**: Identify connections between individuals and groups

- **Pattern Recognition**: Detect behavioral patterns across platforms

- **Digital Forensic Analysis**: Support investigations with multimedia evidence

- - - 

# Installation

- Python 3.8 or higher

**Starting the Tool**

- Create and activate your virtual environment
- Follow the link below, copy and install the tool script manually using nano:
  **https://gist.github.com/techenthusiast167/8b0d962184f8e32d99dbcc687a81545e**

- **Example**:
- **nano tuberecon.py**
- Press **Ctrl + O, Enter, Ctrl + X** to exit. 

**Install core dependencies**

    pip3 install google-api-python-client isodate requests beautifulsoup4

**Verify installation (OPtional)**:

    python3 -c "import googleapiclient.discovery; import isodate; print('Dependencies installed successfully!')"

---

# API Key Setup

**1. Create Google Cloud Project**

- Visit Google Cloud Console > https://console.cloud.google.com/

**2. Create a new project or select existing one**

- Enable "YouTube Data API v3"

- Generate API Credentials

- Navigate to **"APIs & Services" → "Credentials"**

- Click **"Create Credentials" → "API Key"**

- Copy your generated API key

**3. Set Environment Variable**

**Linux**

    export YOUTUBE_API_KEY="your_actual_api_key_here"


---

# Usage Guide

**Run the tool**

    python3 tuberecon.py


---

# YouTube OSINT Menu Overview


**Option 1: Video Analysis**:

**Purpose: Deep analysis of individual YouTube videos**

**How to Use**:

- **1. Select option 1 from the main menu**

- Enter YouTube video URL or ID when prompted

- Example: https://youtu.be/VIDEO_ID or just VIDEO_ID

**2. The tool will automatically**:

- Extract video metadata and statistics

- Download and analyze comments

- Identify related videos

- Extract social media handles

- Calculate engagement metrics

**3. Output Includes**:

- Video title, description, and metadata

- View count, likes, comments statistics

- Upload date and duration information

- Comment analysis and user engagement

- Social media handles found

- Related video recommendations

---

**Option 2: Channel Analysis**

**Purpose: Comprehensive channel investigation and profiling**

**How to Use**:

- **1. Select option 2 from the main menu**

- **2. Enter channel URL, ID, or username**

- **Examples**:

- Channel URL: https://www.youtube.com/channel/CHANNEL_ID

- Custom URL: https://www.youtube.com/c/ChannelName

- Username: @ChannelName

- **3. The tool will automatically**:

- Gather channel metadata and statistics

- Extract uploaded videos and playlists

- Analyze channel description for contacts

- Scan for social media connections

**Output Includes**:

 - Channel name, description, and creation date

- Subscriber count and view statistics

- Video upload history and content analysis

- Playlist information and organization

- Social media handles and website links

- Engagement metrics and growth patterns

---

**Option 3: Search Videos/Channels**

**Purpose: Broad investigation across YouTube content**

**How to Use**:

- **1. Select option 3 from the main menu**

- **2. Enter your search query**

- **Examples**:

- Person name: **John Smith**

- Topic: **cybersecurity tutorials**

- Location: **New York vlog**

- Event: **DEF CON 2023**

- **3. The tool will automatically**:

- Search across videos, channels, and playlists

- Extract social media from all results

- Aggregate findings from multiple sources

- Provide comprehensive intelligence report

**Output Includes**:

 - Search results across all content types

- Aggregated social media intelligence

- Content relevance scoring

- Export of all discovered information

- Organized data for further analysis

---

**Option 4: Profile Analysis (Digital Footprint)**

**Purpose: Comprehensive digital footprint mapping and profile intelligence**

**How to Use**:

- **1. Select option 4 from the main menu**

- **2. Enter YouTube channel URL, ID, username, or target name**

- **Examples**:

- YouTube channel: **https://www.youtube.com/@ChannelName**

- Target name: **John Smith**

- Channel ID: **UCxxxxxxxxxxxxxx**

- **3. The tool will automatically**:

- Extract profile image (if YouTube channel)

- Generate Google dorking queries

- Search across multiple social platforms

- Extract email and phone information

- Create comprehensive digital footprint report

**Output Includes**:

- Profile image download (if available)

- Google dorking queries for multiple platforms

- Social media presence across 10+ platforms

- Email addresses and phone numbers

- Document discoveries (PDF, DOC, etc.)

- Comprehensive digital footprint analysis
---

# Command Line Usage ( customize your search )

**Analyze specific video**:

    python3 tuberecon.py --video "https://youtu.be/VIDEO_ID"

**Analyze specific channel**:

    python3 tuberecon.py --channel "channel_name_or_url"

**Search for content**:

    python3 tuberecon.py --search "search query"

**Profile analysis**:

    python3 tuberecon.py --profile "target_name_or_channel"

**Example investigations**:

    python3 tuberecon.py --search "John Smith cybersecurity"
    python3 tuberecon.py --channel "https://youtube.com/@TargetChannel"
    python3 tuberecon.py --video "dQw4w9WgXcQ"
    python3 tuberecon.py --profile "John Smith"

---

# Output Examples


**Sample Video Analysis Output**:

=== VIDEO ANALYSIS SUMMARY ===
Video ID: dQw4w9WgXcQ
Title: Never Gonna Give You Up
Channel: RickAstleyVEVO
Published: 2009-10-24T20:00:00Z
Duration: PT3M33S
Views: 1,400,000,000
Likes: 18,000,000
Comments: 800,000
Engagement Rate: 1.34%

=== SOCIAL MEDIA HANDLES FOUND ===
TWITTER    : @rickastley, @sonymusic
INSTAGRAM  : rickastley
WEBSITE    : rickastley.co.uk, sonymusic.com
Output ExamplesOutput Examples

---
# Sample Channel Analysis Output

=== CHANNEL ANALYSIS SUMMARY ===
Channel ID: UCU8OZsd0LxO7oN2Z8GX9ZQw
Title: Tech Tutorials
Published: 2015-03-15T10:30:00Z
Subscribers: 450,000
Videos: 287
Views: 25,000,000
Avg Views Per Video: 87,108.00

=== SOCIAL MEDIA HANDLES FOUND ===
TWITTER    : @techtutorials
DISCORD    : techtutorials
PATREON    : techtutorials
WEBSITE    : techtutorials.com

---

# Sample Profile Analysis Output

=== PROFILE ANALYSIS SUMMARY ===
Target: John Smith
Channel Title: John's Tech Reviews
Subscribers: 125,000
Videos: 84

=== SOCIAL MEDIA HANDLES FOUND ===
TWITTER    : @johnsmithtech
INSTAGRAM  : johnsmithtech
EMAIL      : john.smith@email.com

=== GOOGLE DORKING RESULTS ===
Generated 12 custom search queries

Open these searches in your browser:
• "John Smith" site:twitter.com
  https://www.google.com/search?q=%22John+Smith%22+site%3Atwitter.com
• "John Smith" site:instagram.com
  https://www.google.com/search?q=%22John+Smith%22+site%3Ainstagram.com
• "John Smith" site:linkedin.com
  https://www.google.com/search?q=%22John+Smith%22+site%3Alinkedin.com

  ---

# Contributing

**We welcome contributions to enhance the YouTube OSINT Tool**:

- Fork the repository

- Create a feature branch: git checkout -b feature-name

- Commit changes: git commit -am 'Add new feature'

- Push to branch: git push origin feature-name

- Submit a pull request

---

# Suggested Improvements

- Additional social media platform support

- Enhanced data visualization

- Advanced search filters

- Batch processing capabilities

- Integration with other OSINT tools

- Machine learning for pattern recognition

- Enhanced image analysis capabilities

---

# Disclaimer

**Legal and Ethical Use**

**This tool is designed for**:

- Legitimate cybersecurity research

- Authorized investigations

- Educational purposes

- Personal learning and development


---

# Usage Restrictions

❌ Do not use for illegal activities

❌ Do not violate terms of service

❌ Do not harass or stalk individuals

❌ Do not access private information without authorization

❌ Do not use for unauthorized penetration testing

❌ Do not violate privacy laws

---

# Compliance Requirements

**Users must ensure**:

- Compliance with local laws and regulations

- Respect for privacy and data protection laws

- Appropriate authorization for investigations

- Ethical handling of collected information

- Responsibility for proper use of the tool

---

# Responsibility

**The developers are not responsible for**:

- Misuse of this tool

- Legal violations by users

- Any damages caused by improper use

- Consequences of unauthorized investigations

- Violations of terms of service

- Any legal repercussions from tool usage

---

- **Created by Tech Enthusiast** 

- For questions or support, please open an issue on the GitHub repository
