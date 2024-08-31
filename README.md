# demo
use ram;
select * from ratings;
SELECT movieId FROM tags
WHERE tag = 'Sci-Fi'

ORDER BY imdbRating DESC
LIMIT 1;

# Mention the movieId of the "Sci-Fi" movie which has the highest IMDB rating.
SELECT * FROM ratings
WHERE movieId IN (109487, 27660, 260, 7254, 6283, 260, 260, 541, 589, 1200, 1240, 2571, 3527, 79132, 109487, 1196, 3527, 68237, 68358, 68791, 72998, 4446, 924)
ORDER BY rating DESC;

# Mention the movieId of the movie which has the highest IMDB rating.
SELECT * FROM ratings
ORDER BY rating DESC
LIMIT 5;

# What is the shape of "movies.csv"
import pandas as pd
data = pd.read_csv("movies.csv")
size = data.size
print("Size = {}".format(size))




