# CharityTrends
A charity start up tool

## What it is and how it workds

Our tool provides a visual representation of public interest in various charities by analyzing the funds they've raised over the past decade. Here's how it works:

### Data Collection and Cleaning:
We gathered extensive datasets on charities and nonprofits, then used Python (NumPy and Pandas) to clean and process the data. This involved merging columns, filtering data, and extracting meaningful insights.

### Algorithm Development:
We created an algorithm using NumPy and Pandas to filter the charity databse based on keywords and compute the average funds raised by charities with similar missions. The algorithm is then able to generate a graph based on this data.

### User Input and Keyword Extraction:
On the frontend, we built an intuitive interface using React and Next.js. Users input sentences like, "I’d like to learn about charities focusing on water conservation." Our tool then processes the sentence with Google's Gemini large language model to identify relevant keywords.

### Data Analysis and Visualization:
These keywords are sent to an Express.js API, which triggers a Python script that run's our algorithm. As stated above, the algortihm searches the filtered charity database and generates a graph visualizing the average funds raised by charities with those keywords over the last 10 years.

### Insightful Graphs:
The resulting graph displays the general public interest in the chosen charity category based on fundraising success, helping users understand how much money specific causes have raised over time.

This tool empowers users to make informed decisions on where to donate or even start their own charity by showing the financial success of causes aligned with their values.


This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.