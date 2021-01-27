# cf-wrangle
Jan 27 Challenge
## Assigned Play
Macbeth
## Speaker 1
- MALCOLM
## Speaker 2
- MACDUFF
## Question I was asked
How many times did those two speakers, speak? What's the combonation, what's the sum?

## Commands I used to answer the Question
```bash 
$ grep -wc "<b>MALCOLM</b>" macbeth.txt -c > malcolmcount.txt
```

```bash
$ grep -wc "<b>MACDUFF</b>" macbeth.txt -c > macduffcount.txt
```

```bash
$ grep -wc "<b>MACDUFF</b>\|<b>MALCOLM</b>" macbeth.txt -c > totalcount.txt
```

## The ANSWER
The two players spoke a total of 99 times. I used the fact that all the times when a player spoke, their name was surrounded in bold tags to only grab the count of their speaking cues.