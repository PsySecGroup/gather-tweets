# gather-tweets

Gathers all tweets and replies (but not retweets) a user had made and saves it to a CSV file.

Captures the last 3,200 tweets.  (We're working on expanding that)

# Install

We will automatically install [Twint](https://github.com/greyhao/twint.git) if you don't already have it.

If you already have a version of Twint, please uninstall it with the following command:

```bash
pip3 uninstall -y -r <(pip3 show --files twint | grep -oP '(?<=^Location: ).*')/requires.txt
```

Then, simply download the script with:

```bash
curl https://raw.githubusercontent.com/PsySecGroup/gather-tweets/gather-tweets
```

```bash
wget https://raw.githubusercontent.com/PsySecGroup/gather-tweets/gather-tweets
```

# Usage

To use `gather-tweets`, simply replace `elonmusk` with another Twitter account name and you'll see a CSV of the same name appear containing the last 3,200 tweets

```bash
./gather-tweets elonmusk
```