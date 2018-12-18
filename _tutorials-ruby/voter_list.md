---
title:  Voter List
position: 6
exclude: true
layout: full-row
description: Shows active vote totals
---

This example will output the active vote totals for the post/comment passed as an argument to the script.

### Script

First, we ask the blockchain for the active votes on a post or comment.  Then, we count the `upvotes`, `downvotes`, and `unvotes` (which are votes that have been removed after being cast in a previous transaction).

Then, we sort the votes by `rshares` to find the top voter.

### To Run

First, set up your workstation using the steps provided in [Getting Started](https://developers.steem.io/tutorials-ruby/getting_started).  Then you can create and execute the script (or clone from this repository):

```bash
git clone git@github.com:steemit/devportal-tutorials-rb.git
cd devportal-tutorials-rb/tutorials/06_get_voters_list_on_post
bundle install
ruby voter_list.rb https://steemit.com/steemdev/@steemitdev/announcing-the-steem-developer-portal
```

### Example Output

```
Upvotes: 231
Downvotes: 1
Unvotes: 0
Total: 232
Top Voter: thejohalfiles
```
