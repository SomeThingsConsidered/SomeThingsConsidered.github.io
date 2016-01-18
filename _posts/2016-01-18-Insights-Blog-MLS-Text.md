---
layout: post
title: "Insights Blog: Realtor Comments and Hedonic Regression"
date: 2016-01-18
---
I recently added an entry to CoreLogic's Insights blog which examined <a href="http://www.corelogic.com/blog/authors/matt-cannon/2016/01/turning-words-into-data.aspx#.Vp1glXhcKeA" a> realtor comments and property listings. </a>  The analysis was fairly high level, but provided an introduction regarding how information contained in listing agent comments could improve house price estimation via <a href="https://en.wikipedia.org/wiki/Hedonic_regression" a> hedonic regression</a>.  Specifically, I regressed the log of house price against the number of bedrooms, bathrooms, living space, and a bag of words based on the realtor comments. More information can be found on CoreLogic's Insights blog page.

The R code estimating the regression, using glmnet, can be found <a href="https://github.com/SomeThingsConsidered/MLS_text_analysis/blob/master/hedonic_regression_1.R" a> here. </a>

I also created code to identify listings containing a specific word, and then printed the entire realtor comment containing the word.  This was useful in examining the context in which a word was used (i.e. "swamp" was used describe a cooling method-- swamp coolers).  Code <a href = "https://github.com/SomeThingsConsidered/MLS_text_analysis/blob/master/check_corpus_entries.R" a> can be found here. </a> 
