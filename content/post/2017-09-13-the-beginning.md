---
title: The Beginning
author: Alex Norman
date: '2017-09-13'
draft: false
slug: the-beginning
categories: []
tags: []
header:
  caption: ''
  image: ''
---

Now we can type some words that will be about a topc. It will be interesting, ccertainly, and readers will want to continue reading. But now a quote.

>We live in a society exquisitely dependent on science and technology, in which hardly anyone knows anything about science and technology. 
>
>**Carl Sagan**

And what do we think of that?

What we can do now, however, is quote some code to show how cool we are. It's a good way of performing one's identity as a serious programmer.

```r
  # Gather data for dataframe with one row for each unique code application
  for(i in 1:ncol(selected_data_TF)){
    obj <- as.logical(selected_data_TF[, i])  # get TRUE/FALSE for each column
    res <- sum(obj)                  # how many TRUE?
    # if some are TRUE, determine which ones are T and pull those out of 'mop' 
    # which has the start and end time of each code application.
    if(res>=1){                     
          tag <- mop[which(obj==TRUE), ]   
          tag$code <- colnames(selected_data_TF[i]) # get applied code name 
          code_events <- rbind(code_events, tag) # row-bind code_events and tags
    } 
  }
```
How does that look?

Interestingly, there are all sorts of hidden gems.

A Twitter script:
{{< tweet 907269861574930432 >}}

Wow!

And YouTube videos, as well!
{{< youtube _GkBzDQfoHg >}}

And Instagram!
{{<instagram BZBCJ2hFwuq>}}

OMG!! Gists! (which I found [here](https://jabranham.com/blog/2016/12/analyzing-a-bib-file/))

{{< gist jabranham 887495eaf029680316fecb374f0723e0 >}}