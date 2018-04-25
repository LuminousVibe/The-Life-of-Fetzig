
title: Blog
menu-position: 10
---
<!--%
So this is my blog.  I've spent a lot of time thinking about starting one, wondering what I would share, and how I would go about saying it.  Mostly, though, this exists for my sanity, and anything I write will be for the purpose of preserving my sanity. 
from datetime import datetime
posts = [p for p in pages if "post" in p] # get all blog post pages
posts.sort(key=lambda p: p.get("date"), reverse=True) # sort post pages by date
for p in posts:
    date = datetime.strptime(p.date, "%Y-%m-%d").strftime("%B %d, %Y")
    print "  * **[%s](%s)** - %s" % (p.post, p.url, date) # markdown list item
%-->