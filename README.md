# Clients-Sentiment-and-Reputation-Analysis
This project showcases a sophisticated data lifecycle management process, transitioning from raw unstructured data to high-impact business visualizations. By analyzing stakeholder sentiment across the Banking, MEA, and MoRTH sectors, the solution provides a data-driven framework for operational improvement and public relations management

## The "Why" Behind This Project
I wanted to build a project that didn't just start with a clean spreadsheet. In the real world, data is messy, hidden on web pages, or sometimes doesn't even exist yet. I decided to challenge myself by building a complete end-to-end pipeline—starting from raw HTML and ending with a high-level executive dashboard for the Banking, Foreign Affairs (MEA), and Transport (MoRTH) sectors.

## How I Built It (Step-by-Step)
### 1. Creating the "Messy" Source
I started by using Google Gemini to generate a realistic dataset of public feedback. To push my technical boundaries, I didn't just download a CSV; I converted that data into HTML format first. This allowed me to simulate a real-world scenario where a data analyst has to "hunt" for information on a website rather than having it handed to them.

### 2. The Extraction Phase
Using Python in Google Colab, I wrote a web scraper to "read" that HTML. It was a great exercise in navigating tags and structures to pull out the meaningful bits of information. I successfully converted that unstructured web data into a clean CSV format, which was the first big win of the project.

### 3. The "Dirty Work" (ETL in Excel)
We often hear that 80% of data work is cleaning, and this project proved it. I spent significant time in Excel performing the "heavy lifting":

Fixing Dates: I noticed the date formats were inconsistent, so I standardized them to ensure my time-series charts would actually work.

Handling the Gaps: I hunted down missing values and removed duplicates that would have skewed the results.

Normalizing for Comparison: I took the "Impact Weight" (which was in percentages) and normalized it so I could perform actual math on it later in Power BI.

### 4. Bringing the Data to Life in Power BI
This was my favorite part. Once the data was clean, I moved it into Power BI to see what stories the numbers were telling. I didn't just want "pretty charts"; I wanted tools that could solve business problems.

What the Visuals Actually Tell Us
When you look at the dashboard, you aren't just seeing colors; you’re seeing answers to tough business questions:

Is our reputation at risk? The Sentiment Donut Chart gives an instant "Pulse Check." If the negative segment grows, I know we need to call the PR team.

Which department needs help? By comparing Banking vs. MEA vs. MoRTH, I can see exactly which sector is struggling with public perception.

What is the "Root Cause"? My Treemap breaks things down by category. If people are unhappy in the MEA sector, the data shows me it’s specifically about Visa Services, not Diplomatic Relations. That’s the kind of detail that saves a manager’s time.

Are our policies working? The Trend Line allows us to see if sentiment improved after a specific policy was launched. It’s essentially a "report card" for government or bank decisions.

The Takeaway
This project taught me that being a Data Analyst isn't just about knowing Python or Power BI—it’s about the ability to take a "mess" of information and turn it into a clear, actionable roadmap for a business leader. I’m proud of how I handled every step, from the first line of scraping code to the final interactive filter.

## Project Link
https://app.powerbi.com/links/EzTnYg5jn2?ctid=533a5541-3f67-4f61-b095-0968b4060be9&pbi_source=linkShare
