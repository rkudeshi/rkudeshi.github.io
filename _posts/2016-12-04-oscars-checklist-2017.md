---
title: "Oscars checklist: Figuring out which movies are most likely to be nominated for awards so I can watch them while they're still in theaters"
---

Last year, I tried to [watch every movie nominated for an Oscar](http://raviudeshi.com/16/02/top-movies-2015). But I missed a couple because by the time nominations were announced, those movies were out of theaters but not yet out on DVD/Blu-Ray/iTunes.

This year, I decided to try to figure out the Oscar-nominated movies ahead of time. I used data from [GoldDerby.com](http://goldderby.com), a Hollywood awards-prediction site. They have ongoing odds calculations for 18 major categories, which I used to allocate points to each movie.

(Yes, this is all pretty stupid, since the biggest awards contenders are already pretty well-known. But I was curious about the movies that might have flown more under-the-radar, and anyways, it was a fun exercise for me in using Markdown tables!)

---

**Shortcuts**

* [Sort by category](#sort-by-category)
    * <small>*[Best Picture](#best-picture) / [Best Director](#best-director) / [Best Actor](#best-actor) / [Best Actress](#best-actress) / [Best Supporting Actor](#best-supporting-actor) / [Best Supporting Actress](#best-supporting-actress) / [Best Original Screenplay](#best-original-screenplay) / [Best Adapted Screenplay](#best-adapted-screenplay) / [Best Animated Feature](#best-animated-feature) / [Best Visual Effects](#best-visual-effects) / [Best Cinematography](#best-cinematography) / [Best Film Editing](#best-film-editing) / [Best Score](#best-score) / [Best Sound Editing](#best-sound-editing) / [Best Sound Mixing](#best-sound-mixing) / [Best Production Design](#best-production-design) / [Best Costume Design](#best-costume-design) / [Best Makeup and Hairstyling](#best-makeup-and-hairstyling)*</small>
* [Sort by movie](#sort-by-movie)
* [Sort by score](#sort-by-score)
* [Final list](#final-list)

---

### Sort by category

Here's the original set of data, sorted by Oscar category. It is all sourced from [Gold Derby's experts predictions](http://www.goldderby.com/odds/expert-odds/oscars-nominations-2017/) for the 2017 Oscars ceremony. I downloaded the data sometime in the last week of November, so my numbers may be a little different than the latest odds. The only thing I've added is the points column, which I explain below.

An explanation of the columns:

* **NOM** = The number of experts who believe a film will be *nominated* for that award.
* **WIN** = The number of experts who believe a film will *win* for that award.
* **ODDS** = GoldDerby's odds of a movie winning that award.
* **PTS** = My very simple formula for allocating points. It's just 100 divided by the odds. For example, a title with 20/1 odds is calculated as `100/ODDS` = `100/(20/1)` = `100/20` = `5` points. You can think of it as roughly the percentage chance of the movie winning that award.[^implied-probability]

One other thing of note: if you look at the original charts on Gold Derby, every category has numerous movies with 100/1 odds and zero experts predicting a nomination or win. I think Gold Derby keeps them around because they were thought at one time to be contenders, but they serve no real purpose for my needs, so I have omitted them from my charts below. Also, I don't understand how Gold Derby sorts movies with the same odds ranking because there were a few categories with a movie with 100/1 odds and 1 nomination prediction ranked well below a bunch of movies with 100/1 odds and 0 nomination predictions. This is why the last entry in some of the charts has a very different NUM rank than the preceding entry.

[^implied-probability]: It was only after I ran all the numbers that I discovered [implied probability](https://www.sbo.net/strategy/implied-probability/). Unfortunately, I used Markdown tables to organize this data and it's devilishly difficult to re-calculate numbers in that format. And the implied probability calculations would've only slighted changed the numbers and almost never the order of rankings. If I was doing this all over again, I would've kept all the data in an Excel spreadsheet and only converted it to Markdown tables when I was ready to publish this post, but c'est la vie!

#### Best Picture

|-----|---------------------------------|-----|-----|-------|-------|
| NUM |               NAME              | NOM | WIN |  ODDS |  PTS  |
|-----|---------------------------------|-----|-----|-------|-------|
|   1 | La La Land                      |  26 |  22 | 9/2   | 22.22 |
|   2 | Manchester by the Sea           |  26 |   4 | 13/2  | 15.38 |
|   3 | Moonlight                       |  26 |   0 | 9/1   | 11.11 |
|   4 | Fences                          |  25 |   0 | 9/1   | 11.11 |
|   5 | Loving                          |  22 |   1 | 12/1  |  8.33 |
|   6 | Silence                         |  21 |   0 | 14/1  |  7.14 |
|   7 | Lion                            |  20 |   0 | 14/1  |  7.14 |
|   8 | Jackie                          |  18 |   0 | 16/1  |  6.25 |
|   9 | Arrival                         |  15 |   0 | 20/1  |  5.00 |
|  10 | Sully                           |  14 |   0 | 28/1  |  3.57 |
|  11 | Hidden Figures                  |  10 |   0 | 33/1  |  3.03 |
|  12 | Hell or High Water              |   6 |   0 | 50/1  |  2.00 |
|  13 | Hacksaw Ridge                   |   7 |   0 | 66/1  |  1.52 |
|  14 | A Monster Calls                 |   2 |   0 | 100/1 |  1.00 |
|  15 | Nocturnal Animals               |   4 |   0 | 100/1 |  1.00 |
|  16 | Patriot's Day                   |   1 |   0 | 100/1 |  1.00 |
|  17 | The Birth of a Nation           |   4 |   0 | 100/1 |  1.00 |
|  18 | 20th Century Women              |   1 |   0 | 100/1 |  1.00 |
|  19 | Billy Lynn's Long Halftime Walk |   2 |   0 | 100/1 |  1.00 |
|  20 | Passengers                      |   1 |   0 | 100/1 |  1.00 |
|  21 | Live By Night                   |   1 |   0 | 100/1 |  1.00 |
|-----|---------------------------------|-----|-----|-------|-------|


#### Best Director

|-----|-------------------------------------------|-----|-----|-------|-------|
| NUM |                    NAME                   | NOM | WIN |  ODDS |  PTS  |
|-----|-------------------------------------------|-----|-----|-------|-------|
|   1 | La La Land (Damien Chazelle)              |  26 |  22 | 17/10 | 58.82 |
|   2 | Manchester by the Sea (Kenneth Lonergan)  |  26 |   4 | 4/1   | 25.00 |
|   3 | Moonlight (Barry Jenkins)                 |  23 |   0 | 6/1   | 16.67 |
|   4 | Silence (Martin Scorsese)                 |  14 |   0 | 12/1  |  8.33 |
|   5 | Fences (Denzel Washington)                |  14 |   1 | 12/1  |  8.33 |
|   6 | Jackie (Pablo Larrain)                    |   7 |   0 | 33/1  |  3.03 |
|   7 | Loving (Jeff Nichols)                     |   5 |   0 | 40/1  |  2.50 |
|   8 | Arrival (Denis Villeneuve)                |   4 |   0 | 66/1  |  1.52 |
|   9 | Billy Lynn's Long Halftime Walk (Ang Lee) |   2 |   0 | 80/1  |  1.25 |
|  10 | Lion (Garth Davis)                        |   2 |   0 | 80/1  |  1.25 |
|  11 | Hidden Figures (Theodore Melfi)           |   1 |   0 | 100/1 |  1.00 |
|  12 | Passengers (Morten Tyldum)                |   1 |   0 | 100/1 |  1.00 |
|  13 | Sully (Clint Eastwood)                    |   1 |   0 | 100/1 |  1.00 |
|  14 | Hacksaw Ridge (Mel Gibson)                |   1 |   0 | 100/1 |  1.00 |
|  36 | Nocturnal Animals (Tom Ford)              |   1 |   0 | 100/1 |  1.00 |
|-----|-------------------------------------------|-----|-----|-------|-------|


#### Best Actor

|-----|---------------------------------------|-----|-----|-------|-------|
| NUM |                  NAME                 | NOM | WIN |  ODDS |  PTS  |
|-----|---------------------------------------|-----|-----|-------|-------|
|   1 | Manchester by the Sea (Casey Affleck) |  26 |  17 | 2/1   | 50.00 |
|   2 | Fences (Denzel Washington)            |  24 |  10 | 14/5  | 35.71 |
|   3 | La La Land (Ryan Gosling)             |  22 |   0 | 13/2  | 15.38 |
|   4 | Loving (Joel Edgerton)                |  17 |   0 | 9/1   | 11.11 |
|   5 | Sully (Tom Hanks)                     |  14 |   0 | 14/1  |  7.14 |
|   6 | Captain Fantastic (Viggo Mortensen)   |   5 |   0 | 40/1  |  2.50 |
|   7 | Hacksaw Ridge (Andrew Garfield)       |   6 |   0 | 40/1  |  2.50 |
|   8 | The Founder (Michael Keaton)          |   3 |   0 | 66/1  |  1.52 |
|   9 | Silence (Andrew Garfield)             |   3 |   0 | 80/1  |  1.25 |
|  10 | Rules Don't Apply (Warren Beatty)     |   2 |   0 | 100/1 |  1.00 |
|  11 | Nocturnal Animals (Jake Gyllenhaal)   |   2 |   0 | 100/1 |  1.00 |
|  12 | The Birth of a Nation (Nate Parker)   |   2 |   0 | 100/1 |  1.00 |
|  13 | Gold (Matthew McConaughey)            |   1 |   0 | 100/1 |  1.00 |
|-----|---------------------------------------|-----|-----|-------|-------|


#### Best Actress

|-----|----------------------------------------|-----|-----|-------|-------|
| NUM |                  NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|----------------------------------------|-----|-----|-------|-------|
|   1 | La La Land (Emma Stone)                |  26 |  17 | 21/10 | 47.62 |
|   2 | Jackie (Natalie Portman)               |  25 |   6 | 7/2   | 28.57 |
|   3 | Loving (Ruth Negga)                    |  23 |   2 | 6/1   | 16.67 |
|   4 | 20th Century Women (Annette Bening)    |  20 |   1 | 7/1   | 14.29 |
|   5 | Arrival (Amy Adams)                    |  15 |   0 | 14/1  |  7.14 |
|   6 | Hidden Figures (Taraji P. Henson)      |   4 |   1 | 25/1  |  4.00 |
|   7 | Miss Sloane (Jessica Chastain)         |   5 |   0 | 40/1  |  2.50 |
|   8 | Florence Foster Jenkins (Meryl Streep) |   4 |   0 | 50/1  |  2.00 |
|   9 | Elle (Isabelle Huppert)                |   4 |   0 | 66/1  |  1.52 |
|  10 | Fences (Viola Davis)                   |   1 |   0 | 100/1 |  1.00 |
|  11 | Passengers (Jennifer Lawrence)         |   1 |   0 | 100/1 |  1.00 |
|  12 | Nocturnal Animals (Amy Adams)          |   1 |   0 | 100/1 |  1.00 |
|-----|----------------------------------------|-----|-----|-------|-------|


#### Best Supporting Actor

|-----|------------------------------------------------|-----|-----|-------|-------|
| NUM |                      NAME                      | NOM | WIN |  ODDS |  PTS  |
|-----|------------------------------------------------|-----|-----|-------|-------|
|   1 | Moonlight (Mahershala Ali)                     |  24 |  13 | 12/5  | 41.67 |
|   2 | Manchester by the Sea (Lucas Hedges)           |  22 |   4 | 9/2   | 22.22 |
|   3 | Hell or High Water (Jeff Bridges)              |  18 |   2 | 13/2  | 15.38 |
|   4 | Lion (Dev Patel)                               |  14 |   3 | 9/1   | 11.11 |
|   5 | Nocturnal Animals (Michael Shannon)            |  14 |   3 | 9/1   | 11.11 |
|   6 | Silence (Liam Neeson)                          |  10 |   2 | 12/1  |  8.33 |
|   7 | Fences (Stephen Henderson)                     |   5 |   0 | 50/1  |  2.00 |
|   8 | Florence Foster Jenkins (Hugh Grant)           |   6 |   0 | 50/1  |  2.00 |
|   9 | Fences (Jovan Adepo)                           |   4 |   0 | 50/1  |  2.00 |
|  10 | Denial (Timothy Spall)                         |   2 |   0 | 66/1  |  1.52 |
|  11 | Bleed for This (Aaron Eckhart)                 |   2 |   0 | 100/1 |  1.00 |
|  12 | Billy Lynn's Long Halftime Walk (Steve Martin) |   1 |   0 | 100/1 |  1.00 |
|  13 | Hell or High Water (Ben Foster)                |   1 |   0 | 100/1 |  1.00 |
|  14 | Hidden Figures (Kevin Costner)                 |   1 |   0 | 100/1 |  1.00 |
|  15 | Manchester by the Sea (Kyle Chandler)          |   1 |   0 | 100/1 |  1.00 |
|  25 | Fences (Mykelti Williamson)                    |   1 |   0 | 100/1 |  1.00 |
|-----|------------------------------------------------|-----|-----|-------|-------|


#### Best Supporting Actress

|-----|---------------------------------------------------|-----|-----|-------|-------|
| NUM |                        NAME                       | NOM | WIN |  ODDS |  PTS  |
|-----|---------------------------------------------------|-----|-----|-------|-------|
|   1 | Fences (Viola Davis)                              |  25 |  19 | 2/1   | 50.00 |
|   2 | Manchester by the Sea (Michelle Williams)         |  23 |   8 | 10/3  | 30.00 |
|   3 | Moonlight (Naomie Harris)                         |  24 |   0 | 5/1   | 20.00 |
|   4 | Lion (Nicole Kidman)                              |  20 |   0 | 9/1   | 11.11 |
|   5 | 20th Century Women (Greta Gerwig)                 |  10 |   0 | 20/1  |  5.00 |
|   6 | Hidden Figures (Janelle Monae)                    |   8 |   0 | 22/1  |  4.55 |
|   7 | A Monster Calls (Felicity Jones)                  |   7 |   0 | 33/1  |  3.03 |
|   8 | The Hollars (Margo Martindale)                    |   2 |   0 | 100/1 |  1.00 |
|   9 | The Birth of a Nation (Aja Naomi King)            |   3 |   0 | 100/1 |  1.00 |
|  10 | 20th Century Women (Elle Fanning)                 |   1 |   0 | 100/1 |  1.00 |
|  11 | Queen of Katwe (Lupita Nyong'o)                   |   1 |   0 | 100/1 |  1.00 |
|  12 | Billy Lynn's Long Halftime Walk (Kristen Stewart) |   1 |   0 | 100/1 |  1.00 |
|  13 | The Founder (Laura Dern)                          |   1 |   0 | 100/1 |  1.00 |
|  14 | Nocturnal Animals (Amy Adams)                     |   1 |   0 | 100/1 |  1.00 |
|  23 | Hidden Figures (Octavia Spencer)                  |   1 |   0 | 100/1 |  1.00 |
|-----|---------------------------------------------------|-----|-----|-------|-------|


#### Best Original Screenplay

|-----|-----------------------|-----|-----|-------|-------|
| NUM |          NAME         | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------|-----|-----|-------|-------|
|   1 | Manchester by the Sea |  24 |  18 | 2/1   | 50.00 |
|   2 | Moonlight             |  23 |   5 | 7/2   | 28.57 |
|   3 | La La Land            |  23 |   2 | 9/2   | 22.22 |
|   4 | Loving                |  13 |   1 | 11/1  |  9.09 |
|   5 | Jackie                |  15 |   0 | 12/1  |  8.33 |
|   6 | Hell or High Water    |   8 |   0 | 20/1  |  5.00 |
|   7 | 20th Century Women    |  10 |   0 | 20/1  |  5.00 |
|   8 | Captain Fantastic     |   2 |   0 | 100/1 |  1.00 |
|   9 | Zootopia              |   1 |   0 | 100/1 |  1.00 |
|  22 | The Lobster           |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------|-----|-----|-------|-------|


#### Best Adapted Screenplay

|-----|---------------------|-----|-----|-------|-------|
| NUM |         NAME        | NOM | WIN |  ODDS |  PTS  |
|-----|---------------------|-----|-----|-------|-------|
|   1 | Fences              |  21 |  19 | 19/10 | 52.63 |
|   2 | Arrival             |  21 |   2 | 5/1   | 20.00 |
|   3 | Silence             |  20 |   2 | 11/2  | 18.18 |
|   4 | Lion                |  17 |   1 | 15/2  | 13.33 |
|   5 | Nocturnal Animals   |  12 |   1 | 12/1  |  8.33 |
|   6 | Hidden Figures      |  11 |   0 | 16/1  |  6.25 |
|   7 | A Monster Calls     |   6 |   1 | 25/1  |  4.00 |
|   8 | Hacksaw Ridge       |   2 |   0 | 66/1  |  1.52 |
|   9 | Love and Friendship |   2 |   0 | 80/1  |  1.25 |
|  10 | Elle                |   1 |   0 | 100/1 |  1.00 |
|  11 | Sully               |   1 |   0 | 100/1 |  1.00 |
|  12 | Finding Dory        |   1 |   0 | 100/1 |  1.00 |
|  21 | Snowden             |   1 |   0 | 100/1 |  1.00 |
|-----|---------------------|-----|-----|-------|-------|


#### Best Animated Feature

|-----|--------------------------|-----|-----|-------|-------|
| NUM |           NAME           | NOM | WIN |  ODDS |  PTS  |
|-----|--------------------------|-----|-----|-------|-------|
|   1 | Zootopia                 |  21 |  16 | 15/8  | 53.33 |
|   2 | Kubo and the Two Strings |  18 |   2 | 5/1   | 20.00 |
|   3 | Moana                    |  15 |   2 | 13/2  | 15.38 |
|   4 | Finding Dory             |  14 |   0 | 8/1   | 12.50 |
|   5 | The Red Turtle           |  13 |   0 | 11/1  |  9.09 |
|   6 | Sing                     |   9 |   1 | 14/1  |  7.14 |
|   7 | Sausage Party            |   6 |   0 | 28/1  |  3.57 |
|   8 | The Little Prince        |   4 |   0 | 40/1  |  2.50 |
|   9 | Trolls                   |   2 |   0 | 80/1  |  1.25 |
|  10 | My Life as a Zucchini    |   1 |   0 | 100/1 |  1.00 |
|  11 | Miss Hokusai             |   1 |   0 | 100/1 |  1.00 |
|-----|--------------------------|-----|-----|-------|-------|


#### Best Visual Effects

|-----|---------------------------------------------|-----|-----|-------|-------|
| NUM |                     NAME                    | NOM | WIN |  ODDS |  PTS  |
|-----|---------------------------------------------|-----|-----|-------|-------|
|   1 | Doctor Strange                              |   8 |   4 | 3/1   | 33.33 |
|   2 | The Jungle Book                             |   6 |   5 | 10/3  | 30.00 |
|   3 | Rogue One: A Star Wars Story                |   7 |   1 | 11/2  | 18.18 |
|   4 | Fantastic Beasts and Where to Find Them     |   6 |   0 | 9/1   | 11.11 |
|   5 | Arrival                                     |   4 |   1 | 10/1  | 10.00 |
|   6 | Miss Peregrine's Home for Peculiar Children |   5 |   0 | 20/1  |  5.00 |
|   7 | Captain America: Civil War                  |   3 |   0 | 25/1  |  4.00 |
|   8 | Sully                                       |   1 |   0 | 50/1  |  2.00 |
|   9 | Star Trek Beyond                            |   1 |   0 | 66/1  |  1.52 |
|  10 | The BFG                                     |   1 |   0 | 100/1 |  1.00 |
|  11 | A Monster Calls                             |   1 |   0 | 100/1 |  1.00 |
|  12 | Warcraft                                    |   1 |   0 | 100/1 |  1.00 |
|  13 | Deadpool                                    |   1 |   0 | 100/1 |  1.00 |
|-----|---------------------------------------------|-----|-----|-------|-------|


#### Best Cinematography

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | La La Land                              |  18 |  14 | 19/10 | 52.63 |
|   2 | Silence                                 |  15 |   2 | 6/1   | 16.67 |
|   3 | Arrival                                 |  13 |   2 | 6/1   | 16.67 |
|   4 | Jackie                                  |  13 |   0 | 9/1   | 11.11 |
|   5 | Moonlight                               |  12 |   0 | 9/1   | 11.11 |
|   6 | Live By Night                           |   4 |   0 | 28/1  |  3.57 |
|   7 | Nocturnal Animals                       |   2 |   1 | 33/1  |  3.03 |
|   8 | Lion                                    |   3 |   0 | 50/1  |  2.00 |
|   9 | The Jungle Book                         |   3 |   0 | 50/1  |  2.00 |
|  10 | Hail, Caesar!                           |   2 |   0 | 66/1  |  1.52 |
|  11 | A Monster Calls                         |   2 |   0 | 80/1  |  1.25 |
|  12 | Fantastic Beasts and Where to Find Them |   1 |   0 | 100/1 |  1.00 |
|  13 | Cafe Society                            |   1 |   0 | 100/1 |  1.00 |
|  14 | Doctor Strange                          |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Film Editing

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | La La Land                              |  12 |  10 | 2/1   | 50.00 |
|   2 | Silence                                 |   9 |   1 | 11/2  | 18.18 |
|   3 | Jackie                                  |   9 |   1 | 13/2  | 15.38 |
|   4 | Hacksaw Ridge                           |   8 |   0 | 10/1  | 10.00 |
|   5 | Moonlight                               |   6 |   0 | 11/1  |  9.09 |
|   6 | Sully                                   |   1 |   1 | 25/1  |  4.00 |
|   7 | The Jungle Book                         |   2 |   1 | 28/1  |  3.57 |
|   8 | Hidden Figures                          |   2 |   0 | 28/1  |  3.57 |
|   9 | Nocturnal Animals                       |   3 |   0 | 28/1  |  3.57 |
|  10 | Arrival                                 |   3 |   0 | 33/1  |  3.03 |
|  11 | Deepwater Horizon                       |   2 |   0 | 66/1  |  1.52 |
|  12 | Lion                                    |   1 |   0 | 100/1 |  1.00 |
|  13 | Manchester by the Sea                   |   1 |   0 | 100/1 |  1.00 |
|  14 | Fantastic Beasts and Where to Find Them |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Score

|-----|------------------------------|-----|-----|-------|-------|
| NUM |             NAME             | NOM | WIN |  ODDS |  PTS  |
|-----|------------------------------|-----|-----|-------|-------|
|   1 | La La Land                   |  12 |  11 | 9/5   | 55.56 |
|   2 | Jackie                       |  10 |   2 | 4/1   | 25.00 |
|   3 | Silence                      |   9 |   1 | 7/1   | 14.29 |
|   4 | Rogue One: A Star Wars Story |   6 |   0 | 14/1  |  7.14 |
|   5 | Arrival                      |   3 |   0 | 14/1  |  7.14 |
|   6 | Lion                         |   4 |   0 | 22/1  |  4.55 |
|   7 | The Jungle Book              |   5 |   0 | 25/1  |  4.00 |
|   8 | Nocturnal Animals            |   3 |   0 | 33/1  |  3.03 |
|   9 | Hidden Figures               |   2 |   0 | 50/1  |  2.00 |
|  10 | Moonlight                    |   1 |   0 | 66/1  |  1.52 |
|  11 | Florence Foster Jenkins      |   1 |   0 | 66/1  |  1.52 |
|  12 | Hacksaw Ridge                |   1 |   0 | 80/1  |  1.25 |
|  13 | Live By Night                |   1 |   0 | 100/1 |  1.00 |
|  14 | Zootopia                     |   1 |   0 | 100/1 |  1.00 |
|  15 | Fences                       |   1 |   0 | 100/1 |  1.00 |
|-----|------------------------------|-----|-----|-------|-------|


#### Best Sound Editing

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | Hacksaw Ridge                           |   9 |   9 | 7/4   | 57.14 |
|   2 | La La Land                              |   8 |   2 | 4/1   | 25.00 |
|   3 | Rogue One: A Star Wars Story            |   7 |   0 | 13/2  | 15.38 |
|   4 | Deepwater Horizon                       |   6 |   0 | 12/1  |  8.33 |
|   5 | Silence                                 |   4 |   0 | 14/1  |  7.14 |
|   6 | The Jungle Book                         |   4 |   0 | 14/1  |  7.14 |
|   7 | Arrival                                 |   2 |   0 | 25/1  |  4.00 |
|   8 | Live By Night                           |   1 |   0 | 50/1  |  2.00 |
|   9 | Doctor Strange                          |   1 |   0 | 100/1 |  1.00 |
|  10 | Passengers                              |   1 |   0 | 100/1 |  1.00 |
|  11 | Sully                                   |   1 |   0 | 100/1 |  1.00 |
|  12 | Fantastic Beasts and Where to Find Them |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Sound Mixing

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | La La Land                              |   9 |  11 | 3/2   | 66.67 |
|   2 | Hacksaw Ridge                           |   9 |   0 | 4/1   | 25.00 |
|   3 | Rogue One: A Star Wars Story            |   8 |   0 | 11/2  | 18.18 |
|   4 | Silence                                 |   5 |   0 | 10/1  | 10.00 |
|   5 | The Jungle Book                         |   4 |   0 | 16/1  |  6.25 |
|   6 | Deepwater Horizon                       |   4 |   0 | 25/1  |  4.00 |
|   7 | Fantastic Beasts and Where to Find Them |   2 |   0 | 50/1  |  2.00 |
|   8 | Passengers                              |   1 |   0 | 100/1 |  1.00 |
|   9 | Arrival                                 |   1 |   0 | 100/1 |  1.00 |
|  11 | Star Trek Beyond                        |   1 |   0 | 100/1 |  1.00 |
|  12 | Sully                                   |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Production Design

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | La La Land                              |  11 |  11 | 19/10 | 52.63 |
|   2 | Jackie                                  |  11 |   0 | 6/1   | 16.67 |
|   3 | Silence                                 |   9 |   0 | 13/2  | 15.38 |
|   4 | Fantastic Beasts and Where to Find Them |   9 |   1 | 15/2  | 13.33 |
|   5 | Rules Don't Apply                       |   5 |   1 | 14/1  |  7.14 |
|   6 | The Jungle Book                         |   3 |   1 | 22/1  |  4.55 |
|   7 | Live By Night                           |   2 |   0 | 22/1  |  4.55 |
|   8 | Rogue One: A Star Wars Story            |   3 |   0 | 28/1  |  3.57 |
|   9 | Hidden Figures                          |   3 |   0 | 33/1  |  3.03 |
|  10 | Hail, Caesar!                           |   1 |   0 | 66/1  |  1.52 |
|  11 | Hacksaw Ridge                           |   1 |   0 | 80/1  |  1.25 |
|  12 | Florence Foster Jenkins                 |   1 |   0 | 100/1 |  1.00 |
|  13 | Fences                                  |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Costume Design

|-----|-----------------------------------------|-----|-----|-------|-------|
| NUM |                   NAME                  | NOM | WIN |  ODDS |  PTS  |
|-----|-----------------------------------------|-----|-----|-------|-------|
|   1 | Jackie                                  |  11 |   5 | 11/4  | 36.36 |
|   2 | La La Land                              |  10 |   6 | 14/5  | 35.71 |
|   3 | Silence                                 |   7 |   1 | 6/1   | 16.67 |
|   4 | Florence Foster Jenkins                 |   7 |   1 | 8/1   | 12.50 |
|   5 | Live By Night                           |   3 |   0 | 16/1  |  6.25 |
|   6 | Fantastic Beasts and Where to Find Them |   5 |   0 | 18/1  |  5.56 |
|   7 | Allied                                  |   4 |   0 | 28/1  |  3.57 |
|   8 | Rules Don't Apply                       |   3 |   0 | 33/1  |  3.03 |
|   9 | Captain Fantastic                       |   2 |   0 | 50/1  |  2.00 |
|  10 | Love and Friendship                     |   2 |   0 | 66/1  |  1.52 |
|  11 | Hidden Figures                          |   1 |   0 | 100/1 |  1.00 |
|-----|-----------------------------------------|-----|-----|-------|-------|


#### Best Makeup and Hairstyling

|-----|---------------------------------------------|-----|-----|------|-------|
| NUM |                     NAME                    | NOM | WIN | ODDS |  PTS  |
|-----|---------------------------------------------|-----|-----|------|-------|
|   1 | Jackie                                      |  11 |  10 | 5/4  | 80.00 |
|   2 | Fantastic Beasts and Where to Find Them     |   6 |   1 | 7/1  | 14.29 |
|   3 | Silence                                     |   5 |   0 | 9/1  | 11.11 |
|   4 | Rogue One: A Star Wars Story                |   3 |   1 | 11/1 |  9.09 |
|   5 | Florence Foster Jenkins                     |   3 |   1 | 11/1 |  9.09 |
|   6 | Doctor Strange                              |   1 |   1 | 25/1 |  4.00 |
|   7 | Deadpool                                    |   2 |   0 | 28/1 |  3.57 |
|   8 | Loving                                      |   2 |   0 | 33/1 |  3.03 |
|   9 | A Monster Calls                             |   1 |   0 | 50/1 |  2.00 |
|  10 | Hacksaw Ridge                               |   1 |   0 | 50/1 |  2.00 |
|  11 | Miss Peregrine's Home for Peculiar Children |   1 |   0 | 50/1 |  2.00 |
|-----|---------------------------------------------|-----|-----|------|-------|


---

### Sort by movie

If you want to browse through all the different movies, here you go.

(As I mentioned earlier, I started this whole post as a way of experimenting with Markdown tables. But it turns out multi-line cells in Markdown tables are not supported by most Markdown converters, including the one in my blog software, Jekyll. Rather than try to painstakingly convert it manually, I'm just embedding my big ol' plain text chart here instead.)

If you don't want to skim through this, feel free to jump down to the list [sorted by score](#sort-by-score) instead.

```
|--------|---------------------------------------------------|-----------------------------|------------------------|
| TOTAL  |                       TITLE                       |           CATEGORY          |          NOM           |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  26.29 | 20th Century Women (Annette Bening)               | Best Actress                | 14.29 pts (7/1 odds)   |
|        | 20th Century Women (Greta Gerwig)                 | Best Supporting Actress     | 05.00 pts (20/1 odds)  |
|        | 20th Century Women                                | Best Original Screenplay    | 05.00 pts (20/1 odds)  |
|        | 20th Century Women (Elle Fanning)                 | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|        | 20th Century Women                                | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  12.28 | A Monster Calls                                   | Best Adapted Screenplay     | 04.00 pts (25/1 odds)  |
|        | A Monster Calls (Felicity Jones)                  | Best Supporting Actress     | 03.03 pts (33/1 odds)  |
|        | A Monster Calls                                   | Best Makeup and Hairstyling | 02.00 pts (50/1 odds)  |
|        | A Monster Calls                                   | Best Cinematography         | 01.25 pts (80/1 odds)  |
|        | A Monster Calls                                   | Best Visual Effects         | 01.00 pts (100/1 odds) |
|        | A Monster Calls                                   | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   3.57 | Allied                                            | Best Costume Design         | 03.57 pts (28/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   75.5 | Arrival                                           | Best Adapted Screenplay     | 20.00 pts (5/1 odds)   |
|        | Arrival                                           | Best Cinematography         | 16.67 pts (6/1 odds)   |
|        | Arrival                                           | Best Visual Effects         | 10.00 pts (10/1 odds)  |
|        | Arrival (Amy Adams)                               | Best Actress                | 07.14 pts (14/1 odds)  |
|        | Arrival                                           | Best Score                  | 07.14 pts (14/1 odds)  |
|        | Arrival                                           | Best Picture                | 05.00 pts (20/1 odds)  |
|        | Arrival                                           | Best Sound Editing          | 04.00 pts (25/1 odds)  |
|        | Arrival                                           | Best Film Editing           | 03.03 pts (33/1 odds)  |
|        | Arrival (Denis Villeneuve)                        | Best Director               | 01.52 pts (66/1 odds)  |
|        | Arrival                                           | Best Sound Mixing           | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   4.25 | Billy Lynn's Long Halftime Walk                   | Best Picture                | 01.00 pts (100/1 odds) |
|        | Billy Lynn's Long Halftime Walk (Ang Lee)         | Best Director               | 01.25 pts (80/1 odds)  |
|        | Billy Lynn's Long Halftime Walk (Kristen Stewart) | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|        | Billy Lynn's Long Halftime Walk (Steve Martin)    | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Bleed for This (Aaron Eckhart)                    | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Cafe Society                                      | Best Cinematography         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      4 | Captain America: Civil War                        | Best Visual Effects         | 04.00 pts (25/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|    5.5 | Captain Fantastic (Viggo Mortensen)               | Best Actor                  | 02.50 pts (40/1 odds)  |
|        | Captain Fantastic                                 | Best Costume Design         | 02.00 pts (50/1 odds)  |
|        | Captain Fantastic                                 | Best Original Screenplay    | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   4.57 | Deadpool                                          | Best Makeup and Hairstyling | 03.57 pts (28/1 odds)  |
|        | Deadpool                                          | Best Visual Effects         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  13.85 | Deepwater Horizon                                 | Best Sound Editing          | 08.33 pts (12/1 odds)  |
|        | Deepwater Horizon                                 | Best Sound Mixing           | 04.00 pts (25/1 odds)  |
|        | Deepwater Horizon                                 | Best Film Editing           | 01.52 pts (66/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   1.52 | Denial (Timothy Spall)                            | Best Supporting Actor       | 01.52 pts (66/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  39.33 | Doctor Strange                                    | Best Visual Effects         | 33.33 pts (3/1 odds)   |
|        | Doctor Strange                                    | Best Makeup and Hairstyling | 04.00 pts (25/1 odds)  |
|        | Doctor Strange                                    | Best Sound Editing          | 01.00 pts (100/1 odds) |
|        | Doctor Strange                                    | Best Cinematography         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   2.52 | Elle (Isabelle Huppert)                           | Best Actress                | 01.52 pts (66/1 odds)  |
|        | Elle                                              | Best Adapted Screenplay     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  49.29 | Fantastic Beasts and Where to Find Them           | Best Makeup and Hairstyling | 14.29 pts (7/1 odds)   |
|        | Fantastic Beasts and Where to Find Them           | Best Production Design      | 13.33 pts (15/2 odds)  |
|        | Fantastic Beasts and Where to Find Them           | Best Visual Effects         | 11.11 pts (9/1 odds)   |
|        | Fantastic Beasts and Where to Find Them           | Best Costume Design         | 05.56 pts (18/1 odds)  |
|        | Fantastic Beasts and Where to Find Them           | Best Sound Mixing           | 02.00 pts (50/1 odds)  |
|        | Fantastic Beasts and Where to Find Them           | Best Sound Editing          | 01.00 pts (100/1 odds) |
|        | Fantastic Beasts and Where to Find Them           | Best Film Editing           | 01.00 pts (100/1 odds) |
|        | Fantastic Beasts and Where to Find Them           | Best Cinematography         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
| 165.78 | Fences                                            | Best Adapted Screenplay     | 52.63 pts (19/10 odds) |
|        | Fences (Viola Davis)                              | Best Supporting Actress     | 50.00 pts (2/1 odds)   |
|        | Fences (Denzel Washington)                        | Best Actor                  | 35.71 pts (14/5 odds)  |
|        | Fences                                            | Best Picture                | 11.11 pts (9/1 odds)   |
|        | Fences (Denzel Washington)                        | Best Director               | 08.33 pts (12/1 odds)  |
|        | Fences (Stephen Henderson)                        | Best Supporting Actor       | 02.00 pts (50/1 odds)  |
|        | Fences (Jovan Adepo)                              | Best Supporting Actor       | 02.00 pts (50/1 odds)  |
|        | Fences (Viola Davis)                              | Best Actress                | 01.00 pts (100/1 odds) |
|        | Fences (Mykelti Williamson)                       | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|        | Fences                                            | Best Score                  | 01.00 pts (100/1 odds) |
|        | Fences                                            | Best Production Design      | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   13.5 | Finding Dory                                      | Best Animated Feature       | 12.50 pts (8/1 odds)   |
|        | Finding Dory                                      | Best Adapted Screenplay     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  28.11 | Florence Foster Jenkins                           | Best Costume Design         | 12.50 pts (8/1 odds)   |
|        | Florence Foster Jenkins                           | Best Makeup and Hairstyling | 09.09 pts (11/1 odds)  |
|        | Florence Foster Jenkins (Meryl Streep)            | Best Actress                | 02.00 pts (50/1 odds)  |
|        | Florence Foster Jenkins (Hugh Grant)              | Best Supporting Actor       | 02.00 pts (50/1 odds)  |
|        | Florence Foster Jenkins                           | Best Score                  | 01.52 pts (66/1 odds)  |
|        | Florence Foster Jenkins                           | Best Production Design      | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Gold (Matthew McConaughey)                        | Best Actor                  | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
| 103.18 | Hacksaw Ridge                                     | Best Sound Editing          | 57.14 pts (7/4 odds)   |
|        | Hacksaw Ridge                                     | Best Sound Mixing           | 25.00 pts (4/1 odds)   |
|        | Hacksaw Ridge                                     | Best Film Editing           | 10.00 pts (10/1 odds)  |
|        | Hacksaw Ridge (Andrew Garfield)                   | Best Actor                  | 02.50 pts (40/1 odds)  |
|        | Hacksaw Ridge                                     | Best Makeup and Hairstyling | 02.00 pts (50/1 odds)  |
|        | Hacksaw Ridge                                     | Best Picture                | 01.52 pts (66/1 odds)  |
|        | Hacksaw Ridge                                     | Best Adapted Screenplay     | 01.52 pts (66/1 odds)  |
|        | Hacksaw Ridge                                     | Best Score                  | 01.25 pts (80/1 odds)  |
|        | Hacksaw Ridge                                     | Best Production Design      | 01.25 pts (80/1 odds)  |
|        | Hacksaw Ridge (Mel Gibson)                        | Best Director               | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   3.04 | Hail, Caesar!                                     | Best Production Design      | 01.52 pts (66/1 odds)  |
|        | Hail, Caesar!                                     | Best Cinematography         | 01.52 pts (66/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  23.38 | Hell or High Water (Jeff Bridges)                 | Best Supporting Actor       | 15.38 pts (13/2 odds)  |
|        | Hell or High Water                                | Best Original Screenplay    | 05.00 pts (20/1 odds)  |
|        | Hell or High Water                                | Best Picture                | 02.00 pts (50/1 odds)  |
|        | Hell or High Water (Ben Foster)                   | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  30.43 | Hidden Figures                                    | Best Adapted Screenplay     | 06.25 pts (16/1 odds)  |
|        | Hidden Figures (Janelle Monae)                    | Best Supporting Actress     | 04.55 pts (22/1 odds)  |
|        | Hidden Figures (Taraji P. Henson)                 | Best Actress                | 04.00 pts (25/1 odds)  |
|        | Hidden Figures                                    | Best Film Editing           | 03.57 pts (28/1 odds)  |
|        | Hidden Figures                                    | Best Production Design      | 03.03 pts (33/1 odds)  |
|        | Hidden Figures                                    | Best Picture                | 03.03 pts (33/1 odds)  |
|        | Hidden Figures                                    | Best Score                  | 02.00 pts (50/1 odds)  |
|        | Hidden Figures (Theodore Melfi)                   | Best Director               | 01.00 pts (100/1 odds) |
|        | Hidden Figures (Octavia Spencer)                  | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|        | Hidden Figures (Kevin Costner)                    | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|        | Hidden Figures                                    | Best Costume Design         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  230.7 | Jackie                                            | Best Makeup and Hairstyling | 80.00 pts (5/4 odds)   |
|        | Jackie                                            | Best Costume Design         | 36.36 pts (11/4 odds)  |
|        | Jackie (Natalie Portman)                          | Best Actress                | 28.57 pts (7/2 odds)   |
|        | Jackie                                            | Best Score                  | 25.00 pts (4/1 odds)   |
|        | Jackie                                            | Best Production Design      | 16.67 pts (6/1 odds)   |
|        | Jackie                                            | Best Film Editing           | 15.38 pts (13/2 odds)  |
|        | Jackie                                            | Best Cinematography         | 11.11 pts (9/1 odds)   |
|        | Jackie                                            | Best Original Screenplay    | 08.33 pts (12/1 odds)  |
|        | Jackie                                            | Best Picture                | 06.25 pts (16/1 odds)  |
|        | Jackie (Pablo Larrain)                            | Best Director               | 03.03 pts (33/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|     20 | Kubo and the Two Strings                          | Best Animated Feature       | 20.00 pts (5/1 odds)   |
|--------|---------------------------------------------------|-----------------------------|------------------------|
| 504.46 | La La Land                                        | Best Sound Mixing           | 66.67 pts (3/2 odds)   |
|        | La La Land (Damien Chazelle)                      | Best Director               | 58.82 pts (17/10 odds) |
|        | La La Land                                        | Best Score                  | 55.56 pts (9/5 odds)   |
|        | La La Land                                        | Best Production Design      | 52.63 pts (19/10 odds) |
|        | La La Land                                        | Best Cinematography         | 52.63 pts (19/10 odds) |
|        | La La Land                                        | Best Film Editing           | 50.00 pts (2/1 odds)   |
|        | La La Land (Emma Stone)                           | Best Actress                | 47.62 pts (21/10 odds) |
|        | La La Land                                        | Best Costume Design         | 35.71 pts (14/5 odds)  |
|        | La La Land                                        | Best Sound Editing          | 25.00 pts (4/1 odds)   |
|        | La La Land                                        | Best Picture                | 22.22 pts (9/2 odds)   |
|        | La La Land                                        | Best Original Screenplay    | 22.22 pts (9/2 odds)   |
|        | La La Land (Ryan Gosling)                         | Best Actor                  | 15.38 pts (13/2 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  51.49 | Lion                                              | Best Adapted Screenplay     | 13.33 pts (15/2 odds)  |
|        | Lion (Nicole Kidman)                              | Best Supporting Actress     | 11.11 pts (9/1 odds)   |
|        | Lion (Dev Patel)                                  | Best Supporting Actor       | 11.11 pts (9/1 odds)   |
|        | Lion                                              | Best Picture                | 07.14 pts (14/1 odds)  |
|        | Lion                                              | Best Score                  | 04.55 pts (22/1 odds)  |
|        | Lion                                              | Best Cinematography         | 02.00 pts (50/1 odds)  |
|        | Lion (Garth Davis)                                | Best Director               | 01.25 pts (80/1 odds)  |
|        | Lion                                              | Best Film Editing           | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  18.37 | Live By Night                                     | Best Costume Design         | 06.25 pts (16/1 odds)  |
|        | Live By Night                                     | Best Production Design      | 04.55 pts (22/1 odds)  |
|        | Live By Night                                     | Best Cinematography         | 03.57 pts (28/1 odds)  |
|        | Live By Night                                     | Best Sound Editing          | 02.00 pts (50/1 odds)  |
|        | Live By Night                                     | Best Score                  | 01.00 pts (100/1 odds) |
|        | Live By Night                                     | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   2.77 | Love and Friendship                               | Best Costume Design         | 01.52 pts (66/1 odds)  |
|        | Love and Friendship                               | Best Adapted Screenplay     | 01.25 pts (80/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  50.73 | Loving (Ruth Negga)                               | Best Actress                | 16.67 pts (6/1 odds)   |
|        | Loving (Joel Edgerton)                            | Best Actor                  | 11.11 pts (9/1 odds)   |
|        | Loving                                            | Best Original Screenplay    | 09.09 pts (11/1 odds)  |
|        | Loving                                            | Best Picture                | 08.33 pts (12/1 odds)  |
|        | Loving                                            | Best Makeup and Hairstyling | 03.03 pts (33/1 odds)  |
|        | Loving (Jeff Nichols)                             | Best Director               | 02.50 pts (40/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  194.6 | Manchester by the Sea (Casey Affleck)             | Best Actor                  | 50.00 pts (2/1 odds)   |
|        | Manchester by the Sea                             | Best Original Screenplay    | 50.00 pts (2/1 odds)   |
|        | Manchester by the Sea (Michelle Williams)         | Best Supporting Actress     | 30.00 pts (10/3 odds)  |
|        | Manchester by the Sea (Kenneth Lonergan)          | Best Director               | 25.00 pts (4/1 odds)   |
|        | Manchester by the Sea (Lucas Hedges)              | Best Supporting Actor       | 22.22 pts (9/2 odds)   |
|        | Manchester by the Sea                             | Best Picture                | 15.38 pts (13/2 odds)  |
|        | Manchester by the Sea (Kyle Chandler)             | Best Supporting Actor       | 01.00 pts (100/1 odds) |
|        | Manchester by the Sea                             | Best Film Editing           | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Miss Hokusai                                      | Best Animated Feature       | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      7 | Miss Peregrine's Home for Peculiar Children       | Best Visual Effects         | 05.00 pts (20/1 odds)  |
|        | Miss Peregrine's Home for Peculiar Children       | Best Makeup and Hairstyling | 02.00 pts (50/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|    2.5 | Miss Sloane (Jessica Chastain)                    | Best Actress                | 02.50 pts (40/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  15.38 | Moana                                             | Best Animated Feature       | 15.38 pts (13/2 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
| 139.74 | Moonlight (Mahershala Ali)                        | Best Supporting Actor       | 41.67 pts (12/5 odds)  |
|        | Moonlight                                         | Best Original Screenplay    | 28.57 pts (7/2 odds)   |
|        | Moonlight (Naomie Harris)                         | Best Supporting Actress     | 20.00 pts (5/1 odds)   |
|        | Moonlight (Barry Jenkins)                         | Best Director               | 16.67 pts (6/1 odds)   |
|        | Moonlight                                         | Best Picture                | 11.11 pts (9/1 odds)   |
|        | Moonlight                                         | Best Cinematography         | 11.11 pts (9/1 odds)   |
|        | Moonlight                                         | Best Film Editing           | 09.09 pts (11/1 odds)  |
|        | Moonlight                                         | Best Score                  | 01.52 pts (66/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | My Life as a Zucchini                             | Best Animated Feature       | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  34.07 | Nocturnal Animals (Michael Shannon)               | Best Supporting Actor       | 11.11 pts (9/1 odds)   |
|        | Nocturnal Animals                                 | Best Adapted Screenplay     | 08.33 pts (12/1 odds)  |
|        | Nocturnal Animals                                 | Best Film Editing           | 03.57 pts (28/1 odds)  |
|        | Nocturnal Animals                                 | Best Score                  | 03.03 pts (33/1 odds)  |
|        | Nocturnal Animals                                 | Best Cinematography         | 03.03 pts (33/1 odds)  |
|        | Nocturnal Animals (Tom Ford)                      | Best Director               | 01.00 pts (100/1 odds) |
|        | Nocturnal Animals (Jake Gyllenhaal)               | Best Actor                  | 01.00 pts (100/1 odds) |
|        | Nocturnal Animals (Amy Adams)                     | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|        | Nocturnal Animals (Amy Adams)                     | Best Actress                | 01.00 pts (100/1 odds) |
|        | Nocturnal Animals                                 | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      5 | Passengers (Morten Tyldum)                        | Best Director               | 01.00 pts (100/1 odds) |
|        | Passengers (Jennifer Lawrence)                    | Best Actress                | 01.00 pts (100/1 odds) |
|        | Passengers                                        | Best Sound Mixing           | 01.00 pts (100/1 odds) |
|        | Passengers                                        | Best Sound Editing          | 01.00 pts (100/1 odds) |
|        | Passengers                                        | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Patriot's Day                                     | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Queen of Katwe (Lupita Nyong'o)                   | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  71.54 | Rogue One: A Star Wars Story                      | Best Visual Effects         | 18.18 pts (11/2 odds)  |
|        | Rogue One: A Star Wars Story                      | Best Sound Mixing           | 18.18 pts (11/2 odds)  |
|        | Rogue One: A Star Wars Story                      | Best Sound Editing          | 15.38 pts (13/2 odds)  |
|        | Rogue One: A Star Wars Story                      | Best Makeup and Hairstyling | 09.09 pts (11/1 odds)  |
|        | Rogue One: A Star Wars Story                      | Best Score                  | 07.14 pts (14/1 odds)  |
|        | Rogue One: A Star Wars Story                      | Best Production Design      | 03.57 pts (28/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  11.17 | Rules Don't Apply                                 | Best Production Design      | 07.14 pts (14/1 odds)  |
|        | Rules Don't Apply                                 | Best Costume Design         | 03.03 pts (33/1 odds)  |
|        | Rules Don't Apply (Warren Beatty)                 | Best Actor                  | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   3.57 | Sausage Party                                     | Best Animated Feature       | 03.57 pts (28/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
| 152.67 | Silence                                           | Best Film Editing           | 18.18 pts (11/2 odds)  |
|        | Silence                                           | Best Adapted Screenplay     | 18.18 pts (11/2 odds)  |
|        | Silence                                           | Best Costume Design         | 16.67 pts (6/1 odds)   |
|        | Silence                                           | Best Cinematography         | 16.67 pts (6/1 odds)   |
|        | Silence                                           | Best Production Design      | 15.38 pts (13/2 odds)  |
|        | Silence                                           | Best Score                  | 14.29 pts (7/1 odds)   |
|        | Silence                                           | Best Makeup and Hairstyling | 11.11 pts (9/1 odds)   |
|        | Silence                                           | Best Sound Mixing           | 10.00 pts (10/1 odds)  |
|        | Silence (Martin Scorsese)                         | Best Director               | 08.33 pts (12/1 odds)  |
|        | Silence (Liam Neeson)                             | Best Supporting Actor       | 08.33 pts (12/1 odds)  |
|        | Silence                                           | Best Sound Editing          | 07.14 pts (14/1 odds)  |
|        | Silence                                           | Best Picture                | 07.14 pts (14/1 odds)  |
|        | Silence (Andrew Garfield)                         | Best Actor                  | 01.25 pts (80/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   7.14 | Sing                                              | Best Animated Feature       | 07.14 pts (14/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Snowden                                           | Best Adapted Screenplay     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   2.52 | Star Trek Beyond                                  | Best Visual Effects         | 01.52 pts (66/1 odds)  |
|        | Star Trek Beyond                                  | Best Sound Mixing           | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  20.71 | Sully (Tom Hanks)                                 | Best Actor                  | 07.14 pts (14/1 odds)  |
|        | Sully                                             | Best Film Editing           | 04.00 pts (25/1 odds)  |
|        | Sully                                             | Best Picture                | 03.57 pts (28/1 odds)  |
|        | Sully                                             | Best Visual Effects         | 02.00 pts (50/1 odds)  |
|        | Sully (Clint Eastwood)                            | Best Director               | 01.00 pts (100/1 odds) |
|        | Sully                                             | Best Sound Mixing           | 01.00 pts (100/1 odds) |
|        | Sully                                             | Best Sound Editing          | 01.00 pts (100/1 odds) |
|        | Sully                                             | Best Adapted Screenplay     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | The BFG                                           | Best Visual Effects         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      3 | The Birth of a Nation (Nate Parker)               | Best Actor                  | 01.00 pts (100/1 odds) |
|        | The Birth of a Nation (Aja Naomi King)            | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|        | The Birth of a Nation                             | Best Picture                | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   2.52 | The Founder (Michael Keaton)                      | Best Actor                  | 01.52 pts (66/1 odds)  |
|        | The Founder (Laura Dern)                          | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | The Hollars (Margo Martindale)                    | Best Supporting Actress     | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  57.51 | The Jungle Book                                   | Best Visual Effects         | 30.00 pts (10/3 odds)  |
|        | The Jungle Book                                   | Best Sound Editing          | 07.14 pts (14/1 odds)  |
|        | The Jungle Book                                   | Best Sound Mixing           | 06.25 pts (16/1 odds)  |
|        | The Jungle Book                                   | Best Production Design      | 04.55 pts (22/1 odds)  |
|        | The Jungle Book                                   | Best Score                  | 04.00 pts (25/1 odds)  |
|        | The Jungle Book                                   | Best Film Editing           | 03.57 pts (28/1 odds)  |
|        | The Jungle Book                                   | Best Cinematography         | 02.00 pts (50/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|    2.5 | The Little Prince                                 | Best Animated Feature       | 02.50 pts (40/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | The Lobster                                       | Best Original Screenplay    | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   9.09 | The Red Turtle                                    | Best Animated Feature       | 09.09 pts (11/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|   1.25 | Trolls                                            | Best Animated Feature       | 01.25 pts (80/1 odds)  |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|      1 | Warcraft                                          | Best Visual Effects         | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
|  55.33 | Zootopia                                          | Best Animated Feature       | 53.33 pts (15/8 odds)  |
|        | Zootopia                                          | Best Original Screenplay    | 01.00 pts (100/1 odds) |
|        | Zootopia                                          | Best Score                  | 01.00 pts (100/1 odds) |
|--------|---------------------------------------------------|-----------------------------|------------------------|
```

---

### Sort by score

Here's the list of movies sorted by score and properly formatted as a bulleted list, to make it easier to read.

If this is all too long and verbose, feel free to [jump down to the final list](#final-list).

* **La La Land** (504.46 pts)
    - <small>66.67 pts for Best Sound Mixing *(3/2 odds)*</small>
    - <small>58.82 pts for Best Director (Damien Chazelle) *(17/10 odds)*</small>
    - <small>55.56 pts for Best Score *(9/5 odds)*</small>
    - <small>52.63 pts for Best Production Design *(19/10 odds)*</small>
    - <small>52.63 pts for Best Cinematography *(19/10 odds)*</small>
    - <small>50.00 pts for Best Film Editing *(2/1 odds)*</small>
    - <small>47.62 pts for Best Actress (Emma Stone) *(21/10 odds)*</small>
    - <small>35.71 pts for Best Costume Design *(14/5 odds)*</small>
    - <small>25.00 pts for Best Sound Editing *(4/1 odds)*</small>
    - <small>22.22 pts for Best Picture *(9/2 odds)*</small>
    - <small>22.22 pts for Best Original Screenplay *(9/2 odds)*</small>
    - <small>15.38 pts for Best Actor (Ryan Gosling) *(13/2 odds)*</small>
* **Jackie** (230.70 pts)
    - <small>80.00 pts for Best Makeup and Hairstyling *(5/4 odds)*</small>
    - <small>36.36 pts for Best Costume Design *(11/4 odds)*</small>
    - <small>28.57 pts for Best Actress (Natalie Portman) *(7/2 odds)*</small>
    - <small>25.00 pts for Best Score *(4/1 odds)*</small>
    - <small>16.67 pts for Best Production Design *(6/1 odds)*</small>
    - <small>15.38 pts for Best Film Editing *(13/2 odds)*</small>
    - <small>11.11 pts for Best Cinematography *(9/1 odds)*</small>
    - <small>08.33 pts for Best Original Screenplay *(12/1 odds)*</small>
    - <small>06.25 pts for Best Picture *(16/1 odds)*</small>
    - <small>03.03 pts for Best Director (Pablo Larrain) *(33/1 odds)*</small>
* **Manchester by the Sea** (194.60 pts)
    - <small>50.00 pts for Best Actor (Casey Affleck) *(2/1 odds)*</small>
    - <small>50.00 pts for Best Original Screenplay *(2/1 odds)*</small>
    - <small>30.00 pts for Best Supporting Actress (Michelle Williams) *(10/3 odds)*</small>
    - <small>25.00 pts for Best Director (Kenneth Lonergan) *(4/1 odds)*</small>
    - <small>22.22 pts for Best Supporting Actor (Lucas Hedges) *(9/2 odds)*</small>
    - <small>15.38 pts for Best Picture *(13/2 odds)*</small>
    - <small>01.00 pts for Best Supporting Actor (Kyle Chandler) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Film Editing *(100/1 odds)*</small>
* **Fences** (165.78 pts)
    - <small>52.63 pts for Best Adapted Screenplay *(19/10 odds)*</small>
    - <small>50.00 pts for Best Supporting Actress (Viola Davis) *(2/1 odds)*</small>
    - <small>35.71 pts for Best Actor (Denzel Washington) *(14/5 odds)*</small>
    - <small>11.11 pts for Best Picture *(9/1 odds)*</small>
    - <small>08.33 pts for Best Director (Denzel Washington) *(12/1 odds)*</small>
    - <small>02.00 pts for Best Supporting Actor (Stephen Henderson) *(50/1 odds)*</small>
    - <small>02.00 pts for Best Supporting Actor (Jovan Adepo) *(50/1 odds)*</small>
    - <small>01.00 pts for Best Actress (Viola Davis) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actor (Mykelti Williamson) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Score *(100/1 odds)*</small>
    - <small>01.00 pts for Best Production Design *(100/1 odds)*</small>
* **Silence** (152.67 pts)
    - <small>18.18 pts for Best Film Editing *(11/2 odds)*</small>
    - <small>18.18 pts for Best Adapted Screenplay *(11/2 odds)*</small>
    - <small>16.67 pts for Best Costume Design *(6/1 odds)*</small>
    - <small>16.67 pts for Best Cinematography *(6/1 odds)*</small>
    - <small>15.38 pts for Best Production Design *(13/2 odds)*</small>
    - <small>14.29 pts for Best Score *(7/1 odds)*</small>
    - <small>11.11 pts for Best Makeup and Hairstyling *(9/1 odds)*</small>
    - <small>10.00 pts for Best Sound Mixing *(10/1 odds)*</small>
    - <small>08.33 pts for Best Director (Martin Scorsese) *(12/1 odds)*</small>
    - <small>08.33 pts for Best Supporting Actor (Liam Neeson) *(12/1 odds)*</small>
    - <small>07.14 pts for Best Sound Editing *(14/1 odds)*</small>
    - <small>07.14 pts for Best Picture *(14/1 odds)*</small>
    - <small>01.25 pts for Best Actor (Andrew Garfield) *(80/1 odds)*</small>
* **Moonlight** (139.74 pts)
    - <small>41.67 pts for Best Supporting Actor (Mahershala Ali) *(12/5 odds)*</small>
    - <small>28.57 pts for Best Original Screenplay *(7/2 odds)*</small>
    - <small>20.00 pts for Best Supporting Actress (Naomie Harris) *(5/1 odds)*</small>
    - <small>16.67 pts for Best Director (Barry Jenkins) *(6/1 odds)*</small>
    - <small>11.11 pts for Best Picture *(9/1 odds)*</small>
    - <small>11.11 pts for Best Cinematography *(9/1 odds)*</small>
    - <small>09.09 pts for Best Film Editing *(11/1 odds)*</small>
    - <small>01.52 pts for Best Score *(66/1 odds)*</small>
* **Hacksaw Ridge** (103.18 pts)
    - <small>57.14 pts for Best Sound Editing *(7/4 odds)*</small>
    - <small>25.00 pts for Best Sound Mixing *(4/1 odds)*</small>
    - <small>10.00 pts for Best Film Editing *(10/1 odds)*</small>
    - <small>02.50 pts for Best Actor (Andrew Garfield) *(40/1 odds)*</small>
    - <small>02.00 pts for Best Makeup and Hairstyling *(50/1 odds)*</small>
    - <small>01.52 pts for Best Picture *(66/1 odds)*</small>
    - <small>01.52 pts for Best Adapted Screenplay *(66/1 odds)*</small>
    - <small>01.25 pts for Best Score *(80/1 odds)*</small>
    - <small>01.25 pts for Best Production Design *(80/1 odds)*</small>
    - <small>01.00 pts for Best Director (Mel Gibson) *(100/1 odds)*</small>
* **Arrival** (75.50 pts)
    - <small>20.00 pts for Best Adapted Screenplay *(5/1 odds)*</small>
    - <small>16.67 pts for Best Cinematography *(6/1 odds)*</small>
    - <small>10.00 pts for Best Visual Effects *(10/1 odds)*</small>
    - <small>07.14 pts for Best Actress (Amy Adams) *(14/1 odds)*</small>
    - <small>07.14 pts for Best Score *(14/1 odds)*</small>
    - <small>05.00 pts for Best Picture *(20/1 odds)*</small>
    - <small>04.00 pts for Best Sound Editing *(25/1 odds)*</small>
    - <small>03.03 pts for Best Film Editing *(33/1 odds)*</small>
    - <small>01.52 pts for Best Director (Denis Villeneuve) *(66/1 odds)*</small>
    - <small>01.00 pts for Best Sound Mixing *(100/1 odds)*</small>
* **Rogue One: A Star Wars Story** (71.54 pts)
    - <small>18.18 pts for Best Visual Effects *(11/2 odds)*</small>
    - <small>18.18 pts for Best Sound Mixing *(11/2 odds)*</small>
    - <small>15.38 pts for Best Sound Editing *(13/2 odds)*</small>
    - <small>09.09 pts for Best Makeup and Hairstyling *(11/1 odds)*</small>
    - <small>07.14 pts for Best Score *(14/1 odds)*</small>
    - <small>03.57 pts for Best Production Design *(28/1 odds)*</small>
* **The Jungle Book** (57.51 pts)
    - <small>30.00 pts for Best Visual Effects *(10/3 odds)*</small>
    - <small>07.14 pts for Best Sound Editing *(14/1 odds)*</small>
    - <small>06.25 pts for Best Sound Mixing *(16/1 odds)*</small>
    - <small>04.55 pts for Best Production Design *(22/1 odds)*</small>
    - <small>04.00 pts for Best Score *(25/1 odds)*</small>
    - <small>03.57 pts for Best Film Editing *(28/1 odds)*</small>
    - <small>02.00 pts for Best Cinematography *(50/1 odds)*</small>
* **Zootopia** (55.33 pts)
    - <small>53.33 pts for Best Animated Feature *(15/8 odds)*</small>
    - <small>01.00 pts for Best Original Screenplay *(100/1 odds)*</small>
    - <small>01.00 pts for Best Score *(100/1 odds)*</small>
* **Lion** (51.49 pts)
    - <small>13.33 pts for Best Adapted Screenplay *(15/2 odds)*</small>
    - <small>11.11 pts for Best Supporting Actress (Nicole Kidman) *(9/1 odds)*</small>
    - <small>11.11 pts for Best Supporting Actor (Dev Patel) *(9/1 odds)*</small>
    - <small>07.14 pts for Best Picture *(14/1 odds)*</small>
    - <small>04.55 pts for Best Score *(22/1 odds)*</small>
    - <small>02.00 pts for Best Cinematography *(50/1 odds)*</small>
    - <small>01.25 pts for Best Director (Garth Davis) *(80/1 odds)*</small>
    - <small>01.00 pts for Best Film Editing *(100/1 odds)*</small>
* **Loving** (50.73 pts)
    - <small>16.67 pts for Best Actress (Ruth Negga) *(6/1 odds)*</small>
    - <small>11.11 pts for Best Actor (Joel Edgerton) *(9/1 odds)*</small>
    - <small>09.09 pts for Best Original Screenplay *(11/1 odds)*</small>
    - <small>08.33 pts for Best Picture *(12/1 odds)*</small>
    - <small>03.03 pts for Best Makeup and Hairstyling *(33/1 odds)*</small>
    - <small>02.50 pts for Best Director (Jeff Nichols) *(40/1 odds)*</small>
* **Fantastic Beasts and Where to Find Them** (49.29 pts)
    - <small>14.29 pts for Best Makeup and Hairstyling *(7/1 odds)*</small>
    - <small>13.33 pts for Best Production Design *(15/2 odds)*</small>
    - <small>11.11 pts for Best Visual Effects *(9/1 odds)*</small>
    - <small>05.56 pts for Best Costume Design *(18/1 odds)*</small>
    - <small>02.00 pts for Best Sound Mixing *(50/1 odds)*</small>
    - <small>01.00 pts for Best Sound Editing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Film Editing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Cinematography *(100/1 odds)*</small>
* **Doctor Strange** (39.33 pts)
    - <small>33.33 pts for Best Visual Effects *(3/1 odds)*</small>
    - <small>04.00 pts for Best Makeup and Hairstyling *(25/1 odds)*</small>
    - <small>01.00 pts for Best Sound Editing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Cinematography *(100/1 odds)*</small>
* **Nocturnal Animals** (34.07 pts)
    - <small>11.11 pts for Best Supporting Actor (Michael Shannon) *(9/1 odds)*</small>
    - <small>08.33 pts for Best Adapted Screenplay *(12/1 odds)*</small>
    - <small>03.57 pts for Best Film Editing *(28/1 odds)*</small>
    - <small>03.03 pts for Best Score *(33/1 odds)*</small>
    - <small>03.03 pts for Best Cinematography *(33/1 odds)*</small>
    - <small>01.00 pts for Best Director (Tom Ford) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Actor (Jake Gyllenhaal) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Amy Adams) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Actress (Amy Adams) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Hidden Figures** (30.43 pts)
    - <small>06.25 pts for Best Adapted Screenplay *(16/1 odds)*</small>
    - <small>04.55 pts for Best Supporting Actress (Janelle Monae) *(22/1 odds)*</small>
    - <small>04.00 pts for Best Actress (Taraji P. Henson) *(25/1 odds)*</small>
    - <small>03.57 pts for Best Film Editing *(28/1 odds)*</small>
    - <small>03.03 pts for Best Production Design *(33/1 odds)*</small>
    - <small>03.03 pts for Best Picture *(33/1 odds)*</small>
    - <small>02.00 pts for Best Score *(50/1 odds)*</small>
    - <small>01.00 pts for Best Director (Theodore Melfi) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Octavia Spencer) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actor (Kevin Costner) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Costume Design *(100/1 odds)*</small>
* **Florence Foster Jenkins** (28.11 pts)
    - <small>12.50 pts for Best Costume Design *(8/1 odds)*</small>
    - <small>09.09 pts for Best Makeup and Hairstyling *(11/1 odds)*</small>
    - <small>02.00 pts for Best Actress (Meryl Streep) *(50/1 odds)*</small>
    - <small>02.00 pts for Best Supporting Actor (Hugh Grant) *(50/1 odds)*</small>
    - <small>01.52 pts for Best Score *(66/1 odds)*</small>
    - <small>01.00 pts for Best Production Design *(100/1 odds)*</small>
* **20th Century Women** (26.29 pts)
    - <small>14.29 pts for Best Actress (Annette Bening) *(7/1 odds)*</small>
    - <small>05.00 pts for Best Supporting Actress (Greta Gerwig) *(20/1 odds)*</small>
    - <small>05.00 pts for Best Original Screenplay *(20/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Elle Fanning) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Hell or High Water** (23.38 pts)
    - <small>15.38 pts for Best Supporting Actor (Jeff Bridges) *(13/2 odds)*</small>
    - <small>05.00 pts for Best Original Screenplay *(20/1 odds)*</small>
    - <small>02.00 pts for Best Picture *(50/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actor (Ben Foster) *(100/1 odds)*</small>
* **Sully** (20.71 pts)
    - <small>07.14 pts for Best Actor (Tom Hanks) *(14/1 odds)*</small>
    - <small>04.00 pts for Best Film Editing *(25/1 odds)*</small>
    - <small>03.57 pts for Best Picture *(28/1 odds)*</small>
    - <small>02.00 pts for Best Visual Effects *(50/1 odds)*</small>
    - <small>01.00 pts for Best Director (Clint Eastwood) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Sound Mixing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Sound Editing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Adapted Screenplay *(100/1 odds)*</small>
* **Kubo and the Two Strings** (20.00 pts)
    - <small>20.00 pts for Best Animated Feature *(5/1 odds)*</small>
* **Live By Night** (18.37 pts)
    - <small>06.25 pts for Best Costume Design *(16/1 odds)*</small>
    - <small>04.55 pts for Best Production Design *(22/1 odds)*</small>
    - <small>03.57 pts for Best Cinematography *(28/1 odds)*</small>
    - <small>02.00 pts for Best Sound Editing *(50/1 odds)*</small>
    - <small>01.00 pts for Best Score *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Moana** (15.38 pts)
    - <small>15.38 pts for Best Animated Feature *(13/2 odds)*</small>
* **Deepwater Horizon** (13.85 pts)
    - <small>08.33 pts for Best Sound Editing *(12/1 odds)*</small>
    - <small>04.00 pts for Best Sound Mixing *(25/1 odds)*</small>
    - <small>01.52 pts for Best Film Editing *(66/1 odds)*</small>
* **Finding Dory** (13.50 pts)
    - <small>12.50 pts for Best Animated Feature *(8/1 odds)*</small>
    - <small>01.00 pts for Best Adapted Screenplay *(100/1 odds)*</small>
* **A Monster Calls** (12.28 pts)
    - <small>04.00 pts for Best Adapted Screenplay *(25/1 odds)*</small>
    - <small>03.03 pts for Best Supporting Actress (Felicity Jones) *(33/1 odds)*</small>
    - <small>02.00 pts for Best Makeup and Hairstyling *(50/1 odds)*</small>
    - <small>01.25 pts for Best Cinematography *(80/1 odds)*</small>
    - <small>01.00 pts for Best Visual Effects *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Rules Don't Apply** (11.17 pts)
    - <small>07.14 pts for Best Production Design *(14/1 odds)*</small>
    - <small>03.03 pts for Best Costume Design *(33/1 odds)*</small>
    - <small>01.00 pts for Best Actor (Warren Beatty) *(100/1 odds)*</small>
* **The Red Turtle** (9.09 pts)
    - <small>09.09 pts for Best Animated Feature *(11/1 odds)*</small>
* **Sing** (7.14 pts)
    - <small>07.14 pts for Best Animated Feature *(14/1 odds)*</small>
* **Miss Peregrine's Home for Peculiar Children** (7.00 pts)
    - <small>05.00 pts for Best Visual Effects *(20/1 odds)*</small>
    - <small>02.00 pts for Best Makeup and Hairstyling *(50/1 odds)*</small>
* **Captain Fantastic** (5.50 pts)
    - <small>02.50 pts for Best Actor (Viggo Mortensen) *(40/1 odds)*</small>
    - <small>02.00 pts for Best Costume Design *(50/1 odds)*</small>
    - <small>01.00 pts for Best Original Screenplay *(100/1 odds)*</small>
* **Passengers** (5.00 pts)
    - <small>01.00 pts for Best Director (Morten Tyldum) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Actress (Jennifer Lawrence) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Sound Mixing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Sound Editing *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Deadpool** (4.57 pts)
    - <small>03.57 pts for Best Makeup and Hairstyling *(28/1 odds)*</small>
    - <small>01.00 pts for Best Visual Effects *(100/1 odds)*</small>
* **Billy Lynn's Long Halftime Walk** (4.25 pts)
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
    - <small>01.25 pts for Best Director (Ang Lee) *(80/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Kristen Stewart) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actor (Steve Martin) *(100/1 odds)*</small>
* **Captain America: Civil War** (4.00 pts)
    - <small>04.00 pts for Best Visual Effects *(25/1 odds)*</small>
* **Allied** (3.57 pts)
    - <small>03.57 pts for Best Costume Design *(28/1 odds)*</small>
* **Sausage Party** (3.57 pts)
    - <small>03.57 pts for Best Animated Feature *(28/1 odds)*</small>
* **Hail, Caesar!** (3.04 pts)
    - <small>01.52 pts for Best Production Design *(66/1 odds)*</small>
    - <small>01.52 pts for Best Cinematography *(66/1 odds)*</small>
* **The Birth of a Nation** (3.00 pts)
    - <small>01.00 pts for Best Actor (Nate Parker) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Aja Naomi King) *(100/1 odds)*</small>
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Love and Friendship** (2.77 pts)
    - <small>01.52 pts for Best Costume Design *(66/1 odds)*</small>
    - <small>01.25 pts for Best Adapted Screenplay *(80/1 odds)*</small>
* **Elle** (2.52 pts)
    - <small>01.52 pts for Best Actress (Isabelle Huppert) *(66/1 odds)*</small>
    - <small>01.00 pts for Best Adapted Screenplay *(100/1 odds)*</small>
* **Star Trek Beyond** (2.52 pts)
    - <small>01.52 pts for Best Visual Effects *(66/1 odds)*</small>
    - <small>01.00 pts for Best Sound Mixing *(100/1 odds)*</small>
* **The Founder** (2.52 pts)
    - <small>01.52 pts for Best Actor (Michael Keaton) *(66/1 odds)*</small>
    - <small>01.00 pts for Best Supporting Actress (Laura Dern) *(100/1 odds)*</small>
* **Miss Sloane** (2.50 pts)
    - <small>02.50 pts for Best Actress (Jessica Chastain) *(40/1 odds)*</small>
* **The Little Prince** (2.50 pts)
    - <small>02.50 pts for Best Animated Feature *(40/1 odds)*</small>
* **Denial** (1.52 pts)
    - <small>01.52 pts for Best Supporting Actor (Timothy Spall) *(66/1 odds)*</small>
* **Trolls** (1.25 pts)
    - <small>01.25 pts for Best Animated Feature *(80/1 odds)*</small>
* **Bleed for This** (1.00 pts)
    - <small>01.00 pts for Best Supporting Actor (Aaron Eckhart) *(100/1 odds)*</small>
* **Cafe Society** (1.00 pts)
    - <small>01.00 pts for Best Cinematography *(100/1 odds)*</small>
* **Gold** (1.00 pts)
    - <small>01.00 pts for Best Actor (Matthew McConaughey) *(100/1 odds)*</small>
* **Miss Hokusai** (1.00 pts)
    - <small>01.00 pts for Best Animated Feature *(100/1 odds)*</small>
* **My Life as a Zucchini** (1.00 pts)
    - <small>01.00 pts for Best Animated Feature *(100/1 odds)*</small>
* **Patriot's Day** (1.00 pts)
    - <small>01.00 pts for Best Picture *(100/1 odds)*</small>
* **Queen of Katwe** (1.00 pts)
    - <small>01.00 pts for Best Supporting Actress (Lupita Nyong'o) *(100/1 odds)*</small>
* **Snowden** (1.00 pts)
    - <small>01.00 pts for Best Adapted Screenplay *(100/1 odds)*</small>
* **The BFG** (1.00 pts)
    - <small>01.00 pts for Best Visual Effects *(100/1 odds)*</small>
* **The Hollars** (1.00 pts)
    - <small>01.00 pts for Best Supporting Actress (Margo Martindale) *(100/1 odds)*</small>
* **The Lobster** (1.00 pts)
    - <small>01.00 pts for Best Original Screenplay *(100/1 odds)*</small>
* **Warcraft** (1.00 pts)
    - <small>01.00 pts for Best Visual Effects *(100/1 odds)*</small>

---

### Final list

And finally, here's our overall list of movies!

Remember, this isn't the movies most likely to win Best Picture, but rather an aggregated list of movies most likely to score Oscar nominations/wins in ANY category. So some of these movies are "punching above their weight" because they are likely to win more of the technical awards.

All in all, it's a pretty interesting list. The 1st-ranked movie has more than twice the score of the 2nd-ranked movie. There are 7 movies with 100+ points, 13 movies with 50+ points, and 28 movies with 10+ points. And at the end of the list, 12 lonely movies with just 1 point each.

(The dates are color-coded based on whether the movie was playing in my local theaters. Green means the movie is not out yet, yellow means it's currently playing, red means it's out of theatres already. It doesn't always correspond exactly to the dates listed because those are often when the movie debuted in limited release, not wide release.)

Looks like I have a lot of catching up to do before February!

|-----|--------------|-------------------------------------------------|-------------------------------------------------|
| Num |    Points    |                      Title                      |                     Release                     |
|-----|--------------|-------------------------------------------------|-------------------------------------------------|
|  1. | *504.46 pts* | **La La Land**                                  | <span style="color:limegreen">2016-12-16</span> |
|  2. | *230.70 pts* | **Jackie**                                      | <span style="color:limegreen">2016-12-09</span> |
|  3. | *194.60 pts* | **Manchester by the Sea**                       | <span style="color:gold">2016-12-02</span>      |
|  4. | *165.78 pts* | **Fences**                                      | <span style="color:limegreen">2016-12-25</span> |
|  5. | *152.67 pts* | **Silence**                                     | <span style="color:limegreen">2016-12-23</span> |
|  6. | *139.74 pts* | **Moonlight**                                   | <span style="color:gold">2016-10-21</span>      |
|  7. | *103.18 pts* | **Hacksaw Ridge**                               | <span style="color:gold">2016-11-04</span>      |
|  8. | *75.50 pts*  | **Arrival**                                     | <span style="color:gold">2016-11-11</span>      |
|  9. | *71.54 pts*  | **Rogue One: A Star Wars Story**                | <span style="color:limegreen">2016-12-16</span> |
| 10. | *57.51 pts*  | **The Jungle Book**                             | <span style="color:crimson">2016-04-15</span>   |
| 11. | *55.33 pts*  | **Zootopia**                                    | <span style="color:crimson">2016-03-04</span>   |
| 12. | *51.49 pts*  | **Lion**                                        | <span style="color:limegreen">2016-11-25</span> |
| 13. | *50.73 pts*  | **Loving**                                      | <span style="color:gold">2016-11-04</span>      |
| 14. | *49.29 pts*  | **Fantastic Beasts and Where to Find Them**     | <span style="color:gold">2016-11-18</span>      |
| 15. | *39.33 pts*  | **Doctor Strange**                              | <span style="color:gold">2016-11-04</span>      |
| 16. | *34.07 pts*  | **Nocturnal Animals**                           | <span style="color:gold">2016-11-18</span>      |
| 17. | *30.43 pts*  | **Hidden Figures**                              | <span style="color:limegreen">2017-01-06</span> |
| 18. | *28.11 pts*  | **Florence Foster Jenkins**                     | <span style="color:crimson">2016-08-12</span>   |
| 19. | *26.29 pts*  | **20th Century Women**                          | <span style="color:limegreen">2016-12-25</span> |
| 20. | *23.38 pts*  | **Hell or High Water**                          | <span style="color:crimson">2016-08-12</span>   |
| 21. | *20.71 pts*  | **Sully**                                       | <span style="color:crimson">2016-11-09</span>   |
| 22. | *20.00 pts*  | **Kubo and the Two Strings**                    | <span style="color:crimson">2016-08-19</span>   |
| 23. | *18.37 pts*  | **Live By Night**                               | <span style="color:limegreen">2017-01-13</span> |
| 24. | *15.38 pts*  | **Moana**                                       | <span style="color:gold">2016-11-23</span>      |
| 25. | *13.85 pts*  | **Deepwater Horizon**                           | <span style="color:crimson">2016-09-30</span>   |
| 26. | *13.50 pts*  | **Finding Dory**                                | <span style="color:crimson">2016-06-17</span>   |
| 27. | *12.28 pts*  | **A Monster Calls**                             | <span style="color:limegreen">2016-12-23</span> |
| 28. | *11.17 pts*  | **Rules Don't Apply**                           | <span style="color:gold">2016-11-23</span>      |
| 29. | *9.09 pts*   | **The Red Turtle**                              | <span style="color:limegreen">2017-01-20</span> |
| 30. | *7.14 pts*   | **Sing**                                        | <span style="color:limegreen">2016-12-21</span> |
| 31. | *7.00 pts*   | **Miss Peregrine's Home for Peculiar Children** | <span style="color:crimson">2016-09-30</span>   |
| 32. | *5.50 pts*   | **Captain Fantastic**                           | <span style="color:crimson">2016-07-08</span>   |
| 33. | *5.00 pts*   | **Passengers**                                  | <span style="color:limegreen">2016-12-21</span> |
| 34. | *4.57 pts*   | **Deadpool**                                    | <span style="color:crimson">2016-02-12</span>   |
| 35. | *4.25 pts*   | **Billy Lynn's Long Halftime Walk**             | <span style="color:crimson">2016-11-18</span>   |
| 36. | *4.00 pts*   | **Captain America: Civil War**                  | <span style="color:crimson">2016-05-06</span>   |
| 37. | *3.57 pts*   | **Sausage Party**                               | <span style="color:crimson">2016-08-12</span>   |
| 38. | *3.57 pts*   | **Allied**                                      | <span style="color:gold">2016-11-23</span>      |
| 39. | *3.04 pts*   | **Hail, Caesar!**                               | <span style="color:crimson">2016-02-05</span>   |
| 40. | *3.00 pts*   | **The Birth of a Nation**                       | <span style="color:crimson">2016-10-07</span>   |
| 41. | *2.77 pts*   | **Love and Friendship**                         | <span style="color:crimson">2016-05-13</span>   |
| 42. | *2.52 pts*   | **The Founder**                                 | <span style="color:limegreen">2016-12-16</span> |
| 43. | *2.52 pts*   | **Star Trek Beyond**                            | <span style="color:crimson">2016-07-22</span>   |
| 44. | *2.52 pts*   | **Elle**                                        | <span style="color:gold">2016-11-11</span>      |
| 45. | *2.50 pts*   | **The Little Prince**                           | <span style="color:gold">2016-08-05</span>      |
| 46. | *2.50 pts*   | **Miss Sloane**                                 | <span style="color:limegreen">2016-12-09</span> |
| 47. | *1.52 pts*   | **Denial**                                      | <span style="color:crimson">2016-09-30</span>   |
| 48. | *1.25 pts*   | **Trolls**                                      | <span style="color:gold">2016-11-04</span>      |
| 49. | *1.00 pts*   | **Warcraft**                                    | <span style="color:crimson">2016-06-10</span>   |
| 50. | *1.00 pts*   | **The Lobster**                                 | <span style="color:crimson">2016-05-13</span>   |
| 51. | *1.00 pts*   | **The Hollars**                                 | <span style="color:crimson">2016-08-26</span>   |
| 52. | *1.00 pts*   | **The BFG**                                     | <span style="color:crimson">2016-07-01</span>   |
| 53. | *1.00 pts*   | **Snowden**                                     | <span style="color:crimson">2016-09-16</span>   |
| 54. | *1.00 pts*   | **Queen of Katwe**                              | <span style="color:crimson">2016-09-23</span>   |
| 55. | *1.00 pts*   | **Patriot's Day**                               | <span style="color:limegreen">2016-12-21</span> |
| 56. | *1.00 pts*   | **My Life as a Zucchini**                       | <span style="color:gold">2016-11-11</span>      |
| 57. | *1.00 pts*   | **Miss Hokusai**                                | <span style="color:crimson">2016-10-14</span>   |
| 58. | *1.00 pts*   | **Gold**                                        | <span style="color:limegreen">2017-01-27</span> |
| 59. | *1.00 pts*   | **Cafe Society**                                | <span style="color:crimson">2016-07-15</span>   |
| 60. | *1.00 pts*   | **Bleed for This**                              | <span style="color:gold">2016-11-18</span>      |
|-----|--------------|-------------------------------------------------|-------------------------------------------------|