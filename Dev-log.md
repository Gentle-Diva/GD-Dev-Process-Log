[Sep 10, 2026, 05:01] | My AI chat now starts/shows at the recent message, not the first.
[Sep 10, 2026, 04:39] | Delete the stale net_ptofit_summary made the details display on my screen, since there's a specific function that is called.
[Sep 10, 2026, 04:38] | Earlier, AI was failing to get accurate data for specified day or number of days. And a start and end date rectified the issue.
[Sep 10, 2026, 04:37] | The reason there was two was cos I added 'from date' and 'to date' to my function. So, when AI tries to retrieve data, it know when to start from and where to stop depending on request.
[Sep 10, 2026, 04:36] | I realized that the other details on my overview tab - expenses, cogs, damaged stock... were not showing anymore. Digging deep, I realized it was failing to call net_profit_summary from database as there are two parameters for it now. It couldn't decide which to call. It then failed to call.
[Sep 9, 2026, 14:37] | I adjust to have logging feedback be beneath the action done. Earlier, after logging sales, the feedback, 'sale logged' show at the bottom (it began with two actions - sale & restock, so it was visible). 
After additions, the feedback was no longer in sight and could make user thing it wasn't done and tries to relog, since there was no feedback. 
I moved the feedback (inline-feedback) to show beneath the field, action done.
[Sep 9, 2026, 14:34] | If the agent is unable to retrieve response at the back end, that is, it failed, my 'fetching...' button stays stuck. That could be misleading, making user maybe think its network or something but the backend RAG system already failed. No response so ever was gonna come.
So, I updated it to return the button to 'Ask' when there wouldn't be any response to fetch or retrieve.
[Sep 9, 2026, 14:31] | That's not a good UX. 
I then made adjustment for it. threadRef was added. This made my page load blank. No error message. Just blank. 
After checking my browser console, I discovered there was no ref for the threadRef. So, I added useRef to my React state at the top of my jsx. This restored the page.
[Sep 9, 2026, 14:29] | My AI chat thread was beginning at the top. Say, I have 15 conversations, its already a long list. However, when I open AI section, it starts at the top - the first message. I would have to scroll up to recent message.
[Sep 8, 2026, 08:36] | To my AI layer, I added the ability to get product stock. That wasn't there before. A business may want to ask about stock or related though live inventory are also on the app.
[Sep 8, 2026, 08:35] | Returned good can be traced accurately when logging as return. It adds back to existing stocks.
[Sep 8, 2026, 08:34] | AI layer has a better interface. Each question has its timestamp.
[Sep 8, 2026, 08:32] | Unlike before where questions asked can not be seen again or be referenced to, now there is memory and history.
[Sep 8, 2026, 08:31] | I added chat history and chat thread to my AI layer.
[Sep 8, 2026, 08:30] | I had back and forth testing out and ensuring my AI query addition was working accurately. Responding to questions a real user would ask.
[Sep 8, 2026, 08:30] | Profits are well calculated from cost of goods sold (cogs), damaged stock, expenses and the likes. Accurate calculation.
[Sep 8, 2026, 08:29] | Lotta progress made. Expenses are now reflecting on the dashboard.
[Aug 29, 2026, 21:12] | The live dashboard/chart will further have expenses, profits and other details the may need an overview.
[Aug 29, 2026, 21:10] | I also have expenses logging. A business would need to log expenses to be able to eventually get the real profit.
[Aug 29, 2026, 21:10] | I incorporated damaged goods logging. Returned good logging.
[Aug 29, 2026, 21:09] | Alright. So, the page was getting long. It'll be good to have them in sections. So, I had them in sections. When I want to ask AI, I click on it from the sidebar and the page opens. Same for other sections.
[Aug 22, 2026, 19:07] | Recent activities can now be seen. Yes, products the business no longer want to sell can now be deactivated. Deactivated instead of removed/deleted, so the history can still be accessible.
[Aug 22, 2026, 19:06] | I have expanded to include a 'add product' feature. If a new product is stocked.
[Aug 22, 2026, 16:57] | Now at this v1, I can successfully log a sale, log a restock, ask anything about the business, see my revenue flow in live chart.
[Aug 22, 2026, 16:02] | The tool (Get top product sub-workflow) was not responding to webhook call but was responding to manual call. I disconnected it in the main workflow. Unpublished it and reconnected back to main workflow. It ran successfully after republishing them.
[Aug 21, 2026, 21:00] | I am debugging a situation where AI agent is not able to call the right tool for a question asked via the dashboard but is correctly calling tools and answering questions handcoded in the agent.
[Aug 21, 2026, 20:25] | Now, I am debugging some stuff in the dashboard and n8n backend.
[Aug 21, 2026, 20:24] | I added my webhook url in the jsx.
[Aug 21, 2026, 20:24] | I added some jsx to my dashboard jsx in vs code. That wired intake for question about how the business is going.
[Aug 21, 2026, 16:05] | Now, I move to wiring in webhook. Yayy.
[Aug 21, 2026, 16:05] | I handcoded questions to the agent and it ran well. I used openai/gpt-oss-20b. I like the response.
[Aug 21, 2026, 16:04] | The build is with webhook but for test, before wiring in webhook, I used scheduled trigger and tested that the AI agent run that will fetch response from database in supabase through the sub-workflow call, will work.
[Aug 21, 2026, 16:02] | I opted for a main workflow call sub-workflows as tools to check up whatever request is made about the business - revenue, sales, low stock and the likes.
[Aug 21, 2026, 16:01] | While the live dashboard is built to an extent, I built in intake system in n8n.
[Aug 14, 2026, 12:24] | Logging sales and expenses. Seeing inventory live. Making requests for informed decisions. All on the interface.
[Aug 14, 2026, 12:22] | It will not only display business activities live, it will also have entries logging on it.
[Aug 14, 2026, 12:21] | I am planning on making the live dashboard more like a web app. Sort of an interactive interface.
[Aug 13, 2026, 10:14] | I am busy styling and debugging the backend of the dashboard build.
[Aug 12, 2026, 19:24] | I ran some commands in powershell to open launch a localhost for the dashboard.
[Aug 12, 2026, 16:09] | I am installing node. js.
[Aug 12, 2026, 16:09] | I am taking my time to understand the process and not just follow AI. I am using different tools to question/confirm another's output. Beyond copy and paste, understanding the workflow.
[Aug 12, 2026, 15:44] | In the process for live dashboard, I am creating a database in supabase. Vite and React.
[Aug 12, 2026, 15:44] | I set my hands on build a live dashboard using AI layer, React, Vite and Supabase.
[Aug 10, 2026, 18:25] | I just set up and discovered writing new content to a github file. I had back and forth getting the edit file node to add my existing file content and new entry directly from it until I introduced a code node. Noted.
Dev activity Log
