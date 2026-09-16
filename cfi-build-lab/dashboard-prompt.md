# Order Pulse dashboard · the prompt (v2, CFI brand)

Paste this into a new Cowork task with Microsoft 365 connected. Replace OneDrive with SharePoint if that's where your folder is.

    Build me an artifact called "CFI Order Pulse": a one-page dashboard that reads cfi-orders-weekly-v1.csv in my OneDrive folder "Build Lab" every time it opens.

    STYLE, follow CFI brand: white background, black text, Helvetica for all headings and labels, Georgia for the short story text. A CFI Yellow (#FFCE2E) keyline under the title. Green (#1E8449) for anything improving, red (#E63C2F) for anything worsening, and nothing else in color. Big numbers, small uppercase labels with letter-spacing. Generous white space. It should feel like a printed executive page, not a BI tool.

    SECTION 1, the headline. Above everything, one plain-English sentence about this week, written like a newspaper headline, generated from the data. Example shape: "Bookings dipped 5% as Con Forms slowed; Tricon kept climbing." Under it, two sentences of story: what moved, what drove it (name the business unit and region), and the one thing to watch next week. Simple words, no jargon.

    SECTION 2, four tiles: total bookings latest week, change vs prior week (dollar and percent), total backlog, average on-time. Every change has a filled arrow, green if better, red if worse. Under each number, a four-word plain-English caption, e.g. "down for the first time in four weeks".

    SECTION 3, bookings by business unit, last four weeks, one line per unit, Helvetica labels at the line ends. Annotate the chart: put a small callout on the biggest move (e.g. "Con Forms -31%") right at the turn, in red or green. Beside the chart, one card per unit with the latest number, a colored arrow with the percent, and a five-word reason if the data shows one (which region or product family moved).

    SECTION 4, a table by region and product family for the latest week, sortable by any column. Color the on-time cell red when below 91% and green when above 96%. Highlight the top three rows by bookings with a faint yellow tint.

    SECTION 5, at the bottom, "What to look at Monday": two bullets generated from the data, plain English, each ending with a question the leadership team could ask.

    Footer: a small line saying which file it read and when. If the file cannot be reached, show one clear message naming the file and folder instead of empty tiles.

Then: open it, note the headline, close it. Upload v2 renamed as v1 into the same folder. Reopen. The headline rewrites itself.
