--création de la table : distribution_companies
CREATE TABLE distribution_companies (
  id INTEGER PRIMARY KEY,  company_name TEXT NOT NULL
);

-- insert some values
INSERT INTO distribution_companies VALUES (1, 'Columbia Pictures');
INSERT INTO distribution_companies VALUES (2, 'Paramount Pictures');
INSERT INTO distribution_companies VALUES (3, 'Warner Bros. Pictures');
INSERT INTO distribution_companies VALUES (4, 'United Artists');
INSERT INTO distribution_companies VALUES (5, 'Universal Pictures');
INSERT INTO distribution_companies VALUES (6, 'New Line Cinema');
INSERT INTO distribution_companies VALUES (7, 'Miramax Films');
INSERT INTO distribution_companies VALUES (8, 'Produzioni Europee Associate');
INSERT INTO distribution_companies VALUES (9, 'Buena Vista');
INSERT INTO distribution_companies VALUES (10, 'StudioCanal');

select * from distribution_companies ; 


--création de la table movies
CREATE TABLE movies (
id INTEGER PRIMARY KEY,
movie_title TEXT NOT NULL,
imdb_rating NUMBER(2.2),
year_released NUMBER(4),
budget NUMBER(10.2),
box_office NUMBER(2.2),
distribution_company_id INTEGER,
language TEXT NOT NULL
        ) ; 
-- insert some values
INSERT INTO movies VALUES (1,            'The Shawshank Redemption', 9.2,        1994,    25.00,  73.30,   1,                'English') ; 
INSERT INTO movies VALUES (2,            'The Godfather',              9.2,        1972,    7.20,     291.00,                2,                'English');
INSERT INTO movies VALUES (3,            'The Dark Knight',            9.0,        2008,    185.00,               1006.00,             3,                'English');
INSERT INTO movies VALUES (4,            'The Godfather Part II', 9.0,        1974,    13.00,  93.00,  2,            'English, Sicilian');
INSERT INTO movies VALUES (5,            '12 Angry Men', 9.0,        1957,    0.34,     2.00,     4,            'English');
INSERT INTO movies VALUES (6,            'Schindlers List',             8.9,        1993,    22.00,  322.20,                5,                'English, German, Yiddish');
INSERT INTO movies VALUES (7,            'The Lord of the Rings: The Return of the King',               8.9,        2003,    94.00,                1146.00,             6,            'English');
INSERT INTO movies VALUES (8,            'Pulp Fiction',   8.8,        1994,    8.50,     213.90,               7,            'English');
INSERT INTO movies VALUES (9,            'The Lord of the Rings: The Fellowship of the Ring',      8.8,        2001,    93.00,                898.20,                6,            'English');
INSERT INTO movies VALUES (10,         'The Good, the Bad and the Ugly',          8.8,        1966,    1.20,     38.90,  8,                'English, Italian, Spanish');

select * from movies ;

