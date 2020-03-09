# Basic Spring MVC + MySQL Blog App
> Sample project from Spring + MySQL workshop

## Table of content:
- [Database](#database)
- [SQL data for import](#sql)

- [Download project](https://lide.uhk.cz/fim/ucitel/macinmi1/blog.zip)

### Database

**1. [RemoteMysql Hosting](https://remotemysql.com/)**

**2. Docker**
```
docker run --name mysql-db -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=yes -e MYSQL_DATABASE=blog-db -e MYSQL_USER=blog-admin -e MYSQL_PASSWORD=heslo123 -d mysql:5.7 --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci
```

### SQL
```
INSERT INTO `blog-db`.`user` (`id`, `email`, `username`) VALUES
(1, 'macinmi1@uhk.cz', 'macinmi1'),
(2, 'michal.macinka@gmail.com', 'thatismybad');

INSERT INTO `blog-db`.`article` (`id`, `content`, `date`, `title`, `author_id`) VALUES
(1, 'The New Hampshire Department of Health and Human Services has announced a person in New Hampshire is being tested for the new coronavirus. The person recently returned from Italy and developed a fever and respiratory symptoms after returning.', '2020-03-02 00:00:00.000000', 'Person being tested for coronavirus in New Hampshire', 1),
(2, '(Reuters) - U.S. stock index futures tumbled when trading reopened on Sunday night with investors still unnerved by coronavirus and taking little solace from weekend comments by U.S. officials that aimed to soothe panic about a pandemic. \r\nSenior officials in President Donald Trump’s administration on Sunday tried to reduce concern about a global recession, saying the U.S. public had over-reacted and that stocks would rebound due to the American economy’s underlying strength.\r\n\r\nS&P 500 e-mini futures ESc1 were down 1.6%, indicating a another bad day for the benchmark index on Monday after it fell more than 11% last week, its worst since the 2008 financial crisis.', '2020-02-21 00:00:00.000000', 'U.S. stock futures resume coronavirus rout as trading resumes', 1),
(3, 'SANTIAGO (Reuters) - A study by Massachusetts Institute of Technology experts that called into question the alleged election fraud that drove Bolivian President Evo Morales to resign has triggered sniping between left and right-leaning governments in Latin America.', '2020-02-22 00:00:00.000000', 'Study casting doubt on Bolivian election fraud triggers controversy', 2),
(4, 'Young people from Black, Asian and other minority ethnic backgrounds are at greater risk of being in unstable employment, according to research.\r\n\r\nThe group is 47% more likely to to be on a zero-hours contract, a study said.\r\n\r\nA report from the Carnegie Trust, University College London\'s Centre for Longitudinal Studies and Operation Black Vote says the group is 4% less likely to have a permanent job.\r\n\r\nThe researchers compared the experiences of 25-year-olds in England.\r\n\r\nIt included people who are white, as well mixed-race, Indian, Pakistani, Bangladeshi, Black African and Caribbean, and other minority ethnicities, sometimes collectively known as BAME workers.\r\n\r\nThe report follows research that about a third of FTSE 100 firms have no ethnic minority board members.\r\n\r\n\'Precarious work\'\r\nThe study also found that such unsecure work could be linked to mental ill health.\r\n\r\nDouglas White from Carnegie UK Trust said: \"Good work can have a really positive impact on people\'s wellbeing - but we need to tackle the inequalities in who has access to good quality jobs. This report highlights that young people from BAME communities are particularly likely to enter into precarious forms of work. We need policy and practice to recognise and respond to this to ensure that good work is available to all.\"\r\n\r\nThe report suggests that employers should carry out internal audits of pay, employment terms and promotions when it comes to race.\r\n\r\nIt also suggests government action on the gap in pay BAME workers suffer.', '2020-02-27 00:00:00.000000', 'Young ethnic minority workers more likely to be in unstable jobs - study', 1),
(5, 'BOULDER, Colo., (CBS4) — The spread of the novel coronavirus is creating major, last-minute decisions for a large number of CU students studying around the world. On Friday, the university decided to suspend all study abroad programs in Italy.\r\n\r\nStudents currently studying abroad in the country have the option to transfer to programs in different countries or return home and continue their courses online.', '2020-02-28 00:00:00.000000', 'CU Suspends Study Abroad In Italy Due To Coronavirus Concerns', 2),
(6, 'The coronavirus\' global death toll has reached nearly 3,000 as countries around the world continue to report their findings to the World Health Organization.\r\n\r\nAt least 74 cases and one death have been detected in the U.S., according to the Centers for Disease Control and Prevention.\r\n\r\nHere is how the situation is unfolding on Sunday (all times Eastern).\r\n\r\n5:30 p.m. American Airlines waives change fees for flights\r\nAmerican Airlines joins the growing list of air carriers that will waive fees for all of its flights due to coronavirus concerns.\r\n\r\nAll travelers who book an American flight between March 1 and March 16 can have their change fee waived as long as the request is made up to 14 days prior to the flight, airline officials announced Sunday evening.\r\n\r\n\"This change offers customers the best fares with even more flexibility,\" an American Airlines spokesperson said in a statement.', '2020-02-28 00:00:00.000000', 'Global death toll of coronavirus reaches nearly 3,000 after confirmed cases in Iran spikes overnight', 1),
(7, 'Watch \"First U.S. coronavirus death reported in Washington \", a CBSN video on CBSNews.com. View more CBSN videos and watch CBSN, a live news stream featuring original CBS News reporting.', '2020-02-29 00:00:00.000000', 'First U.S. coronavirus death reported', 2),
(8, 'Nike announced Sunday it would temporarily close its world headquarters in Beaverton, Oregon out of an \"abundance of caution.\" \r\nThere has just been one confirmed case of COVID-19 in Oregon — a worker at an elementary school in Lake Oswego.\r\nThe CDC confirmed Saturday the first US death from the coronavirus, in neighboring Washington state.\r\nVisit Business Insider\'s homepage for more stories.\r\nNike announced Sunday it temporarily closed its corporate headquarters in Beaverton, Oregon in order to deep clean the campus following the first US death from COVID-19 the day prior. ', '2020-03-01 00:00:00.000000', 'Nike closed its worldwide headquarters in Oregon for deep-cleaning after the 1st US coronavirus death', 1),
(9, 'Cal Ripken Jr. congratulates Terps\' Anthony Cowan Jr. on becoming the latest \'Iron Man\' originally appeared on NBC Sports Washington\r\n\r\nAnthony Cowan Jr.\'s time at the University of Maryland has been filled with big buckets in clutch moments. But above all else, Cowan has been one thing for the Terps: consistent.\r\n\r\nOn Wednesday night, for Maryland\'s thrilling last-second win over Minnesota, Cowan started his 127th consecutive game. Now a senior, Cowan has never missed a game in his Maryland career. The start on Wednesday allowed him to pass Keith Booth for the most consecutive starts in school history.\r\n\r\nAn impressive feat, Cowan is now the Terps\' \"Iron Man.\"', '2020-03-01 00:00:00.000000', 'Cal Ripken Jr. congratulates Terps\' Anthony Cowan Jr. on becoming the latest \'Iron Man\'', 2),
(10, 'Robert Downey Jr. struck an Iron Man pose for charity earlier this week. The Tony Stark actor seemingly retired from the role after the events of Avengers: Endgame, so this should be a nice surprise for Marvel Cinematic Universe fans from all over the world. Downey Jr. started to let MCU fans know ahead of time that Infinity War and Endgame were going to be the end of the line for Tony Stark, though he never confirmed it at the time. Instead, he let the movies do the talking for him.\r\n\r\nRobert Downey Jr. posted an image of himself doing the classic Iron Man pose and captioned the image with, \"pulling the old repulsors out of retirement for a good cause.\" The good cause is specifically to benefit Australia\'s tragic bushfire relief. While it\'s only been a year since we\'ve lost Tony Stark, RDJ is still having fun with fans. As an added bonus, he\'s wearing a sweet Van Halen 5150 shirt, which is possibly cooler than his Iron Man pose.', '2020-03-02 00:00:00.000000', 'Robert Downey Jr. Pulls Iron Man Out of Retirement for a Quick Photo', 1),
(11, 'It’s actually crazy to think about how young ScarJo was when she first donned those red locks in Jon Favreau’s Iron Man sequel. She was already a well-known actress for her roles in Match Point, The Island, Lost In Translation or He’s Just Not That Into You, but when she slipped into that leather suit, she soared even higher into the A-list.', '2020-03-02 00:00:00.000000', 'Scarlett Johansson Explains An Unexpected Way Iron Man 2 Role Changed Her Life', 2);
```
