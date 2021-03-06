![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Lab | My first queries

Please, import the .csv database called *AppleStore.csv*. Use the *data* table to query the data about Apple Store Apps and answer the following questions: 

**1. Which are the different genres?**
Games
Productivity
Weather
Shopping
Reference
Finance
Music
Utilities
Travel
Social Networking
Sports
Business
Health & Fitness
Entertainment
Photo & Video
Navigation
Education
Lifestyle
Food & Drink
News
Book
Medical
Catalogs

**2. Which is the genre with more apps rated?**
— Games	3346

**3. Which is the genre with more apps?**
— Games	3797

**4. Which is the one with less?**
— Catalogs	10

**5. Take the 10 apps most rated.**
— Facebook	2974676
— Instagram	2161558
— Clash of Clans	2130805
— Temple Run	1724546
— Pandora - Music & Radio	1126879
— Pinterest	1061624
— Bible	985920
— Candy Crush Saga	961794
— Spotify Music	878563
— Angry Birds	824451

**6. Take the 10 apps best rated by users.**
— TurboScan™ Pro - document & receipt scanner: scan multiple pages and photos to PDF	5
— Flashlight Ⓞ	5
— Learn to Speak Spanish Fast With MosaLingua	5
— :) Sudoku +	5
— The Photographer's Ephemeris	5
— King of Dragon Pass	5
— Escape the Sweet Shop Series	5
— Infinity Blade	5
— Plants vs. Zombies HD	5
— Plants vs. Zombies	5


**7. Take a look on the data you retrieved in the question 5. Give some insights.**
— The apps that have recieved more reviews in the app store are Social Networks (Facebook and Instagram). I suspect they'll be the most common apps found on iPhone users.

— There are 4 Games (Clash of Clans, Temple Run, Candy Crush and Angry Birds), in the top 10, reflecting the preponderance of games as an important universal experience (at least for the iPhone users).

- The same can be said about the presence of 2 music streaming platforms in the top 10.

- Pintrest and the Bible close this top10. It's interesting to find the most published book (The Bible) to creep into a similar popularity among iPhone users, and what's essentially a "read latter"/"consult latter" service (which may reflect a prevelance of "FOMO" in today's culture among iPhone users).

- All in all, I'd conclude that the most common uses for the iPhone (judging by this metric) will be to sociallize and leisure, due to the prevelance of social networks, music streaming apps and games among the top10 of the most rated apps.


**8. Take a look on the data you retrieved in the question 6. Give some insights.**
I changed the Query slightly for this question, since, I believe, it would give more relevant information (as it is not the same to compare apps that have something like 10 Ratings, 1K Ratings and 100K Ratings. The new list (for apps with 100K Ratings or more) is:

Plants vs. Zombies HD	163598	5
Zappos: shop shoes & clothes, fast free shipping	103655	5
Credit Karma: Free Credit Scores, Reports & Alerts	101679	5
Infinity Blade	326482	5
Head Soccer	481564	5
Plants vs. Zombies	426463	5
Flashlight Ⓞ	130450	5
The Room	143908	5
Domino's Pizza USA	258624	5
Pic Collage - Picture Editor & Photo Collage Maker	123433	5

— They all still have 5 stars (which is pretty impressive). 
— There are 5 games: Plants vs. Zombies HD, Plants vs. Zombies, Infinity Blade, Head Soccer and The Room (4 if you consider that Plants vs. Zombies has 2 entries), reflecting both the popularity and satisfaction of the iPhone users with these games.
— A couple of utilities (flashlight and Pic Collage); Flaslight is surprising, since iPhone has a flashlight by default.
— Then there is a clothing shop (Zappos), a credit score app (Credit Karma) and Domino's Pizza, which probably reflect habits of American users.

**9. Now compare the data from questions 5 and 6. What do you see?**
Games seem to dominate these rankings.

**10. How could you take the top 3 regarding the user ratings but also the number of votes?**

**11. Does people care about the price?** Do some queries, comment why are you doing them and the results you retrieve. What is your conclusion?

— 1st, and since there seems to be no total downloads, I used the average rating_count_tot to infer if price had an impact on the amount of downloads. 'though inconclusive (naturally), since the top 11 in this category are all free (not considering the possibility of being freemium), and the top 20 only have 3 payed entries (1,99 | 0,99 and 6,99), I'd say that probably does skew whether a user will download an app or not. With a little more certainty I can say that it influences the amount of people that rate an app, probably because more people download it (but can't be too confident about that with the current data).

— 2nd the list of the average price for the rating is interesting; The least well rated are also the cheapest (0 starts at aprox. 0,99), which would either indicate a low quality of the app or that users become no less demanding of its quality regardless of what they pay for it. Also, there seems to be little variance among price and user rating; with 5 stars the average price is (aprox.) 1,64, while with 1 star it's at (aprox.) 1,93, with the higest average price (aprox 2,16) in the 4 stars and lowest average price (not counting 0 stars) at 2.5 (with, aprox., 1,10).

- 3rd Many free apps (unkown if they're freemium), with more than 100K ratings, are still able to reach 5 and 4.5 stars, while, strangely, none appears to be below 2 stars, which begs the question: does "free" bring with it some tolerance? 


## Deliverables 
You need to submit a `.sql` file that includes the queries used to answer the questions above, as well as an `.md` file including your answers. 
