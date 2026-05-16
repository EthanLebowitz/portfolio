---
title: "The Birders Burden (Birding and its Many Dangers)"
description: "A visualization of the harms experienced by extreme birders."
date: 2026-05-12
tags: ["data visualization"]
draft: false
---

![Dot-plot of the harms incurred by birding](/images/birding-costs.png)

## Chart context

I recently stumbled across the documentary [LISTERS: A Glimpse Into Extreme Birdwatching](https://www.youtube.com/watch?v=zl-wAqplQAo), which I could not recommend enough. The documentary briefly references Jamal Hussein Essayli's 2013 master's thesis titled [the psychology of extreme birders: parallels to other extreme behaviors, anorexia nervosa, addiction, and autism spectrum disorder](https://scholarspace.manoa.hawaii.edu/server/api/core/bitstreams/235f6a40-7a9c-4bd0-9134-76fddd50df6b/content). Essayli sought to understand how extreme birding might relate to other extreme activities such as mountaineering, ultrarunning, and severe calorie restriction. The data in this study was gathered from ~400 participants enlisted from internet birding forums. The sample being taken from volunteers on birding forums probably skews the demographics, and is likely not a representative sample of all birders (participants in a forum tend to be more involved in the activity than average). In his sample, he observed that birding has features that are also found in these extreme activities. From the thesis:

>These features
include: euphoria, identification with the pursuit, pride, a sense of superiority, and
competitiveness related to the pursuit; a concern for the purity of the pursuit; and valuing
the pursuit in part because it facilitates predictable judgments, stability, simplicity, and
structure.

He also explored the possible relationship between extreme birding and addiction (both sometimes sharing "a pattern of escalation", an inability to fulfill expectations, and functional autonomy "which refers to the initial motives of a behavior becoming less important than the behavior itself"), as well as autism (both sharing "a tendency to systemize").

The data shown in the chart is from table 13 of the thesis, titled "Percentage of Birder Groups Endorsing the Costs of Birding". When I saw this table it was love at first sight. The birders were grouped into three categories: low-intensity, mid-range, and extreme. 
To determine the groupings, participants were given a questionnaire to determine how active and how experienced the birder was. Some examples of these features included:
 - Number of Birds on Life List
 - Number of Birds Identifiable by Sound
 - Number of Countries Visited for Birding
 - Days Involved in the Act of Birding
 - Days Thinking about Birding
 - Willing to Travel 5 Hours for Rare Bird
 - Percent Travel for Birding Purposes
 - Cost of Birding Equipment

These features were used to calculate a combined score. The category boundaries were then set 
at one standard deviation above the mean, and one standard deviation below the mean. In other words, a birder was considered "extreme" if their combined score was greater than one standard deviation above the mean of the combined scores of all study participants. 52 participants were classified as "extreme birders". They were 

>primarily male (79%), Caucasian (98%), involved in a romantic relationship (64%), born
in the United States (77%), have received a college degree or higher (71%), and currently
own $5,000 or more in birding-related equipment (71%). Although the Active score that
was utilized to identify extreme birders was not confounded by the number of years
birding, the final group of extreme birders still exhibited substantial birding experience:
extreme birders reported that, on average, they have been birding for 24 years, have 1,076
birds on their life lists, are able to identify 1,169 birds by sight and 495 birds by sound,
and have traveled to 9 different countries to bird. Within the past year, extreme birders
reported birding an average of 261 days and being somehow involved in the activity of
birding for 345 days. 64% of extreme birders reported that they would travel five hours
on short notice to see a rare bird, and 98% reported that they would travel one hour.

The plot was made with the matplotlib Python library, and checked for color blindness accessibility with daltonlens.

### Some of my favorite excerpts from the thesis

I found many of these quotes a delightful mix of hilarious, insightful, horrifying, and inspiring.

>“Birds are my salvation. I can look to them and I can fall back to
them. I care far more about birds than I do about people” (Lee Evans in Leveugle, 2010).

>Snetsinger, who began pursuing her record-breaking life list after being diagnosed with
cancer, also noted a connection between birding and her sense of identity: “Now, all I had
to do was recover from the surgery, and then I could start birding and living (had the two
become synonymous?) once more!” (Snetsinger, 2003, p. 86)

>Many extreme birders venture into unstable nations 
across the planet to list bird species, and some have lost their lives
in guerrilla zones (Connell, 2009). Snetsinger encountered various life-threatening
dangers before she died in a van accident while birding in Madagascar: she was chased
down by armed tribes in different countries, contracted malaria in Gabon, experienced a
shipwreck in Indonesia, and was assaulted and raped in Papua New Guinea (Snetsinger,
2003). Other notable birders have also died as a result of this extreme pursuit: Ted Parker
was killed in a plane crash in Ecuador, Alan Adams disappeared in the Himalayas, David
Hunt was mauled by a tiger in India, Tim Andrews died at the hands of guerrillas in Peru,
and Joe Wood disappeared while birding on Mount Rainier.

>“The most problematic relationship for a twitcher is usually your
spouse, if you have one at all” (Cocker, 2001, p. 125).

>Top birder Richard Koeppel estimated that he had spent more
than $300,000 to accumulate a list of 6,500 bird species (Koeppel, 2005, p. 176).

>Additionally, Scott Weidensaul connected the extreme and
costly components of birding to the pursuit of mountaineering:
How normal is it to abandon your career and family for a year,
ricocheting from one end of the continent to the other as you try to rack up
a record-breaking list of birds? But then, how normal is it to pay $60,000
to $70,000 to risk death climbing Mount Everest? Every pastime, pushed
to its logical bounds, becomes peculiar; push it well beyond those limits,
and it becomes bizarre (Weidensaul 2007, pp. 277-278).

>Extreme birders frequently report an appreciation for the pursuit’s ability to
facilitate simplicity, predictability, stability, and structure. Sean Dooley explained:
“When you identify and list things, [you can] impose order on an otherwise baffling
universe. Birding gives people who don’t have much control in other aspects of their
lives at least some illusion of control” (Dooley, 2005, p. 38).

>Dan Koeppel, the son of extreme birder Richard Koeppel, characterized his father as “a
brilliant man whose life didn’t turn out the way he wanted [and who] buried the sadness
by watching birds [and] tending his log-books and checklists” (Koeppel, 2005, p. xv)

>anecdotal accounts suggest that extreme birding may prove unsuccessful
at satisfying the lofty expectations of meaning and fulfillment that birders hope to
achieve from the pursuit. In reference to his father’s extreme birding, Dan Koeppel
concluded that extreme birding and obsessive behaviors fail to “fill our empty spaces . . .
Not for Dad, not for me, and probably not for any of the Big Listers” (Koeppel, 2005, p. 270)
