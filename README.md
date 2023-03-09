# Formula 1 News Mobile Application 
## README

## Introduction
#####  What the app does:
This mobile app is designed to keep F1 fans up to date with the latest news and articles from various sources. The app 
collects articles using the News API and displays them in a user-friendly interface allowing the users to quickly access information with an intuitive and clean interface.

#### Features:
- Displays articles from the internet about F1
- Allows the user the sort articles about their favourite team first
- Simple interface
- Webview displays the articles in app
- The user can choose a dark or light theme that saves when the user exits the app
- Lightweight design

#### Design Rationale:
##### For my data storage I chose shared preferences:
1. Simple - shared preferences(SP) is a very uncomplicated way to store small amounts of data
2. Efficient use of the available resources. SP uses minimal resources and does not impact the performance of the application
which was important to me as I wanted my app to be responsive and quick.
3. Implementation - Implementing SP is very easy and straightforward.
4. Data size - All I needed to store in memory was boolean values a database or file system  would be too large for this usecase

##### I decided not to use fragments because:
1. It would have added unnecessary complexity to the app
2. I did not want the app to be bloated and have performance issues
3. Older devices may not support fragments limiting the user base

##### I used News API:
1. I chose to use the News API because I have previous experience with it
2. Using an API to collect and deliver data saved on development time
3. My users are provided with a large range of news data that I could not have provided by myself

#### Future implementations:
- Ability to save favourite articles
- Option to share articles
- Display thumbnails and description
- Push notification
- User profiles

#### Challenges Faced:
- Initially I intended to display a thumbnail for each article however I could not get that feature to work, so I had to abandon it.
- I could not change the colour of the cards in the recycler view
- I had some design challenges trying to fit the save button and the switch into the main activity view without blocking the articles are being in the way. 


