# NSS-DA6-Abi-Capstone
My repository for my capstone project for my Nashville Software School Data Analytics Bootcamp

Please note that this ReadMe will update as project progresses.

**Executive Summary**

As a life-long lover of the arts and a certifiable rows-and-columns person, I am planning to do a deep dive into the data that makes the performing arts industry tick – specifically the statistics about Broadway plays and musicals. I’m interested in analyzing patterns and trends in revenue, audience capacity, length of run, count of cast members, etc. to hopefully find some key indicators that would help someone predict the success and/or failure of a production. Are musicals more successful than straight plays? Are totally original works better investments than stage adaptations or jukebox musicals? **what makes a Broadway show successful?**

*Stretch goal:* in a perfect world, I would be able to cross-reference in-theater performance data with respective cast recording data, to evaluate patterns between successful musicals and popular stage soundtracks. In the past, popular stage productions tend to have cast recordings that end up being very popular in turn. However, I have noticed that this trend has started to shift to the reverse with the rise of digital streaming: a soundtrack may gain internet notoriety before the stage production has even gotten on its feet, and the popularity and social media buzz becomes a huge driver in the success of the musical. I’m interested in diving into this idea more, but it may be too much to accomplish.

**Motivation**

I have been a less-than-secretive theatre nerd since my early teen years. Most of my career thus far has been in the performing arts industry, and while I am looking to transition away from that path, it still holds a near and dear place in my heart. One of the companies that I interned with in college had a paid subscription to the Theatrical Index (a resource with huge amounts of data for Broadway, Off-Broadway, and touring productions) and the interns were encouraged to spend our time between projects perusing the statistics and trends. With my music business background and my love for the arts, I’ve always been completely intrigued by all the moving pieces that go into the success and failure of stage shows, and would love to dive into those intricacies with this project.

**Data Question**

Truthfully, I think my initial exploratory data analysis will help clear up what question I’m seeking to answer, but I think it will be along these lines:
1.	Are some Broadway theaters (the buildings) home to more successful shows than others? If so, why?
2.	What differentiated between shows that could reopen after the COVID-19 shutdown and shows that could not?
3.	Is box office success always an indicator of Tony Award success?
4.	Is it better for a show to have a big cast or a small cast? A big audience or a small audience?
5.	**What makes a show successful?**
6.	What gives long-running shows (ex, Phantom of the Opera, The Lion King, Chicago) such great success?
7.	Are musicals consistently more successful than straight plays? Are totally original works better options for investors than stage adaptations or jukebox musicals? What types of shows are good investments?
These types of questions are top of mind for any Broadway producer or investor, since the answers to these questions will ultimately drive profit. I have found plenty of articles about what makes a great show – good plot, excellent characters and acting performances, interesting choreography, or fresh design – but all these are all relatively subjective answers, and I’m wondering if there is a concrete trend to find at all.

**Minimum Viable Product (MVP)**

In my head, there are two potentials for a minimum viable product, dependent on what direction the data leads me.

In one lane, I would love to make a series of interactive dashboards (either through Excel, PowerBI, Tableau, or maybe Python) that allows a user to make selections (a particular venue, a particular season, a particular actor, etc.) and look at all details and relevant statistics for that selection. It could be interesting to make a timeline or a line chart and pinpoint major moments in theatrical history (technological advancements, significant show openings or closings, record-setting weeks, etc.) and look for reasons for them, as an educational piece for any other math-oriented theatre lovers.

On the other hand, this project could easily turn into a presentation in a more formal sense, with an intended audience of Broadway producers and investors to help them make wise decisions with their funds. It could be a PowerPoint with static charts and true deep dives into the data, to dig into KPIs and success measures that would indicate a strong ROI.

**Schedule (through 06/28/2022)**
1.	Get the Data (06/03/2022) *in progress, but behind schedule*
2.	Clean & Explore the Data (06/12/2022)
3.	Create Presentation of your Analysis (06/21/2022)
-	Should be a presentation, but could include a Jupyter Notebook or dashboard in Excel, Tableau, or PowerBI
4.	Internal demos (06/25/2022)
5.	Demo Day!! (06/28/2022)

Data Sources
1.	Web-scraped data from these websites, in order of preference: (none of these websites have APIs or native CSV-download options)
a.	https://www.ibdb.com/
i.	I have seen GitHub repositories of people who have successfully scraped IBDB (one in Ruby and one in Python), so I am optimistic.
b.	https://www.theatricalindex.com/
i.	This is a paid resource, and I’m not sure if I could pull off the scrape within the 7-day free trial.
c.	http://playbillpro.com/
i.	This is similarly a paid resource, but it has a 14-day free trial. However, I’m less familiar with this platform.
d.	https://www.playbill.com/grosses
i.	This seems very scrapable, BUT it doesn’t have all the data I’m hoping to use.
e.	https://www.broadwayleague.com/research/grosses-broadway-nyc/
i.	This one seems harder to scrape, considering the graph and season toggle are in an embedded dashboard and the URL doesn’t change as you click around.
2.	Stretch goal: If time permits, I would love to cross-reference my findings from theatrical statistics with the corresponding data for musical cast recordings, where applicable, either by streaming or sales. Potential sources for this:
a.	Spotify API
i.	Free and notoriously well-documented on how to use; I know several people have used the Spotify API with great success.
b.	Billboard chart data
i.	A paid resource, no free trial to my understanding.
Known Issues and Challenges
1.	Web scraping and API use are brand-new to me, and I am truthfully not feeling confident about it. Optimistic, for sure – but not confident quite yet.
2.	Sometimes, audiences just like what they like, and there might not be a good answer to my questions – it could all be a bit random, or too subjective to be quantified.
3.	I am sure cleaning scraped data will be a challenge. I am near certain that there will be some case-specific issues (ex, HAMILTON != Hamilton). I am particularly worried about having keys for table matching and joins – one data source may refer to the Imperial Theater, while another simply says the Imperial – so this will likely take some more manual work.
4.	I anticipate some data integrity issues and/or comparability issues, particularly around the COVID-19 closure and reopening. Some shows didn’t reopen at all, and those that did certainly didn’t all reopen simultaneously. There will likely be some data that is not comparable for a few months, so there may be some caveats to explore in this sense.

