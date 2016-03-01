# soccer-tweet-data
Twitter Data Collected related to European Soccer Games ( English Premier League, Spanish League, International friendlies).

# Data Format

* Most of the csv files are in tabular format with columns: 
* text - Tweet Text
* user - User who tweeted the tweet
* created_at - The time at which tweet was tweeted
* timestamp - Unix timestamp of the tweet
* geo - Location Co-ordinate of the tweet from where it was created. None if there is no location information.
* lang - This column is not present in all files, This is for the possible language of the tweet as given by Twitter.

# Config File format

Only few config files have detailed information about the game to which the data belongs to. Each of the data file 
has corresponding configuration inside config/config-[datafilename].txt. 

* game: Name and League of the game
* starttime=Not Applicable
* endtime=Not Applicable
* keywords= The keywords that are used for filtering tweets from twitter stream.
* db=Data file name
* kotime=Kick of Time in GMT
* fh_added_time= First Half Added time in minutes
* sh_added_time=Second Half Added time in minutes
* home-team=Home team name and the comma separated players given name seperated by colon
* away-team=Away team name and the comma separated players given name seperated by colon
* tpm=Tweets per minute for that Game, Calculated using collected tweets over 90 minute game
* n_tweets=Number of tweets collected for this game
