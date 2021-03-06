# Twitter Mentions

This is a command line application which searches Twitter for the 5 most recent tweets that mention a given Twitter username.

There are two search methods in the application:

- `use_oauth`, the default method, uses the OAuth gem. It is faster but requires both a consumer key and an access token.
- `use_twitter` uses the Twitter gem. It is slower but requires only a consumer key.

## Usage

In order to use this application, two key-secret pairs are required, which can be generated at https://apps.twitter.com/.
They need to be saved into `access_token.txt` and `consumer_key.txt`, examples are included in this project.

To run the application, execute the following in a terminal:
```
$ ./search_tweets.rb <username> <method> 
```
Without arguments, the application will ask for a username and use the `use_oauth` method.

If a username is provided, `twitter` can be specified as a secondary argument to use the `use_twitter` method.
